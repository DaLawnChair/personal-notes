For programs that are small enough to fit within the cache, cache locality and branch predicitability become more dominent factors in determining speed than Big O complexity.


When you access the value from an object, you are calling the OS to get the value inside of the memory location and load it into cache. In actuality it pulls in a chunk of memory that is related to it, like other fields of the object. When a memory access is already loaded into cache, then it is called a cache hit and it is very fast to find the value. If it isn't, then it must fetch it to read it, this is called a cache miss and it is very slow comparitively.

Accessing memory in consectutive order like in insertion sort makes lots of cache hits, so it is very fast. Random accessing can be slower because of the cache misses, though you need enough memory to achieve this (most noticable with >cache memory size amounts).


For matrix multiplication, the order of accessing i,j,k matter for cache locality. Though this isn't as big of an effect for larger matricies because you will end up doing threading of smaller blocks of the matrix




Branch Predictability
How often are the guesses of the processor correct at predicting future behaviour of conditional statements?

If there is some underlying pattern at run time that the processor can see, then it may be more probable to select the option that occurs the most and precompute the value before it is realized.

However, the compiler may just convert the conditional statement into a deterministic one by optimizing it away into one without branching.

 

Reference:
https://www.youtube.com/watch?v=EmzdmqUWq3o
