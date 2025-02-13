## []
**Lookout for:**

**Idea:**
* Visualize problem, typically using a directed acyclic graph.
* Find a subproblem within the problem, ie look for the length of the sequence up to some point rather than the whole sequence
* Find relationship between the subproblems

**Common problems:**
*  n length array, subproblem is finding the ordered subsequence of length i
* Sequence of length n, in random order (need to sort first), subproblem is finding the ordered subsequence of length i
* Given 2 sequences, need to find appropriate subsequence of both of these sequences
	* same idea as before
* 2D matrix as input, and need to find submatrix of dimensions less than original 
* (uncommon) problems where the sequence starts in the middle of the sequence
* 
**Example:**
* [2466. Count Ways To Build Good Strings](https://leetcode.com/problems/count-ways-to-build-good-strings/)
	* Can make the n'th way by checking the number of ways to make the n-zero and n-one way to make it, base condition 1 way
* [322. Coin Change](https://leetcode.com/problems/coin-change/)
	* The max possible value for # of coins is amount+1 because the value coin is `1<=coin`
	* We can make a dp table where the index is the amount and the value is the # of coins needed to get that `ith` amount
		* Base case is 0 because we cannot make an amount of 0
	* iterate over all coins checking that we are still in bounds, then take the minimum of `dp[i]` and `dp[i-coin]+1` to see if having this coin is optimal
	* return -1 if `dp[amount]==amount+1` (max case, so cannot be done) and `dp[amount]` otherwise
* [518. Coin Change II](https://leetcode.com/problems/coin-change-ii/submissions/1496773127/)
	* The # of ways to make the ith value inside of the dp table is based on `dp[i] + dp[i-coin]` for all coins. Because of this we have 2 loops, the first one is for iterates over all coins, then the internal one loops over `[coins[i], amount+1]` for values that it can control. And here we count the # of ways we can make this.
	* I was thinking before the other way, counting the values and then count the coins that can solve it like in the original coin change problem. However that way was convoluted since
		* it double counted every value (ie 5 = 1+1+2 was double counted with 5 = 2+1+1)
		* also worried about the conditions on when and how to increment the count.
	* The former version doesn't double count becasue of our choice of start and end. 
**Conceptual videos:**
* https://www.youtube.com/watch?v=aPQY__2H3tE 