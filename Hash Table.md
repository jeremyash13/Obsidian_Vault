#DataStructuresAlgorithms #HashTables #ComputerScience

```ad-summary
Hash Tables are a data structure designed for storing key/value pairs in a way where data is indexed, so it can be retrieved without having to search the data structure.
```


Hash Tables are designed to store large amounts of data in an `indexed` fashion, so that the data can be retrieved as fast as possible. Hash Tables use a [Hashing Function](Hash%20Function.md) to map unique identifiers `(Keys)` such as: `integers`, `strings`, names, words, `UUIDs`, etc. into an `Array index`, where the `key/value pair` is stored. 

- Used to store key/value pairs
	- keys must be `unique`
- [Hash Function](Hash%20Function.md)
- Collisions
	- [Chaining](Chaining.md)
	- [Open Addressing](Open%20Addressing.md)

# Operations and [[Time Complexity - Big O Notation]]

- Insert(x) [O(1) - Constant Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%201%20-%20Constant%20Time)
- Remove(x) [O(1) - Constant Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%201%20-%20Constant%20Time)
- Lookup(x) [O(1) - Constant Time](Time%20Complexity%20-%20Big%20O%20Notation.md#O%201%20-%20Constant%20Time)

### Example:
![[Hash_Table_Example.png]]