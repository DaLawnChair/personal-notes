**Lookout for:**
* Solutions of O(log(n)), or a very optimal solution
* Finding values in a sorted list pattern (any sorted list)
* For asking questions regarding first instance, smallest such instsance, within an array  
**Idea:**
```python
def binarySearch(list: List[],target:object) -> int: 
	# Where list is a sorted array
	low = 0
	high = len(list)-1
	
	while low<high:
		mid = (low+high)//2
		if list[mid]==target: # target found
			return mid
		elif list[mid]>target: # too far, reduce upper bound
			high=mid-1
		else: # too low, reduce lower bound
			low=mid+1
	return -1 # not found
```
Complexity
* Time Complexity: $O(log(n))$
* Space complexity: $O(1)$

This is the most simple case we see, but is there a more general solution that encapsulates more information (ie duplicates?)
```python
def generalize_binarySearch(list: List[],target:object) -> int: 
	"""
	We return 2 values, first one will point to the index where we'd want to insert a new value next to the target, and the index of the target inside of list, if it exists 
	"""
	# Where list is a sorted array
	low = 0
	high = len(list)-1
	
	while low<=high:
		mid = (low+high)//2
		if list[mid]<=target:
			low=mid+1
		else:
			high=mid-1

	# add a case when value is not found
	if not (high>0 and high<len(list) and list[high]==target):
		return low, -1
	return low,high # high will point to the last instance where list[mid]==target, and low will point to the value after it (ie the item where you want to add an element the right of target) 
```
* The property of returning the left pointer is exactly that `bisect.bisect_right(items,target)` does
* This will inheritenly make right point to the last instance of the value,
	* if we are to want to get the first instance, we will want to change the line to `if list[mid]<target:`
		* the left pointer will be the index of which we should add another element after the first instance of target, which is what `bisect.bisect_left(items,target)` 

Bisect right algorithm:
```python
 def bisect_left(arr, low, high, target):
    
    while low<high:
        mid = (low+high)//2 
        
        if arr[mid]<= target: # increase
            low = mid 
        else:
            high = mid-1
    return low


print(bisect_left([10,11,13,50], 0, 4, 20))
print(bisect_left([10,11,13,15,18,19,50], 0, 7, 20))
print(bisect_left([10,11,13,15,18,19,50], 3, 7, 20))
print(bisect_left([10,11,13,15,18,19,50], 0, 7, 10))
```


When should `low<=high` or `low<high`?
* Look out for special cases such as `[1]`
* `low<=high` always holds if you don't mess it up
* Think about the search interval, is it `(left,right]` or `(left,right)`?
When to do `right=mid` or `right=mid-1`?
* Look into what is need for the question
	* If you need minimum, that may mean you want the search intervals of `[left, mid) and [mid+1,right)` and so we use `right=mid` to shrink the left boundary
	* In this very vain, is `mid` inside of the new boundary you want to test? If so, we use `right=mid`
Infinite loops:
* choice of low, right, and while condition depends on the choice here
	* always have it so that we have exactly 1 value left after the while loop terminates
	* Think the case of having 2 elements left, does the loop terminate? If not, reconsidered your choice on the low and right conditions

Off by one error:

**Example:**
* [875. Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/)
	* Make a new sequence where from  `[1,2,...,max(pile)]` is the domain where we binary search for the lowest possible value for the # of bananas we eat. We want to minimize the lower bound so we do `left=mid+1` or `high=mid` while `low<high` 
* [153. Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/description/) 
	* Binary search, but we need to find the mimumum of an already sorted list, so our target to beat is actually the right pointer (or the left, we choose one and minimize that to pick the side). Because of its sorted nature, the minimum will be in 1 of the halves of the list, so find it within the half. `right=mid` or `left=mid+1`. We then return the mimimum side, `nums[left]` as that must be the minimum
* [33. Search in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/description/) $\star\star\star$
	* `[too long to type]`
	* https://www.youtube.com/watch?v=U8XENwh8Oy8
	* Way better strategy is just split find the pivot through `nums[i-1]>nums[i]`, and then doing binary search on the two sides. Then take conditions based on which one is none and return the other
* [981. Time Based Key Value Store](https://leetcode.com/problems/time-based-key-value-store/description/)
	* Adding a hashmap to a binary tree in for most recent value of a given key
**Conceptual videos:**
* Basics and why we choose the boundaries and pointer values: https://labuladong.gitbook.io/algo-en/iii.-algorithmic-thinking/detailedbinarysearch
* Similar to above: https://leetcode.com/problems/binary-search/solutions/423162/Binary-Search-101-The-Ultimate-Binary-Search-Handbook/
* Good generalization of binary search and the meaning behind the our if/else conditions: https://www.youtube.com/watch?v=1IOp0jyu128
