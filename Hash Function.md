#DataStructures/Algorithms #HashTables #ComputerScience

```ad-summary
Used to transform a unique identifier such as UUIDs, large numbers, names, words, etc. to an [Array](Array.md) Index. Usually a `Number` or `String` type.
```


- function must return a valid [Array](Array.md) index
	- must not return values larger than the size of the [Array](Array.md)
	- the `% modulo` operator is used to calculate the divisible remainder
		- this ensures a value within the bounds of the [Array](Array.md)
- the input key must first be converted to a number
	- `Strings` can have the ASCII code of each individual character summed together to achieve this

### Examples:

```javascript
let key = 12345;
let hashIndex = Array(10); // length of 10

function(key) {
	return key % hashIndex.length;
}
```