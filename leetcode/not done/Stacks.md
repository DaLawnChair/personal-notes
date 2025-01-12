## []
**Lookout for:**
* Some sense of validitity through ordering
**Idea:**
* A stack lets you add elements to the end of the stack using `append(item)` and pop to remove elements at the front with `pop()`  
**Example:**
* [20. Valid Parethesis](https://leetcode.com/problems/valid-parentheses/)
	* Make a stack. If the value is the corresponding alternative one, then you pop it, otherwise then invalid
* [2116. Check if a Parentheses String can be valid](https://leetcode.com/problems/check-if-a-parentheses-string-can-be-valid/description/?envType=daily-question&envId=2025-01-12)
	* Base case is if length of the string is odd, then there is no such parentheses combination that is valid, so return False
	* Keep count of unlocked values and open brackets that are forced open from being `locked[i]='('`
	* If we see `locked[i]=='1' and s[i]==")"`, then we must immediately validate it with a previous index. First we try to use the open brackets, then used the option brackets. If neither work, the string is invalid and we return False
	* After iterating over the entire string, check if there are any more open brackets and if there are, is there an unlockable bracket that we can close it with. If not, return False. Return True at the end if all conditions pass
**Conceptual videos:**