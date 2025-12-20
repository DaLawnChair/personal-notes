# Chapter 1.

1.2.2
$8n^2 < 64nlog_2(n)$. Find n.
$n < 8log_2(n)$
$n - 8log_2(n) < 0$
Let $y=n-8log_2(n)$
	$y' = 1-8/ln(2)n$
	$y' = 1-8/ln(2)n=0$
	$=> n = 8/ln(2) = 11.5415$
	and
	$y'' = 8/ln(2)(n^2) > 0 $
So n=8 is a local minimal. Taking limits we see that y will go to +ve inf as n goes to inf and y goes to -ve inf as n goes to -ve inf. Thus there should be two zeros. 

To find the points of which these y=0, use Newton's method:
	n=12 
		x_{n+1} = n - y(8)/y'(8) .... = 43.559525 = 43
	n=11
		x_{n+1} = n - y(8)/y'(8) .... = 1.1
	
Thus insertion sort is faster from n=1 to n=43.

1.2.3
$100n^2< 2^n$
$100n^2 - 2^n < 0$

Let $y=100n^2 - 2^n = 0 $
	$y'=200n - ln(2)*2^n$
	$y''=200 - ln(2)*ln(2)*2^n$
Becasuse we want the lower bound, we want to find the upper bound for n.
As n goes to +ve inf, then y' and y'' goes to -ve inf.
So the function is decreasing after this point and had a downward curvature. So that means that the zero found will be the upper bound.

Using newton's method for a large n, yields 14
	
	
## Chapter 2
2.1.2
```python
def reverse_insertion_sort(arr):
	n = len(arr)
	for j in range(2,n):
		key = arr[i]
		i = j-1
		while i>0 and arr[i]<key:
			arr[i+1] = arr[i]
			i=i-1
		arr[i+1] = key
			
		
```

2.1.3
```python
def linear_search(arr,target):
	specialNIL = NILL
	for i in range(len(arr)):
		if arr[i]==target:
			return i
	return specialNIL
```
Loop invariant initalizes to 0, increases by 1 and stops if target is found at index i, otherwise will termiante when i\=\=len(arr)

2.1.4
Input: 2 n-element arrays to represent the bit representaiton of two integers A and B
Output: the sum of the two array, C

```python
def sum_of_bits(a,b):
	carry = 0
	N = max(len(a),len(b))
	while i in range(N,0,-1):
		C[i+1] = (carry+a[i]+b[i]) %2
		if carry+a[i]+b[i] >=2:
			carry = 1
		else:
			carry = 0 
	C[0] = carry
```