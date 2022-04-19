#DataStructures/Algorithms #HashTables

Hash Tables are designed to store large amounts of data in an `indexed` way, so that the data can be searched and returned as fast as possible. Hash Tables use a [[Hash Function]] to map unique identifiers `(Keys)` such as: `integers`, `strings`, names, words, `UUIDs`, etc. into an `Array index`, where the `Key/Value pair` is stored. 

- Used to store key/value pairs
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