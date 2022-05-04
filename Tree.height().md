#DataStructuresAlgorithms #Trees 

```ad-summary
returns the height of a `node`. `Height` is the distance from the furthest `child/leaf` to a given `node` (counted starting from the bottom-most node). Runs in [O(n) - Linear Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20n%20-%20Linear%20Time)

`Height` is the inverse of `Depth`.
```


## Example:
![Tree-Height_Example](Tree-Height_Example.png)
															`Binary Tree`


### Example Code:
`Tree.height(): integer`

```javascript
// Recursive Solution
class BinaryTree {

	// public method
	getHeight() {
	   console.log(this.#getHeight(this.rootNode));
	}

	// private method
	#getHeight(node) {
	   if (!this.rootNode) return -1;
	   if (node.leftChild === null && node.rightChild === null)
	   return 0;
	    
	   let left = this.#getHeight(node.leftChild);
	   let right = this.#getHeight(node.rightChild);
	
	   return 1 + Math.max(left, right);
	}
}
```

---
Related: [Trees](Trees.md), [Tree.printNodesAtDistance()](Tree.printNodesAtDistance().md), [Tree.traverseLevelOrder()](Tree.traverseLevelOrder().md)