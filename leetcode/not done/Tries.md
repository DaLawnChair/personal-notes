**Idea:**
* This is a tree structure designed for searching for sequentially organized datatypes like strings or permutations
 usually fairly expensive to implement, but bitwise representation and other optimizations help it
* radix tree is a good optimization of the trie
* **properties**
	 * the parent node represents the prefix for its children
	* root is the empty string
	* nodes in the trie do not store assocated values, instead the position represents the key of a character inside of the string.
	* null links in the tree implies 
		* that the characters and string keys are stored in the trie
		* each node contains one possible link to a prefix of strong keys of the set
* **Implementaitons**
	* The actual implementation and operations are much like that of an n-ary tree
	* the difference usually here is that insertion can add more than one node to the trie and you can safely iterate over the characeter's length
	* trie-delete is interesting as it recursively removes 
```
Trie-Delete(x, key)

	// recursie removal of the key
    if x = nil then
        return nil
    else if key = "" then
        x.Value := nil
    else
        x.Children[key[0]] := Trie-Delete(x.Children[key[0]], key[1:])
    end if
    // there still lies element in the trie
    if x.Value != nil then
        return x
    end if
    // keeps structure of the remaining elements
    for 0 ≤ i < x.Children.length do
        if x.Children[i] != nil then
            return x
        end if
    repeat
    return nil	  
```

* **Usage**
	* autocomplete
	* spell checking
	* ip routing
* Can be better than hash tables in given curcumstances because 
	* they do not have hash collisions
	* is prefix-orangized
	* keys can be sorted lexographically
* **implementation strategies**
	* standard approach: using a vector/linked list to store these. Alternatively we can store a vector of 256 pointers as a bitmap representaiton of 256 bits needed to represent the ASCII characters, which reduces the size of individual nodes 
	* bitwise tries: each character in the string is represented as individual bits. Is cache-local and paralleziable, so good for out-of-order execution on cpi
	* radix/compression tree: space optimized variant of trie where nodes with 1 child gets merged with the parent.
	* patricia trees: implementation of compression tree with binary encoding, where the nodes has a index (called a skip number) that stores the node's branching index to avoid empty subtree traversal. This skip number is used for all the basic functions, and a bitmask is performed every iteration
	

**Lookout for:**

**Example:**
* [Design Add and Search Word Data Structure](https://neetcode.io/problems/design-word-search-data-structure/question?list=neetcode150)  $\star$ $\star$
	* Problem is hard because the solution is a brute force 
	* Fuzzy searching is a hard concept, but this is only being done in the 1 match case
		* consider all characters in the word
		* if we have a mismatched character, then iterate over all of our child nodes to and see if it can be found within our children's search, if so return True, otherwise continue.
		* If it cannot be found then return False
* 
**Conceptual videos:**