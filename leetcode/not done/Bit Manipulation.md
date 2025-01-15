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
* 
**Conceptual videos:**