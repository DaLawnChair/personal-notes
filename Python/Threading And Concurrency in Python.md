# Python is NOT single threaded
Even using `threading` allows you to spawn in threads that are handled at the system level, thus these are not actual threads.
* it is single threaded in the base case of it, without any packages and such that makes it operate outside of a thread, which most languages do

No matter if you use `threading` or not, the program will have a single shared lock called the Global Interpreter Lock (GIL) that will force the system to operate on **one core**.

If you want o use more than one core, use `multiprocessing`


# Python is single threaded

https://www.youtube.com/watch?v=dyhKXCpkCGE
Due to the CPython implementation, Python is limited to being used as a single threaded program if you use threads as the GIL will prevent multipule threads from operating  on the same python bytecode. 

This is enherent, and most libraries that work with python and want some compuation spread out elects to use processes instead.

### How to avoid this?
* Use processes
* Use C extension libraries that's implementation avoid this (numpy, tensorflow)
* Change the python implementation
* Asynchio - Asycnhronous I/O tasks concurrency (without threads)
	* Though this is yield based, and thus has a similar limitation as the thread
* Use Python13.3, which allows for no GIL which can be defined during the build
# Njit 
Note that NJit is also limited by the GIL. To ignore it, you must pass the `nogil=True` inside of its decorator or constructor.

ie
`njit(func,nogil=True)`

You can see this with system manager on the python program; it will not exceed 100% usage, but with `nogil=True`, it can.


# concurent

Has a nice function for performing multitasking.

```python
from concurrent.futures import ThreadPoolExecutor

# Map: performing the task right now
with ThreadPoolExecutor(numOfThreads) as ex:
	"""
	func: function of iterables that can be executed asynchronously and concurrently
	timeout: 
	chunksize: only useful for ProcessPoolExecutor, as with ThreadPoolExectutor it will not change from the default of 1
	"""
	ex.map(func, iteratiables, timeout=None, chunksize=1)

# submit: perform the task later
with ThreadPoolExecutor(numOfThreads) as ex:
	"""
	func: function of iterables that can be executed asynchronously and concurrently
	timeout: 
	chunksize: only useful for ProcessPoolExecutor, as with ThreadPoolExectutor it will not change from the default of 1
	"""
	future = ex.submit(func,*args. **kwargs)
future = future.result()
```
#### References:

https://www.youtube.com/watch?v=m2yeB94CxVQ
* Python is not single threaded