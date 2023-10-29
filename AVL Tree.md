#DataStructuresAlgorithms #Trees #ComputerScience

```ad-summary
AVL Trees are a type of **self-balancing** *binary search tree.* Named after its investors (Adelson-Velsky and Landis)
```


Tree balancing is essential to maintain `lookUp(x)` performance. An unbalanced tree will degrade from [O(log n) - Logarithmic Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20log%20n%20-%20Logarithmic%20Time) to [O(n) - Linear Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20n%20-%20Linear%20Time) (worst case scenario) when searching for values.

An  unbalanced `tree` is where the `height` difference between the `left child` and `right child` is greater than 1.   $height(left) - height(right) > 1$


### Example: 
![Unbalanced-Tree_Example](Unbalanced-Tree_Example.png)


---
Related: [Trees](Trees.md), [Binary Search Tree](Binary%20Search%20Tree.md)