


## []
**Lookout for:**
    * (too general to say, look into other methods for classification for the type of problem)
**Idea:**
**Example:**
* [1769. Minimum number of Operations to Move All Balls to Each Box](https://leetcode.com/problems/minimum-number-of-operations-to-move-all-balls-to-each-box/)
	* similar to the product of all but self question
	* count locations of 1s, then do left and right pass of the array over all ones except for the start of each ends
    * can additionally collpase it down to 1 for pass by knowing the positions of the balls as increasing in balls from the left is decreasing in the balls for the right

* [128. Longest Consecutive Sequence](https://leetcode.com/problems/longest-consecutive-sequence/description/)
* conceptually just need to check that the `nums[i]-1` element is not in the list, then this is the start of the sequence, and then check for later numbers `nums[i]+n` for the length of the streak
**Conceptual videos:**
