**Lookout for:**
* Typically given to you that it is a palindrome question
* Typically look at using a char list of `counts = [0]*26` for counting the occurances of each letter for each letter
* Do something regarding it to check if the values are palindromes or not
**Idea:**
**Example:**
* [1400. Construct K Palindromes] (https://leetcode.com/problems/construct-k-palindrome-strings/description/?envType=daily-question&envId=2025-01-11)
	* get counts of all letters. 
	* Palindromes => odd occurances <= splits that are palindromes
	* Base cases of `len(string)<k` is not possible; `len(string)==k` is always true since a single letter is a palindrome


* [647. Palindrome Substrings](https://leetcode.com/problems/palindromic-substrings/description/) $\star$
    * conceptually the same idea as proposed as in expand from center algorithm for palindromes 
    * can be done in many different ways, but the DP solution can be solved in 2d and 1d:
        * 1d (by me): consider all the indices of a given letter. Check if s[prev_i:i+1] is a palindrome and add 1 to the dp[i] if it is. Then add in 
        dp[i] += dp[i-1] as they are all palindromes before it 
        * 2d (published): consider a 2D dp table where where i and j represent the substring composed from idx i to j. Add in base cases of dp[i][i]=True 
        and if the same double letter strings are present. Then do a double for loop, the outer one to handle lengths of 3 to n, the inner one will iterate 
        over all i and j values between i to n to verify and check if s[i]==s[j] and the inner term dp[i+1][j-1], thus verifying that they are a palindrome.
    * can be solved by the Manacher's Algorithm, which does so in O(n) time and space complexity.
        * implementation of the expand from center algorithm 
        * does both even and odd cases by appending unused values before and after each character, so length is only odd 
        * For i between 0 and n, we calculate the radius of l and r boundaries. If i extends beyond r, then we update l and r to recenter it.
        * we verify until false that i is within the radius and that the mirrors values across the padded string are the same.
        * We intern get a list of radius where we have palindromes. This is double counted so we will do (p[index]+1)//2
    * intuition of the Manacher's Algorithm:
        * [][] todo
**Conceptual videos:**
