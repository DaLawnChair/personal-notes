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
	* 
**Conceptual videos:**