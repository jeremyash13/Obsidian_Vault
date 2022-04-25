#DataStructuresAlgorithms #Trees 

```ad-summary
The *Binary Tree* solution compares both left and right `child nodes,` and returns the minimum value. Runs in [O(n) - Linear Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20n%20-%20Linear%20Time)

The *Binary Search Tree* only needs to return the left most `value` since values are sorted. Runs in [O(log n) - Logarithmic Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%20log%20n%20-%20Logarithmic%20Time)
```


## Example Code:
`Tree.min(): integer`

													Binary Tree solution:
```javascript
// Recursive Solution
class BinaryTree {

	// public method
	min() {
		this.#min(this.rootNode);
	}
	
	// private method
	#min(node) {
	    if (!node) return Number.MAX_SAFE_INTEGER; // 
	    
	    let left = this.#min(node.leftChild);
	    let right = this.#min(node.rightChild);
	    
	    return Math.min(left, right, node.value);
	}
}
```


												Binary Search Tree solution:
```javascript
// Recursive Solution
class BinaryTree {

	// public method
	min() {
		this.#min(this.rootNode);
	}
	
	// private method
	#min(node) {
	    if (!node) return Number.MAX_SAFE_INTEGER;
	    
	    let left = this.#min(node.leftChild);
	    
	    return Math.min(left, node.value);
	}
}
```


---
Related: [Trees](Trees.md)