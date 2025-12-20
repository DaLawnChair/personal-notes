
Function evaluations inside of compile time



## Requirements for usage:
* arguments must be literal (ie int, char, value must be known at compile time)
* recursive function must have base case
	* base value case must be known at compile time
* enough memory to compile the function, recursion depth limits, 
* Most things need to be known at compile time, like types, sizes, etc. [][] check over

Take for example the time it takes to get the fibbonacci value for 35
```cpp

int fibonnacci(int n){
	if (n<=1) return n;
	return fibonnacci(n-1) + fibonnacci(n-2)
}
// time: 40720 microseconds

constexpr int fibonnacci_c(int n){
	if (n<=1) return n;
	return fibonnacci_c(n-1) + fibonnacci_c(n-2)
}
// time: 38 microseconds
```

So the function is a 1000x speed up, which is not entirely accurate due to clock readout time. But why? and when is this useful?

* Why is it faster?
	* constexpr compresses the recursive calls down into a single function call inline for a given value at compile time. 



# Reference:
https://www.youtube.com/watch?v=8-VZoXn8f9U&t=72s
