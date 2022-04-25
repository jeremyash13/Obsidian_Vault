#DataStructuresAlgorithms #Trees 

```ad-summary
Returns `True` or `False` if a given value exists in the `Tree`
```


### Example Code:
`Tree.find(value: any): boolean`

```javascript 
// Iterative Solution

class BinaryTree {

  find(v) {
     let current = this.rootNode;
     while (current != null) {
     // only run if the Tree has atleast 1 Node/entry
      if (v === current.value) {
       //   value found in current node
       return true;
      }
      
      if (v < current.value) {
        //   traverse left side tree
        current = current.leftChild;
      } else if (v > current.value) {
        //   traverse right side tree
        current = current.rightChild;
      }
    }
    
    // current is null, value doesnt exist.
    return false;
  }
}
```


---
Related: [Trees](Trees.md)