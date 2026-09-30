**Lookout for:**
* Sequential movement through the array
* Counting # of values
* finding min/max of a sequence
**Idea:**
* Pointer at both ends:
	* Set up 2 pointers at both ends
* Fast/Slow pointer:
	* set up 2 pointers, both at the start, but one increments faster than the other (usually in link list problems)
* Iterate over the array, based on some criterion, increment `l` or decrement `r`
* `Note:` there are a lot of parallels between binary search, two pointers, and sliding window
**Example:**
* [15. 3Sum](https://leetcode.com/problems/3sum/description/) (two pointer)
	* Must sort the array first because `i<j<k`. First choose i value over all values. If that I is already seen, then we can skip it because enteries must be unique. Then iterate inside `[i+1,n]` where we denote 2 pointers j and k respectively to them. Calculate the 3 sum and add to `res`. Reduce k or increase j if 3 sum does not achieve target, increment j if the value is the same as previous j.
	* Highly recommend looking at the non-sorted version
		* Key idea is that you can have dups be the one to avoid duplicate usage values, and that you can keep track of complements by using a dictionary of complement and index i to avoid duplications
		* For ordering, you need to sort the indicies of the 3sum solution
```python
class Solution:
    def threeSum(self, nums: List[int]) -> List[List[int]]:
        res, dups = set(), set()
        seen = {}
        for i, val1 in enumerate(nums):
            if val1 not in dups:
                dups.add(val1)
                for j, val2 in enumerate(nums[i + 1 :]):
                    complement = -val1 - val2
                    if complement in seen and seen[complement] == i:
                        res.add(tuple(sorted((val1, val2, complement))))
                    seen[val2] = i
        return [list(x) for x in res]
```

* [11. Container with the most water](https://leetcode.com/problems/container-with-most-water/description/) (two pointer)
	* have pointers on each end. Slide towards the larger value.
* [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/submissions/1494555888/) (two pointer) $\star\star\star$
	* `[hard conceptuall, watch video]` https://www.youtube.com/watch?v=ZI2z5pq0TqA
	* actually very simple when brought down into conditions for when to choose left and right and the math behind the 3 cases of the max value and the current height
		* can be done numerous other ways, but two pointer is the best as it only contains 2 pointers, 
        * alternative solution is to view it as water contained is `min(max_left[i],max_right[i]) - height[i]` for every position i, taking the value if it is >0. 
        * two pointer solution utilizes the fact that we are bounded by our max_left[i] or max_right[i] value when calculating the water contained
**Conceptual videos:**
* https://www.youtube.com/watch?v=On03HWe2tZM
