## []
**Lookout for:**

**Idea:**
**Example:**
* [50. Pow(x,n)](https://leetcode.com/problems/powx-n/)
	* Specifically need to turn integer for n to double
	* Cases for `n<0` is the same for `n>0`, just need to change `x=1.0/x` 
	* Recall these principles:
		* If n is odd, then `x^n = x * x^(n-1)`, so do `result = result * x; n=n-1`
		* If n is even, then `x^n = (x^2)^(n/2)` so do `x = x^2; n=n/2`
* [2429. Mimimum XOR](https://leetcode.com/problems/minimize-xor/description/?envType=daily-question&envId=2025-01-15) $\star \star \star$
	* Get the count of set bits with `bin(num1).count("1")` for both numbers
	* Recall the mimimum augmentations to num1 to get the same number of set bits as num2.
	* Take cases
		* If equal, then return num1
		* if count for 1 >2, then decrease num1 from top to bottom
		* if count for 1 <2, then increment num1 from bottom to top, filling in indicies of 0s
* [2425. Bitwise XOR of All Pairs](https://leetcode.com/problems/bitwise-xor-of-all-pairings/description/?envType=daily-question&envId=2025-01-16) $\star$
	* Property of `a XOR a = 0` and XOR is communative, so if the len of nums2 is even, then we perform an even number of XOR for each element of nums1, thus nums1 values equate to 0. Same goes for len of nums1 being even, then nums2 elements don't account. 
	* Thus take 2 values for XOR'ing each list, defaulting to 0 if the len of the other list is even. Return the XOR of these two sum values.
**Conceptual videos:**