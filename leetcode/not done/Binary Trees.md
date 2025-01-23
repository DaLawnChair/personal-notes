 ```python
from collections import deque
class Node:
	def ___init__(self, val=0, left= None, right=None):
		self.val = val
		self.left = left # left pointer
		self.right = right # right pointer

class BinaryTree:
	def ___init__(self, val=0):
		self.head = Node(val)
```

## []
**Lookout for:**

**Idea:**
**Example:**
**Conceptual videos:**

# BFS

## []
**Lookout for:**

**Idea:**
**Example:**
**Conceptual videos:**

# DFS

## []
**Lookout for:**

**Idea:**
**Example:**
* [543. Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree/submissions/1512232232/)
	* Keep a global counter `diameter`. Do DFS on the left and right, make `diameter = max(diameter,left+right)`. Return `max(left,right)+1` for the DFS and then for the caller function return `diameter`

**Conceptual videos:**
# Implementation:
```python
# An Iterative Python program to do DFS traversal from 
# a given source vertex. DFS(int s) traverses vertices 
# reachable from s. 

# This class represents a directed graph using adjacency 
# list representation 
class Graph: 
	def __init__(self,V): # Constructor 
		self.V = V	 # No. of vertices 
		self.adj = [[] for i in range(V)] # adjacency lists 

	def addEdge(self,v, w):	 # to add an edge to graph
		self.adj[v].append(w) # Add w to v’s list. 

	def bfs(self, adj, s):
	    
	    q = deque() # Create a queue for BFS
	    
	    # Initially mark all the vertices as not visited
	    # When we push a vertex into the q, we mark it as 
	    # visited
	    visited = [False] * len(adj);
	
	    # Mark the source node as visited and enqueue it
	    visited[s] = True
	    q.append(s)
	
	    while q: # Iterate over the queue
	      
	        # Dequeue a vertex from queue and print it
	        curr = q.popleft()
	
	        # Get all adjacent vertices of the dequeued 
	        # vertex. If an adjacent has not been visited, 
	        # mark it visited and enqueue it
	        for x in adj[curr]:
	            if not visited[x]:
	                visited[x] = True
	                q.append(x)

	def DFS(self,s):
		# Initially mark all vertices as not visited 
		visited = [False for i in range(self.V)] 

		# Create a stack for DFS 
		stack = []

		# Push the current source node. 
		stack.append(s) 

		while (len(stack)): 
			# Pop a vertex from stack and print it 
			s = stack[-1] 
			stack.pop()

			# Stack may contain same vertex twice. So 
			# we need to print the popped item only 
			# if it is not visited. 
			if (not visited[s]): 
				print(s,end=' ')
				visited[s] = True

			# Get all adjacent vertices of the popped vertex s 
			# If a adjacent has not been visited, then push it 
			# to the stack. 
			for node in self.adj[s]: 
				if (not visited[node]): 
					stack.append(node) 
	


```