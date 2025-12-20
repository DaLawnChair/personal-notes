
What is the quickest way to sort integers/floats?

General sorting solutions are O(nlogn). However the constraint of dealing with the bit representation of integers and floats allows for a different representation and thus different approaches. Take the example of integers, though the same premise applies to floats.

Commonly used to represent integers is int32. We can think of int32 as just concatenated versions of two int16 numbers.


The general premise of radix sort is that the two int16 numbers can be "bin sorted" by passing in the value and evaluating if the value fits in a designed bin. These bins can be mod 10 or larger, just depends on the implementation. The bin size is denoted by d.

If we run bin sorting with the two int16 values, then we can effectively sort the values as long as we keep track of the values of which the partition belonged to.

Consider the ordering:
Larger value first, smaller value second:
* This seems intuitive as the correct approach, but this yields incorrect results. Yes the most significant value will be ordered, but the least significant one will require more iterations to perform

Smaller value first, then larger value second:
* This yields an interesting results. If you sort by smaller value first, the relative ordering for the values will be the same as the final results
Below is a good example of what I mean:

Thus we have a way to effectively sort integer numbers. The time complexity will be O(n+d), where n is the number of bits and d is the dimensionality of the given bins.

This is often times 7x faster than quick sort for n>10_000. However this is slower for smaller values. Defining smaller paritions from int16 to int8 yields better results for smaller n values, however less benefit for larger n.



References:
https://www.youtube.com/watch?v=Y95a-8oNqps

