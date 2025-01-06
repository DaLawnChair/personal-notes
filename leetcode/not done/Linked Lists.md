# Linked Lists
## Singly Linked List
**Idea:**
* Can store values as nodes connected with each other
```python
class SinglyLinkedListNode:
	def __init__(self, val=0, next=None):
		self.val = val
		self.next = next
		
class DoublyLinkedListNode:
	def __init__(self, val=0, prev = None, next=None):
		self.val = val
		self.next = next
		self.prev = prev
```

**General time complexity:**

| Action                                | Time complexity | Space complexity |
| ------------------------------------- | --------------- | ---------------- |
| Max                                   | O(n)            | O(1)             |
| Insertion at beginning                | O(1)            | O(1)             |
| Insertion at end (no tail/ with tail) | O(n)/O(1)       | O(1)             |
| Insertion inbetween                   | O(n)            | O(1)             |

### Algorithms
* Lead Lag:
	* Set up 2 pointers of X distant a part
**Example:**
* Singly Linked lists:
	* [143. Reorder List](https://leetcode.com/problems/reorder-list/)
	* [19. Remove Nth Node From End of List](https://leetcode.com/problems/remove-nth-node-from-end-of-list/)
	* 
* Doubly linked list: 
	* [146. LRU Cache](https://leetcode.com/problems/lru-cache/submissions/1489285593/)
	* [138. Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer/)
	* 

* Fast and slow pointers solvable:
	* [287. Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/) Super hard, has 7 ways to solve, classic
**Conceptual videos:**
[][]

# Fast-Slow:

**Lookout for:**
* Useful for getting fractional part of the linked list with the fast pointer going to end quicker, thus by the time the while loop ends, the slow pointer is halfway through the linked list
**Lookout for:**
* Look for values  
**Idea:**
* Set up 2 pointers in the same location, but one moves twice as fast as the other
```python
def fastSlow(self. head):
	slow = head
	fast = head
	while fast and fast.next:
		fast = fast.next.next
		slow = slow.next
```

**Example:**
* [141. Linked List Cycle](https://leetcode.com/problems/linked-list-cycle/)
	* Set 1 pointer to move twice as fast as the other, if faster pointer terminates to None, then no cycle, otherwise there is a cycle
* [287. Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/)
	* Because the values are within the size of the array, we can actually loop through the values inside the array without sequential iteration.
**Conceptual videos:**
[][]