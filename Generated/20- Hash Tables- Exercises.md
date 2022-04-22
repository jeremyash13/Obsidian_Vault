
Source: [[PDFs/20- Hash Tables- Exercises.pdf]]





---
## Page 1

# Hash Tables

## Exercises 

1Find the most repeated element in an array of integers. What is the 

time complexity of this method? (A variation of this exercise is finding 

the most repeated word in a sentence. The algorithm is the same. Here 

we use an array of numbers for simplicity.)  

Input: [1, 2, 2, 3, 3, 3, 4] 

Output: 3 

**Solution: HashTableExercises.mostFrequent()** 

2Given an array of integers, count the number of **unique** pairs of 

integers that have difference k.  

Input: [1, 7, 5, 9, 2, 12, 3] K=2 

Output: 4 

We have four pairs with difference 2: (1, 3), (3, 5), (5, 7), (7, 9). Note 

that we only want the number of these pairs, not the pairs themselves.  

**Solution: HashTableExercises.countPairsWithDiff()** 

3Given an array of integers, return **indices** of the two numbers such 

that they add up to a specific target.



---
## Page 2

Input: [2, 7, 11, 15] - target = 9

Output: [0, 1] (because 2 + 7 = 9)

Assume that each input has **exactly** one solution, and you may not use 

the 

*same* element twice. 

**Solution: HashTableExercises.twoSum()** 

4Build a hash table from scratch. Use linear probing strategy for 

handling collisions. Implement the following operations:  

-

put(int, String) 

-

get(int) 

-

remove(int) 
-

size() 

Solution: **HashMap** 

---
## Footnotes