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

**Conceptual videos:**