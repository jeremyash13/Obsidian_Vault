#DataStructures/Algorithms #HashTables 

- used to transform a unique identifier such as a UUIDs, large numbers, or names/words to an `Array Index`. Usually a `Number` or `String` type.

- function must return a valid `Array` index
	- must not return values larger than the size of the `Array`
	- the `% modulo` operator is used to calculate the divisible remainder
		- this ensures a value within the bounds of the `Array`
- the input key must first be converted to a number
	- `Strings` can have the ASCII code of each individual character summed together to achieve this

```javascript
let key = 12345;
let hashIndex = Array(10); // length of 10

function(key) {
	return key % hashIndex.length;
}
```