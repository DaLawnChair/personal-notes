## []
**Lookout for:**
* Getting the K-th last item from a list/operation
* Task selection with delay 

**Idea:**
* With the items, the ordering you need is represented by the max item at a given time, and thus you do not need a fully sorted list, you just need the next largert/smallest item.
* In cpp, `priority_queue<int, vector<int>, greater<int>>` represents the minHeap, will changing greater to less uses a max heap
* 
**Example:**
* [612. Task Scheduler](https://leetcode.com/problems/task-scheduler/submissions/) $\star$
	* Define a heap based on the count of the task, and then a jail as a queue that will hold items while they wait for them to be able to be ran again
	* 
**Conceptual videos:**