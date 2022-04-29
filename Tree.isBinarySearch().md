#DataStructuresAlgorithms #ComputerScience #Trees 

```ad-summary
Determines if the `Tree` is a *Binary Search Tree* or not.
```


### Example Code:
`Tree.isBinarySearch(): boolean`

```javascript
// Recursive Solution

// public method
isBinarySearch() {
	this.#isBinarySearch(this.rootNode, 0, Number.MAX_SAFE_INTEGER);
}

// private method
#isBinarySearch(currentNode, min, max) {
    if (!currentNode) {
      return true;
    }

    if (currentNode.value < min || currentNode.value > max) {
      return false;
    }

    // on left traversal, update MAX
    // on right traversal, update MIN
    return (
      this.#isBinarySearch(currentNode.leftChild, min, currentNode.value) &&
      this.#isBinarySearch(currentNode.rightChild, currentNode.value, max)
    );
}
```
---
Related:  [Trees](Trees.md)