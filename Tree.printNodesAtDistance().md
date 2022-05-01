#DataStructuresAlgorithms #ComputerScience #Trees 

```ad-summary
`Prints` or `returns` all `nodes` at the given distance away from `root`.
```

### Example Code:

`Tree.printNodesAtDistance(distance: Integer): Array`
```javascript
// Recursive Solution

// public method
printNodesAtDistance(distance) {
	let nodesArr = []; // transfer to recursive func via dependency 
					   // injection
					   
    this.#printNodesAtDistance(this.rootNode, distance, nodesArr);
    return nodesArr;
}

// private method
#printNodesAtDistance(currentNode, distance, nodesArr) {
    if (!currentNode) {
      // blank/null node found (reached end of the tree)
      return;
    }
    if (distance === 0) {
	  nodesArr.push(currentNode.value);
      return;
    }
    this.#printNodesAtDistance(currentNode.leftChild, distance - 1);
    this.#printNodesAtDistance(currentNode.rightChild, distance - 1);
}
```

---
Related: [Trees](Trees.md), [Tree.height()](Tree.height().md), [Tree.traverseLevelOrder()](Tree.traverseLevelOrder().md)