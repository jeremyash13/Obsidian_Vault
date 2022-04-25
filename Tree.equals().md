#DataStructuresAlgorithms #Trees 

```ad-summary
Compares two `Trees` and returns `True` or `False` if the two `Trees` are identical.
```


### Example Code:
`Tree.equals(tree2: Tree): boolean`

```javascript 
// Recursive Solution

class BinaryTree {

	// public method
	equals(tree) {
		if (!tree) return false;
		return this.#equals(this.rootNode, tree.rootNode);
	}
	
	// private method
	#equals(node1, node2) {
		if (!node1 && !node2) return true;
		if (node1 && node2)
			return (
				node1.value === node2.value &&
				this.#equals(node1.leftChild, node2.leftChild) &&
				this.#equals(node1.rightChild, node2.rightChild)
			);
		return false;
  }
}
```


---
Related: [Trees](Trees.md)