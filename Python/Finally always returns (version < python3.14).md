

Take the given code block
```python
def perform_compare(value:list, index:int):
    try:
        return 100*values[index] 
    except IndexError:
        print('bad index')
    finally:
        return True 

print(perform_compare([1,2,3],2)) # True, but no print ???
print(perform_compare([1,2,3],4)) # True, but no returned value ???
```

This is weird behaviour, as we expect the try block's return and the printing from the except block.

As per the docs:
**Finally in try-except blocks are always executed before leaving a try statement.**

	A finally clause is always executed before leaving the try statement, whether an exception has occurred or not. When an exception has occurred in the try clause and has not been handled by an except clause (or it has occurred in a except or else clause), it is re-raised after the finally clause has been executed. The finally clause **is also executed “on the way out” when any other clause of the try statement is left via a break, continue or return statement**. A more complicated example (having except and finally clauses in the same try statement works as of Python 2.5):

Reference: https://stackoverflow.com/questions/19805654/python-try-finally-block-returns

Note that this is patched inside of python3.14 with Pep765: https://peps.python.org/pep-0765/

