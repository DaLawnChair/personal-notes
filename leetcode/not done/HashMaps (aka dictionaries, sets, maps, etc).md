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
**Conceptual videos:**