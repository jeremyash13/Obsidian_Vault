#ComputerScience 

```ad-summary
Recursion is when a `Function` or `Method` calls itself.
```


## Example:
```javascript 
// factorial 4 = 4 x 3 x 2 x 1

function factorial(n) {
	// Base condition to end the recursive loop
	if (n === 1) return 1;
	
	return n * factorial(n - 1);
}
```

---
Related:  