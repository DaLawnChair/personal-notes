**Goal:** We want to interface and call methods/classes from C/C++ with the ease of using Python.


**Marshalling**: The process of transforming the memory representation of an object to a data format 
suitable for storage or transmission.
* As C/C++ is much more verbose on the data types it has and Python just declares all datatypes as an object, we need to convert a C datatype into a Python one.
* Strings can be hard to represent during marhsalling
* Differences in pass-by-reference and pass-by-value
	* Inherently C/C++ always do pass-by-value, but for Pyhton it depends on if the value is immutable (pass-by-value) or mutable (pass-by-reference)
* Managing memory:
	* Everytime you create a non-smart pointer, you need to deallocate the reference and the memory.



# Binders
PyBind11:

CPPYY: Automatic C++ binding in python
* Given a C++ library or plain C++ formated code, this package simply uses clang to compile the the code using cling as the parser and allows the user to run C++ binded code.

Format:
```python
import cppyy

# include the package to include. If the original code is #include <package>, then th e package is the raw name
cppy.include("package")

# instantiate code here, can be raw code from a .cpp file
cppy.cppdef("""<CPP CODE HERE>""")

# load a library given just the name (no extension). Just works automatically with .dll and .so 
cpp.load_library("Library_name")

#
```
Note that the docs mention functions with Numba, however this requires the pypy interpreter, otherwise the import of `import cppyy.numba_ext` will lead to a crash related to missing `__pypy__` the `cppyy/reflex.py` 

# Reference:
https://realpython.com/python-bindings-overview/
- Guideline for how all of this is done

https://cppyy.readthedocs.io/en/latest/index.html
* cppyy docs
* Can use Numba if using pypy as the interpreter

