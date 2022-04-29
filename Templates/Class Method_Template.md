tags

```ad-summary
Summary goes here.
```

### Example Code:

```javascript
// public method
isBinarySearch() {
	this.#validate(this.rootNode, 0, Number.MAX_SAFE_INTEGER);
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
      this.#validate(currentNode.leftChild, min, currentNode.value) &&
      this.#validate(currentNode.rightChild, currentNode.value, max)
    );
}
```
---
Related: 