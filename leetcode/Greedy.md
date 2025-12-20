Greedy algorithms are algorithms that aim to find an optimal solution by sequential traversal and finding the best choice up to a given point, treating that as the method to which will give the solution

**Lookout for:**
* Is there an enherent ordering to the original information? Ie can it be sorted?
* What is the relationship between solutions at index i vs i-1?
	* If it is completely dependent on i-1, then how can you find i-2?
	* Build a relationship between them
* 
**Idea:**
* Guidelines for solving:
	* Sort the objects by some criterion
	* Repeatidy select the ext item under constraints until no more selections can be made
* **Be very careful on picking your criterion, and make sure that it is able to be proved before proceeding to the algorithm coding**
* The concept is that the local optimum will lead to the global optimum
* Theory works by induction:
	* Base case, inductive hypothesis, inductive step
* Requires 2 proofs:
	* Inductive proof that the algorithm is optimal after the first choice
		* Proof by induction, where we want to prove that after the first choice, the remainder of the solution is optimal
		* Rationally if the first choice is optimal, and there are k+1 enteries total, then the problem reduces to k enteries, and thus the inductive hypothesis is applied
	* The solution found starts with the same choice as the optimal one:
		* Consider how do you find the best first choice
		*  Consider that the optimal choice is O={o1,o2,o3,...,on}
		* As the solution is greedy, a1 is the best possible choice at the start. Thus a1\<o1
		* So O*={a1,o2,...,on} is optimal and the size of |O*|=|O|
		* By our greedy algorithm (proved by induction), the remainder of the solution {a2,a3,...,an} to the reduced problem after a1. Thus {a2,a3,...,an}<={o2,o3...,on}
		* Thus the solution of A <= O.
		* Therefore A is optimal
	* Optionally you can replace the proof by induction with a proof by contradiction
		* Assume that the algorithm is not optimal, then prove that it is


## Kadane's Algorithm
A simple algorithm for calcuating the maximum sum of an array in O(n) time an O(1) space:
```python
  
def max_subarray(numbers):
    """Find the largest sum of any contiguous subarray."""
    best_sum = float('-inf')
    current_sum = 0
    for x in numbers:
        current_sum = max(x, current_sum + x)
        best_sum = max(best_sum, current_sum)
    return best_sum
```
note this doesn't work for empty subarrays, where it should be `best_sum=0` and `current_sum=max(0,current_sum+x)`
A fair amount of "fake" DP problems, ie problems that are solvable as such, but do not have memoization or the same concept that yields a good solution.
This is also a dp problem


**Example:**
* [45. Jump Game II](https://leetcode.com/problems/jump-game-ii/description/) $\star \star \star$
	* Works by iterating over the entire list, checking for the largest jump possible using 2 pointers, largestJump for the largest jump possible from a previous position, and curr_end, the ending for that largest jump
* [55. Jump Game](https://leetcode.com/problems/jump-game/description/)
	* work backwards, think of getting from the end to the beginning. If we can go from currPos from lowerPos+nums[lowerPos], then can then solve for the sub problem of getting to lowerPos in the first place
	* Has a much more eligant solution where you consider the local max jump you can make, and while iterating from the start to the local max distance, checking if you have over shot or at at the end already
* [846. Hand of Straights](https://leetcode.com/problems/hand-of-straights/description/) $\star \star$
	* can do it by sorting and then iterating over every group, skipping duplicate values,
	* but a much better way is...
	* just use a Counter for all cards, and then for every card, find the lowest card in that it is consecutive to. This will be the start of the consecutive streak.
	* Then while this start is lower than the inital card you got, you check the items in the group size and validate the next consecutive card exists and that there are enough of it.
		* Do so for all cards 
	* This leads to a O(n) solution in both time and space complexity.

* Platform Assigment (cisc365)
	* Sorting based on arrival time, you can select d # of trains to be parked at once, once a new train arrives and the d slots are filled, then you add in d+1 slots.
	* Optimal as if there are d conflicts with the train, then you need d+1 slots. Thus the algorithm is optimal!

**Conceptual videos:**
* https://www.youtube.com/watch?v=pVA8OcW4RJ8
	* Solves the [Darius Wisdom problem](https://codeforces.com/problemset/problem/2034/D) where you can solve it by defining regions of where 0, 1, and 2 should lie in. You can then define a 2D array where the row defines the value and the column defines the region it lies in, and each entry is a list of indicies that lie there.
	* The solution is quite simple, ensure that each value lies in its correct region, and so you deal with values of 2 in the wrong region and move them over by swapping, and then you deal with values of 1 in the wrong region
	* basically just need to do a bunch of swaps between positions, so the time complexity ends up being O(n)
	* 