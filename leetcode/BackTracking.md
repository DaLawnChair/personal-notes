

**Lookout for:**
* You want to perform some combinatorical construction of the results by adding in elements to a previous result
**Idea:**

```python
def problem(candidates:list[any], target) -> list[any]:

    finished_set = []
    temporary_set = [] 

    def backtrack(candidates, idx): # use idx in case you need it 
        for i in range(len(candidates)):
            # selection of criterion of candidates[i]
            
            if candidate_to_finish_at:
                finished_set.append(temporary_set.copy())
            temporary_set.append(candidates[i]) # test backtrack with new element
            backtrack(candidates, i+1)
            temporary_set.pop() # undo that element, and try the next one next iteration
    
    backtrack(candidates,0)
    return finished_set
```

**Example:**
* [78. Subsets](https://leetcode.com/problems/subsets/description/)
	* Essentially just need to define the backtrack as "add new element to temporary list, add result to combinatorical list, and backtrack on all possible results for other elements, and then try this again with a new element at idx"
* [90. Subsets II](https://leetcode.com/problems/subsets-ii/description/)
	* Same idea as [78. Subsets], but requires a sorting of the list, and then skipping all the same values in the for loop that are the same as its previous
* [39. Combination Sum](https://leetcode.com/problems/combination-sum/description/)
    * need to iterate over all candidates from \[i, len(nums)\], this is because we are allowed to use the same values, but we do not want all permutations, thus we restrict outselves to the i as our minimum
    * simply just check the new added candidate reaches target or not. if not then perform the backtrack again.
    * every iteration, we want to pop the last element at the end because we want to test out different values.
* [40. Combination Sum II](https://leetcode.com/problems/combination-sum-ii/description/)
    * same idea as [39. Combination Sum], but need to sort the list and skip all adjacent values when comparing the previous iteration.
* [46. Permutations](https://leetcode.com/problems/permutations/description/) $\star$
    * idk why i found this so hard, i guess this is different from the last 3 problems
    * simple backtrack problem where you just check if an element is not in the temp_set, then append it, backtrack on it, and then pop it.
* [17. Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number/description/)
    * simple and same idea as [46. Permutations]
* [79. Word Search](https://leetcode.com/problems/word-search/description/) $\star$ $\star$ 
    * hard problem to conceptualize a more efficient solution. Doesn't work with it tho
    * Just need to iterate over all board positions, and then backtrack on its adjacent positions to check if the position furthers the word_idx
    * I guess this is the first one in the series to use backtracking for an actual return value

* [131. Palindrome Partitioning](https://leetcode.com/problems/palindrome-partitioning/description/) $\star$ $\star$
    * very hard problem for me 
    * palindrome partitoning can be done (expensively) by considering if s[:i] being a palindrome, then backtrack on all other enteries on if s[i:] being
    a palindrome
**Conceptual videos:**
