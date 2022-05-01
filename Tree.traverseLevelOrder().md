#DataStructuresAlgorithms #ComputerScience #Trees 

```ad-summary
Traverses the `Tree` level-by-level, `returning` or `printing` the `nodes` one level at a time.
```


To get the node values one level at a time, first get the `height` of the `tree`, then call `printNodesAtDistance()` at each level (0, 1, 2, ...).


### Example Code:

`Tree.traverseLevelOrder(): Void`
```javascript
traverseLevelOrder() {
    let height = this.height();
    for (let i = 0; i <= height; i++) {
      //   this.printNodesAtDistance(i);
      console.log(this.printNodesAtDistance(i));
    }
}
```
---
Related: [Trees](Trees.md), [Breadth First Level Order](Tree%20Traversal%20(Breadth%20First).md#Breadth%20First%20Level%20Order), [Tree.height()](Tree.height().md), [Tree.printNodesAtDistance()](Tree.printNodesAtDistance().md)