#DataStructures/Algorithms #Trees

```ad-summary
A Binary Tree is a data structure designed for representing hierarchical data. Binary Trees are sorted alphanumerically so they can be traversed using a Binary Search algorithm, also known as Divide and Conquer.
```


- Each node can have a max of 2 children/leaves
- The left child node is always a lower value than its parent node
- The right child node is always a greater value than its parent node
		*left child < node < right child*
- Lookup(x) [O (log n) - Logarithmic Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20log%20n%20-%20Logarithmic%20Time)
- Insert(x) [O (log n) - Logarithmic Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20log%20n%20-%20Logarithmic%20Time)
- Delete(x) [O (log n) - Logarithmic Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20log%20n%20-%20Logarithmic%20Time)
- Poorly structured trees can see their performance decrease to [O(n) - Linear Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20n%20-%20Linear%20Time)


## Exercises
- [ ] Implement a method to calculate the size of a binary tree. `Tree.size()`
- [ ] Implement a method to count the number of leaves in a binary tree. `Tree.countLeaves`
- [ ] Implement a method to return the maximum value in a binary search tree using recursion. `Tree.max()`
- [ ]  Implement a method to check for the existence of a value in a binary tree using recursion. Compare this method with the `find()` method. The `find()` method does the same job using iteration. `Tree.contains()`
- [ ] Implement a method to check to see if two values are siblings in a binary tree. `Tree.areSibling()`
- [ ] Implement a method to return the ancestors of a value in a `List<Integer>`. `Tree.getAncestors()`