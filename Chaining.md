#DataStructuresAlgorithms #HashTables #ComputerScience

```ad-summary
Chaining is a method of resolving [Hash Table](Hash%20Table.md) collisions that stores overflow data into a [Linked List](Linked%20List.md).
```


Rather than storing the key/value pair directly in the cell provided by the [Hash Function](Hash%20Function.md), instead store a reference to another data structure such as a [Linked List](Linked%20List.md) in the cell, then appending the key/value pair to the [Linked List](Linked%20List.md).


# Example:

![[Hash_Table_Chaining_Example.png]]