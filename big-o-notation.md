# Big O Notation
In computer science, big O notation is used to describe how complex an algorithm can be and how much time it will take to execute based on the worst case scenario.

## O(![1](https://latex.codecogs.com/gif.latex?1)) - Constant Time Algorithm
The algorithm will always take the same time to execute no matter how big or complex the input data set is.
### Example
``` 
const getFirstItem = list => list[0];

getFirstItem([0, 1, 2]); // will return '0' in the 1st iteration
getFirstItem([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]); // will return '0' in the 1st iteration
```

## O(![n](https://latex.codecogs.com/gif.latex?n)) - Linear Time Algorithm
The algorithm's execution time will grow based on the size of the input data set. Worst case scenario would be the size of the data set.
### Example
``` 
const matchMe = (list, text) => {
  list.forEach((item) => {
    if(item === text){
      return true;
    }
  });
};

matchMe([0, 1, 2], 2); // will return '2' in the 3rd iteration
matchMe([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 10); // will return '10' in the 11th iteration
```

## O(![n^2](https://latex.codecogs.com/gif.latex?n^{2})) - Quadratic Time Algorithm
The algorithm's execution time will grow exponentially based on the size of the input data set. Worst case scenarion would be input data set size squared.
### Example
``` 
const matchMe = (listA, listB) => {
  listA.forEach((itemA) => {
    listB.forEach((itemB) => {
      if(itemA === itemB){
        return true;
      }
    })
  });
};

matchMe([0, 1, 2], [5, 4, 3, 2]); // will return 'true' in the 12th iteration
matchMe([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], [12, 11 ,10]); // will return '0' in the 33rd iteration```

