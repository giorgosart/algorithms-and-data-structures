# Big O Notation
In computer science, big O notation is used to describe how complex an algorithm can be and how much time it will take to execute based on the worst case scenario.

## O(1) - Constant Time Algorithm
The algorithm will always take the same time to execute no matter how big or complex the dataset is
### Example
``` 
const getFirstItem = list => item[0];

getFirstItem([0, 1, 2]); // will return '0' in the first iteration
getFirstItem([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]); // will return '0' in the first iteration
```
