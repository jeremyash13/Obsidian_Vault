#ComputerScience #DataStructures/Algorithms #Trees 

```ad-summary
*Depth First Traversal*, is method of traversing a Tree data structure where children nodes, a.k.a. leaves, are read before their parent nodes.
```


##### Pre-Order Traversal
Tree is traversed and read in the order of: `*Root*, Left, Right`.
Print `Root` nodes, followed by `Left` children nodes, and finally `Right` children nodes.

![Tree-Traversal__Depth-First__PRE-ODER__Example](Tree-Traversal_Depth-First_PRE-ODER_Example.png)
`output: [7, 4, 1, 6, 9, 8, 10]`

Code Example:
```javascript 
// Recursive Solution
class BinaryTree {

//public method
  traversePreOrder() {
   this.#traversePreOrder(this.rootNode);
  }

// private method
  #traversePreOrder(node) {
    if (!node) return;
    
    console.log(node.value);
    this.#traversePreOrder(node.leftChild);
    this.#traversePreOrder(node.rightChild);
  }
}
```

---

##### In-Order Traversal
Tree is traversed and read in the order of: `Left, *Root*, Right`. *Outputs in ascending or descending order.* Print 

![Tree-Traversal_Depth-First_IN-ODER_Example](Tree-Traversal_Depth-First_IN-ODER_Example.png)
`output: [1, 4, 6, 7, 8, 9, 10]`

---

##### Post-Order Traversal
Tree is traversed and read in the order of: `Left, Right, *Root*`. Post-Order traversal is commonly used when node values need to be passed up along the tree for calculations.


![Tree-Traversal_Depth-First_POST-ODER_Example](Tree-Traversal_Depth-First_POST-ODER_Example.png)
`output: [1, 4, 6, 8, 9, 10, 7]`


---
Related: [Trees](Trees.md), [Tree Traversal (Breadth First)](Tree%20Traversal%20(Breadth%20First).md)