#DataStructuresAlgorithms #ComputerScience

```ad-summary
Time and Space Complexity is a method of measuring how an algorithm's run time (Time) and memory requirements (Space) grow in relation to the size of the `Input`.

Big-O-Notation is a method of representing this relationship mathmatically.
```


Time complexity and space complexity usually have a ***trade-off-type-relationship***. In other words, by increasing the amount of memory your algorithm uses, you can increase the run-time-efficiency, and vice-versa.


## O(1) - Constant Time
- has the same run time no matter the `input` size
- ideal efficiency

## O(log n) - Logarithmic Time
- deals with large `inputs` very efficiently, due to the `input` halving on each iteration
- requires a sorted data set

## O(n) - Linear Time
- run time scales in a 1:1 ratio with the `input` size.

## O(n^2) - Quadratic Time
- run time grows at the rate of $n^2$
- very poor efficiency

## O(2^n) - Exponential Time
- run time grows at the rate of $2^n$
- very poor efficiency
- nested loops are most likely the culprit of exponential run-time

![[Time+Space_Complexity_Cheatsheet.png]]