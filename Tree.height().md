#DataStructuresAlgorithms #Trees 

```ad-summary
returns the height of the `Tree`. `Height` is the distance from the furthest `child/leaf` to the `root`
```


###### Example:
![Tree-Height_Example](Tree-Height_Example.png)


###### Example Code:
`Tree.height(): integer`

```javascript
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
```

---
Related: [Trees](Trees.md)