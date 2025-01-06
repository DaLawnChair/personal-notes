**Lookout for:**
* Solutions of O(log(n))
* Finding values in a sorted list pattern (any sorted list)
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
**Example:**
* [875. Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/)
	* Make a new sequence where from  `[1,2,...,max(pile)]` is the domain where we binary search for the lowest possible value for the # of bananas we eat. We want to minimize the lower bound so we do `left=mid+1` or `high=mid` while `low<high` 
* [153. Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/description/) 
	* Binary search, but we need to find the mimumum of an already sorted list, so our target to beat is actually the right pointer (or the left, we choose one and minimize that to pick the side). Because of its sorted nature, the minimum will be in 1 of the halves of the list, so find it within the half. `right=mid` or `left=mid+1`. We then return the mimimum side, `nums[left]` as that must be the minimum
* [33. Search in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/description/) $\star\star\star$
	* `[too long to type]`
	* https://www.youtube.com/watch?v=U8XENwh8Oy8
* [981. Time Based Key Value Store](https://leetcode.com/problems/time-based-key-value-store/description/)
	* Adding a hashmap to a binary tree in for most recent value of a given key
**Conceptual videos:**
* Basics and why we choose the boundaries and pointer values: https://labuladong.gitbook.io/algo-en/iii.-algorithmic-thinking/detailedbinarysearch
* Similar to above: https://leetcode.com/problems/binary-search/solutions/423162/Binary-Search-101-The-Ultimate-Binary-Search-Handbook/