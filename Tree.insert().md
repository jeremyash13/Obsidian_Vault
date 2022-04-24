#DataStructuresAlgorithms #Trees 

```ad-summary
inserts a new `node` into the `Tree`. in `BinaryTrees`, sorting occurs at the time of inserting a new `node`.
```


## Example Code:
`Tree.insert(value: any): integer`

```javascript 
class BinaryTree {
   insert(v) {
    let newNode = new Node(v);
    if (this.rootNode === null) {
      this.rootNode = newNode;
      return;
   }
  
    let current = this.rootNode;

    while (true) {
      if (v < current.value) {
        // traversing left side
        if (current.leftChild === null) {
	    // reached parent. node needs to be inserted to the 
		// left of current
        current.leftChild = newNode; // appending new node to  
        // its parent
          break;
        } else {
          current = current.leftChild;
        }
      }
      
      if (v > current.value) {
        // traversing right side
        if (current.rightChild === null) {
          // reached parent. node needs to be inserted to the    
          // right of current
          current.rightChild = newNode; // appending new node to 
          // its parent
          break;
        } else {
          current = current.rightChild;
        }
      }
    }
  }
}
```


---
Related: [Trees](Trees.md)