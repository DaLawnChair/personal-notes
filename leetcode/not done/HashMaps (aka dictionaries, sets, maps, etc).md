## []

Typically use `defaultdict()` to have a dictionary that can be accessed without any elements in `dict[key]=value` and don't need to use `dict.get(key,<default>)`.

**Lookout for:**
* Counting
* Unique values/ duplicates
* Encoding where previous vales were in a sliding window

**Idea:**
* Store values inside of a key, value pairing where the key is distinct 
**Example:**
* [Two Sum](https://leetcode.com/problems/two-sum/)
	* Uses a hashmap to map differences and list entry, return `[values[difference],<current value>]`
* [347. Top K Frequency Elements](https://leetcode.com/problems/top-k-frequent-elements/description/)
	* Make a hashmap for value:frequency pairs. Then make a double list where the index is frequency and the values in that index are values of that frequency
	* count from the top, look at the values inside of the double list, and append values from there until you reach k. Once full, you are done and can submit the k most frequent elements
* [3223. Minimum Length of String After Operations](https://leetcode.com/problems/minimum-length-of-string-after-operations/description/?envType=daily-question&envId=2025-01-13)
	* operations is based on parity. If frequency of values is odd, then there can be 1 left. If its even, then there will be 2 left.

* [15. 3Sum](https://leetcode.com/problems/3sum/) $\star$
* easiest solution is make 2 for loops, one to iterate through i nested is iterating through j, making sure to skip duplicate values. Then check that `target=nums[i]+nums[j]` and check if target exists in the list and that it `target>=nums[j+1]` to avoid duplicates
* a smarter solution it too keep count of frequencies of each item in a Counter, and to store the values in 2 sets, one positive and one negative. Then iterate over the two sets as a nested for loop, checking that `target=-(pos+neg)` exists in the list, and if so, then based off the values of `0=target+p+n`then we know that if `target==p`, then the we get `[p,p,n]`, if `target==n`, then `[n,n,p]`, and if `n<target<p`, then `[n,target,p]`. Note that the solutions does not require checking ordering.
**Conceptual videos:**
