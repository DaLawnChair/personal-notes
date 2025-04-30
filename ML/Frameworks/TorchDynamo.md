* Python level Just-In-Time compiler to make torch programs faster with limited modification
* Hooks onto evaluation APIs in CPython (pep 523) to dynamically modify Python bytecode before execution
* Aims to improve usability and performance


How it is done:
* Rewrites Python bytecode into Pytorch sequence operations that can be fed into an FX graph, which is then compiled into 

How to use:
* Simply add the decorator to the function
```python
import torch
from torch import _dynamo as torchdynamo
def my_compiler(gm: torch.fx.GraphModule, example_inputs: List[torch.Tensor]):
    print("my_compiler() called with FX graph:")
    gm.graph.print_tabular()
    return gm.forward  # return a python callable

@torchdynamo.optimize(my_compiler)
def toy_example(a, b):
    x = a / (torch.abs(a) + 1)
    if b.sum() < 0:
        b = b * -1
    return x * b
for _ in range(100):
    toy_example(torch.randn(10), torch.randn(10))	
```

Explainability of the compilation:
* Download `depf` for byte level compilation of the code
	* run `pip install depf`
	* In the python file, add the lines
```python
import depyf
depyf.install()
```
* Run code with `TORCH_LOGS="+dynamo,guards,bytecode"` to view outputs
	* The output will contain 2 sections
		* FX graph
		* Possible Source code
`[[]] There is a lot of unpacking for what the full meaning of everything is and how it is compiled that can be found from the reference`

The above example yields:
```python
def toy_example(a, b):
    __temp_1 = __compiled_fn_0(a, b)
    x = __temp_1[0]
    if __temp_1[1]:
        return __resume_at_30_1(b, x)
    return __resume_at_38_2(b, x)
    
```
Functionally we have the same code that 
* is converted into a graph of sub functions
* compiled into optimized sub functions
* assembled into a new, equivalent function that is optimized to have good computation speed

Here is a diagram of what is done:
![[dynamo example.png]]

Reference:
https://pytorch.org/docs/stable/torch.compiler_dynamo_overview.html