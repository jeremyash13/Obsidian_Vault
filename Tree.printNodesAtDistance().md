#DataStructuresAlgorithms #ComputerScience #Trees 

```ad-summary
`Prints` or `returns` all `nodes` at the given distance away from another `node`.
```

### Example Code:

`Tree.printNodesAtDistance(node: Node, distance: Integer): Array`
```javascript
// Recursive Method

// public method
printNodesAtDistance(distance) {
    this.#printNodesAtDistance(this.rootNode, distance);
}

// private method
#printNodesAtDistance(currentNode, distance) {
    if (!currentNode) {
      return;
    }
    if (distance === 0) {
      console.log(currentNode.value);
      return;
    }
    this.#printNodesAtDistance(currentNode.leftChild, distance - 1);
    this.#printNodesAtDistance(currentNode.rightChild, distance - 1);
}
```
---
Related: [Trees](Trees.md)