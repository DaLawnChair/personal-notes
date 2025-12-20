Note that python stores values as objects, so we can see that may things take up way more space than what might be needed:

```python
>>> import sys
>>> y = 32
>>> sys.getsizeof(y)
28
```


We can use libraries to ensure that the values are smaller:
## Ctypes:
```python
>>> import ctypes
>>> import sys
>>> x = ctypes.c_int32(123)
>>> sys.getsizeof(x)
128
```
But it is 128, which is more than the Pyhton integer? Yes, because this includes the wrapper as a part of it.

## Array: using the native list type for a specified datatype
```python
>>> import array
>>> import sys
>>> 
>>> arr = array.array('i', [123])
>>> print(sys.getsizeof(arr))        # Includes array overhead, still compact
84
>>> print(arr.itemsize)              # 4 bytes per element
4
>>> arr_large = array.array('i',[123,424,232,23123,23123])
>>> print(sys.getsizeof(arr_large))        # Includes array overhead, still compact
100
>>> print(arr_large.itemsize)              # 4 bytes per element
4
```


Compare this with just lists
```python
>>> arg = [123]
>>> sys.getsizeof(arg)
64
>>> arg_large = [123,424,232,23123,23123]
>>> sys.getsizeof(arg_large)
104
>>> sys.getsizeof(arg_large[0])
28
```


Numpy arrays is the same as it will show the change in allocation depending on the sizing allocated for it

```python
>>> import numpy as np
>>> np_arr = np.array([123],dtype=np.int8)
>>> sys.getsizeof(np_arr[0])
25

>>> np_arr = np.array([123],dtype=np.int64)
>>> sys.getsizeof(np_arr)
120
>>> sys.getsizeof(np_arr[0])
32

>>> np_arr = np.array([123,424,232,23123,23123],dtype=np.int64)
>>> sys.getsizeof(np_arr)
152
>>> sys.getsizeof(np_arr[0])
32
```
Torch tensors remain the same size

```python
>>> import torch
>>> tensor = torch.tensor([123])
>>> sys.getsizeof(tensor)
88
>>> tensor_large = torch.tensor([123,424,232,23123,23123])
>>> sys.getsizeof(tensor_large)
88
>>> sys.getsizeof(tensor_large[0])
88
>>> sys.getsizeof(tensor_large[1])
88

# and only it isn't affected by the data type:
>>> tensor_large = torch.tensor([123,424,232,23123,23123],dtype=torch.int64)
>>> sys.getsizeof(tensor_large[1])
88
```