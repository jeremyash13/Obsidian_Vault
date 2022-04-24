#ComputerScience #DataStructuresAlgorithms #Trees 

```ad-summary
*Depth First Traversal*, is method of traversing a Tree data structure where children nodes, a.k.a. leaves, are read before their parent nodes.
```

## Table Of Contents:
1. [Pre-Order Traversal](#Pre-Order%20Traversal)
2. [In-Order Traversal](#In-Order%20Traversal)
3. [Post-Order Traversal](#Post-Order%20Traversal)

---

# Pre-Order Traversal
From `Top` to `Bottom`, read Tree nodes in the order of: `*Root*, Left, Right`.
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

# In-Order Traversal
From `Bottom` to `Top`, read Tree nodes in the order of: `Left, *Root*, Right`. *Outputs in ascending or descending order.* 

![Tree-Traversal_Depth-First_IN-ODER_Example](Tree-Traversal_Depth-First_IN-ODER_Example.png)
`output: [1, 4, 6, 7, 8, 9, 10]`

Code Example:
```javascript 
// Recursive Solution
class BinaryTree {

//public method
  traverseInOrder() {
   this.#traverseInOrder(this.rootNode);
  }

// private method
  #traverseInOrder(node) {
    if (!node) return;
    
    this.#traverseInOrder(node.leftChild);
    console.log(node.value);
    this.#traverseInOrder(node.rightChild);
  }
}
```


---

# Post-Order Traversal
From `Bottom` to `Top`, read Tree nodes in the order of: `Left, Right, *Root*`. Post-Order traversal is commonly used when node values need to be passed up along the tree for calculations.


![Tree-Traversal_Depth-First_POST-ODER_Example](Tree-Traversal_Depth-First_POST-ODER_Example.png)
`output: [1, 4, 6, 8, 9, 10, 7]`

Code Example:
```javascript 
// Recursive Solution
class BinaryTree {

//public method
  traversePostOrder() {
   this.#traversePostOrder(this.rootNode);
  }

// private method
  #traversePostOrder(node) {
    if (!node) return;
    
    this.#traversePostOrder(node.leftChild);
    console.log(node.value);
    this.#traversePostOrder(node.rightChild);
  }
}
```


---
Related: [Trees](Trees.md), [Tree Traversal (Breadth First)](Tree%20Traversal%20(Breadth%20First).md)