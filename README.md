# Data Structures and Algorithms

1. Fork and clone this repo
2. Fill out the Big O and Written Questions in this README.
3. Complete the HackerRank challenges on hackerrank.com
4. You have 1 hour and 20 minutes


### Big O Analysis

---
Function 1 Time Complexity:

Explain your answer:
```
function bobIsFirst(people){
  return people[0] == 'bob'
}
```

# This is constant time complexity as the time required to run is the same in each instance.
Three seperate operations
1. Looking up bobIsFirst 0(1)
2. Assigning bobIsFirst  to the variable [0] 0(1)
3. returning that variable 0(1)
# 0(1+1+1) = 0(3) or 0(3x1) simplified 0(1)

Big O notation is the most common metric for calculating time complexity. It describes the execution time of a task in relation to the number of steps required to complete it. ... A task can be handled using one of many algorithms, each of varying complexity and scalability over time.
---
Function 2 Time Complexity:

Explain your answer:
```
function wordOccurrence(word, phrase){
  let result = 0
  const array = phrase.split(' ')
  for(let i = 0; i < array.length; i++){
    if(word.toLowerCase() === array[i].toLowerCase()){
      result++;
    }
  }
  return result
}
```
# 0(n)
# This is 'linear time complexity' as it is unclear whether this is running once or a quadrillion times

---
Function 3 Time Complexity:

Explain your answer:
```
function sort(list){
  for(let i = 0; i < list.length - 1; i++){
    for(let j  = 0; j < list.length - 2; j++){
      if(list[j+1] < list[j]){
        const temp = list[j];
        list[j] = list[j+1];
        list[j+1] = temp;
      }
    }
  }
  return list;
}
```
#  0(n²)
# this is 'quadratic time complexity' as the algorithm will have to run a linear time operation for each value

---

### Written Questions

- What method would you use to look up a word in a dictionary (book, not Python)?

# linear

- Imagine you have a closet full of shirts. What can you do to organize your shirts for easy retrieval?

# organize the by color, style(checked, striped), and sleeve length


- Describe advantages and disadvantages of the most popular sorting algorithms.

# Ireally don't know enough on the subject to give a substantive answer on comparisons and contrasts. I think I may have missed that day with a bad case of brew inflicted postgres monodb-itis.

---

### HackerRank Problems

- [Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem) (Algorithm, Warmup)
- [Left Rotation](https://www.hackerrank.com/challenges/array-left-rotation/problem) (Data Structures, Array)
- [Get Node Value](https://www.hackerrank.com/challenges/get-the-value-of-the-node-at-a-specific-position-from-the-tail) (Data Structures, Linked List)
