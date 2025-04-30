## []
**Lookout for:**

**Idea:**
**Example:**
* [45. Jump Game II](https://leetcode.com/problems/jump-game-ii/description/) $\star \star \star$
	* Works by iterating over the entire list, checking for the largest jump possible using 2 pointers, largestJump for the largest jump possible from a previous position, and curr_end, the ending for that largest jump
* [55. Jump Game](https://leetcode.com/problems/jump-game/description/)
	* work backwards, think of getting from the end to the beginning. If we can go from currPos from lowerPos+nums[lowerPos], then can then solve for the sub problem of getting to lowerPos in the first place

**Conceptual videos:**