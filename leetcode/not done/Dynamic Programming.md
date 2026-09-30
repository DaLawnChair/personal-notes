**Lookout for:**

**Idea:**
* Visualize problem, typically using a directed acyclic graph.
* Find a subproblem within the problem, ie look for the length of the sequence up to some point rather than the whole sequence
* Find relationship between the subproblems

**Common problems:**
* n length array, subproblem is finding the ordered subsequence of length i
* Sequence of length n, in random order (need to sort first), subproblem is finding the ordered subsequence of length i
* Given 2 sequences, need to find appropriate subsequence of both of these sequences
	* same idea as before
* 2D matrix as input, and need to find submatrix of dimensions less than original 
* (uncommon) problems where the sequence starts in the middle of the sequence
 
**Example:**
* [2466. Count Ways To Build Good Strings](https://leetcode.com/problems/count-ways-to-build-good-strings/)
	* Can make the n'th way by checking the number of ways to make the n-zero and n-one way to make it, base condition 1 way
    * Relies on the idea that `list index of i-idx>=i` for easy syntax of just doing `dp[i-ones] and dp[i-zeros]` 
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
* [198. House Robbers](https://leetcode.com/problems/house-robber/description/)
	* Pretty standard, same idea as coin change
* [213. House Robbers II](https://leetcode.com/problems/house-robber-ii/description/)
	* just House Robbers 1 but doing it twice, once with the last vaule excluded and the other time with the first value excluded
* [91. Decode Ways](https://leetcode.com/problems/decode-ways/submissions/1715306138/) $\star$
	* Use a 1-D DP table keeping track of the number of ways to decode at the the idx of the string s.
	* Need to segment between when the previous character is a 0 and if the current character is a 0.
		* if current is not 0, then you need to consider new ways to generate the charcter if prev is 1 or 2. If so, then it is just the number of ways to make the previous character + before the previous character `dp[i] = dp[i-1] + dp[i-2] if i-2>0 else 1`. Otherwise it continues the streak from before
		* if current is 0, then it is the same there are no new considerations and the response reverts back to 2 previous enteries `dp[i]=dp[i-2] if i-2>0 else 1`
			* if prev is also 0, then the code is invalid if prev is not 1 or 2, thus return 0
	* Many many edge cases when having to deal with 0 


## Kadane's Algorithm
A simple algorithm for calcuating the maximum sum of an array in O(n) time an O(1) space:
```python
  
def max_subarray(numbers):
    """Find the largest sum of any contiguous subarray."""
    best_sum = float('-inf')
    current_sum = 0
    for x in numbers:
        current_sum = max(x, current_sum + x)
        best_sum = max(best_sum, current_sum)
    return best_sum
```
note this doesn't work for empty subarrays, where it should be `best_sum=0` and `current_sum=max(0,current_sum+x)`
A fair amount of "fake" DP problems, ie problems that are solvable as such, but do not have memoization or the same concept that yields a good solution.
This is also a greedy problem

* [5. Longest Palindrome Substring](https://leetcode.com/problems/longest-palindromic-substring/description/)
	* Key idea is that you can compare from inner outwardly and then keep track of what solutions are still palindromes by comparing the new ends. Need to do so for both even and odd lengths
	* DP Approach: use a 2D DP table where the first value is start, second value is end index. Initalize all dp\[i]\[i] values as True (as they are single elements) and all even dp\[i]\[i+1] as true if s\[i]\==s\[i+1] (even palindroms). If dp\[i+1]\[j-1] is a palindrome, then you just need to check over different widths and verify that it is a palindrome
**Conceptual videos:**
* https://www.youtube.com/watch?v=aPQY__2H3tE 
