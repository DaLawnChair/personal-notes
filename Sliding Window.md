## Sliding window 
**Lookout for:**
* Contiguous, sequential groupings
* Longest/smallest/contains/ max/min
* Substrings/sub-arrays/sub-linked lists 
**Idea:**
* You can iterate sequentailly over the data and draw a 'window' of a region and keep track of this window's properties while you iterate through the whole domain

**Example:**
* [209. Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/)
```python
def minSubArrayLen(self, target: int, nums: List[int]) -> int:
	minWindowSize = float('inf')
	currWindowSum = 0
	windowStart = 0
	for windowEnd in range(len(nums)):
		currWindowSum += nums[windowEnd]
		while currWindowSum >= target:
			minWindowSize = min(minWindowSize, windowEnd-windowStart+1)
			currWindowSum -= nums[windowStart] 
			windowStart += 1
	return minWindowSize if minWindowSize!=float('inf') else 0
```
**Conceptual videos:**
* General approaches to sliding window: https://www.youtube.com/watch?v=MK-NZ4hN7rs&list=WL&index=1&t=152s