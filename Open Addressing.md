#DataStructures/Algorithms #HashTables 

Open addressing resolves hash table collisions by seeking out nearby empty cells

# Linear Probing
- on collision, linearly iterate through the table until an open address/cell is found
- O(n) - Linear time complexity
- CONS
	- when clusters form, performance suffers
	- O(n) is acceptable efficiency in many cases, but in large datasets will want a more efficient method
- $(i+1)$
# Quadratic Probing
- on collision, iterate through the table in a quadratic fashion (i^2) to help reduce the likelihood of clusters forming
- can result in an infinite loop, with increased likelihood in smaller datasets
- $(i^2)$

# Double Hashing
- on collision, send the `Key` through a second hash function
- O(1)
```javascript
function hash1(key) {
	return key % table_size;
}

function hash2(key) {
	// prime is a Prime Number
	// prime number must be smaller than table_size, pick any
	return prime - (key % prime)
}

function doubleHash(key) {
	// only call on collision
	return (hash1(key)+i*hash2(key))% table_size
}
```

#DataStructures/Algorithms #HashTables 

Open addressing resolves hash table collisions by seeking out nearby empty cells

# Linear Probing
- on collision, linearly iterate through the table until an open address/cell is found
- O(n) - Linear time complexity
- CONS
	- when clusters form, performance suffers
	- O(n) is acceptable efficiency in many cases, but in large datasets will want a more efficient method
- $(i+1)$
# Quadratic Probing
- on collision, iterate through the table in a quadratic fashion (i^2) to help reduce the likelihood of clusters forming
- can result in an infinite loop, with increased likelihood in smaller datasets
- $(i^2)$

# Double Hashing
- on collision, send the `Key` through a second hash function
- O(1)
```javascript
function hash1(key) {
	return key % table_size;
}

function hash2(key) {
	// prime is a Prime Number
	// prime number must be smaller than table_size, pick any
	return prime - (key % prime)
}

function doubleHash(key) {
	// only call on collision
	return (hash1(key)+i*hash2(key))% table_size
}
```

