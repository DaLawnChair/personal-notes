# []
**Lookout for:**

**Idea:**
**Example:**
* [Insert Interval](https://leetcode.com/problems/insert-interval/) $\star$ $\start$
    * since the arrays are sorted, we can use a binary search to find the position of the newInterval. This position I elect is the furthers position where all intervals before it 
    are not within its newInterval's range.
    * all these values before this position will not merge, so we can add these to the intervals into the return list
    * loop overall other and check that they lie within the the new interval, merging as we go by taking the min of both starts and max of both ends
    * after we can add this and then all other remaining intervals into the return list

**Conceptual videos:**
