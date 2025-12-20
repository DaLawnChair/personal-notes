You can set the traceback for python script after the following line is ran 

```python
import pdb
pdb.set_trace()

#or alternatively
breakpoint()
```

Alternatively you can enter into the file with 
```bash
python3 -m pbd script.py
```

Inside of PDB:
```bash
n  # next line
p args # view the contents of args at this breakpoint
q  # quit debug
```

Parsing the output
```python
# denotes the line number of the script ran, and that it is of type module/function_name.
# Next line is showing the line being called
> .../path/script.py(number)<module>()
-> func(args)

# if you want to see what values of args is, run 
(pdb) p args
<value of args>

```


# References
https://www.youtube.com/watch?v=0LPuG825eAk