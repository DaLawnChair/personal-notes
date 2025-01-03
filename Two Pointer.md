**Lookout for:**
* Sequential movement through the array
* Counting # of values
* finding min/max of a sequence
**Idea:**
* Pointer at both ends:
	* Set up 2 pointers at both ends
* Fast/Slow pointer:
	* set up 2 pointers, both at the start, but one increments faster than the other
* Iterate over the array, based on some criterion, increment `l` or decrement `r`
* `Note:` there are a lot of parallels between binary search, two pointers, and sliding window
**Example:**
* [15. 3Sum](https://leetcode.com/problems/3sum/description/) (two pointer)
	* Must sort the array first because `i<j<k`. First choose i value over all values. If that I is already seen, then we can skip it because enteries must be unique. Then iterate inside `[i+1,n]` where we denote 2 pointers j and k respectively to them. Calculate the 3 sum and add to `res`. Reduce k or increase j if 3 sum does not achieve target, increment j if the value is the same as previous j.
* [11. Container with the most water](https://leetcode.com/problems/container-with-most-water/description/) (two pointer)
	* have pointers on each end. Slide towards the larger value.
* [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/submissions/1494555888/) (two pointer) $\star\star\star$
	* `[hard conceptuall, watch video]` https://www.youtube.com/watch?v=ZI2z5pq0TqA
**Conceptual videos:**
* https://www.youtube.com/watch?v=On03HWe2tZM