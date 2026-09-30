# leetcode-DSA


# Todo:
* Fill in intuition of Manacher's Algorithm inside of [Palindromes.md]
* Horare's selection algorithm, an approach to "find kth something" problems
    * O(n) average time complexity, with worse case O(n^2)
    * essentialyl a quicksort adoptation for these types of questions
    1. build hashmap of {element: frequency}  
    2. choose random pivot and put it in its place ina s orted array, items on left are less frequent, right are more or same frequency 
    3. pivot is nth less frequent element, return right part of array
# Focus on:

Arrays:
* https://leetcode.com/problems/top-k-frequent-elements/
    * solution is currently slow, should be O(nlogn) but is slow
        -- actually solutions to this are super weird, not sure worth it to look into, refer to Horare's algorithm above

try to code up this problem:
https://leetcode.com/problems/trapping-rain-water-ii/
