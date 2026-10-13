# NumPy Array Iteration
### Iterating Arrays
Iterating means going through elements one by one.
As we deal with multi-dimensional arrays in numpy, we can do this using basic for loop of python.
If we iterate on a 1-D array it will go through each element one by one.

## Iterating 1-D array
Iterate on the elements of the following 1-D array:
```code
import numpy as np

arr = np.array([1, 2, 3])

for x in arr:
  print(x)
```

## Iterating 2-D array
In a 2-D array it will go through all the rows.

```code
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

for x in arr:
  print(x)
```
***If we iterate on a n-D array it will go through n-1th dimension one by one.***

## Iterating 2D array in each element
```code
Import numpy as np
Arr=np.array([[1,2,3,4],[5,6,7,8]])
For x in arr:
    For y in x:
        Print(y)
```
```Output: 1 2 3 4 5 6 7 8```

## Iterating 3-D Arrays
In a 3-D array it will go through all the 2-D arrays.

Iterate on the elements of the following 3-D array:
```code
Import numpy as np
Arr=np.array([[1,2,3],[4,5,6],[7,8,9]])
For x in arr:
    Print(x)
```
```Output: [1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]```

**To return the actual values, the scalars, we have to iterate the arrays in each dimension.**
```code
Import numpy as np
arr=np.array([[[1,2,3],[4,5,6]],[[7,8,9],[10,11,12]]])
For x in arr:
  For y in x:
      For z in y:
        Print(y)
```
```Output: 1 2 3 4 5 6```
## We can do this same operation with nditer() method.
The function nditer() is a helping function that can be used from very basic to very advanced iterations. It solves some basic issues which we face in iteration.
### Iterating on Each Scalar Element
In basic for loops, iterating through each scalar of an array we need to use n for loops which can be difficult to write for arrays with very high dimensionality.
**Iterate through the following 3-D array:**
```code
import numpy as np
arr=np.array([[[1,2,3],[4,5,6]],[[7,8,9],[10,11,12]]])
for x in np.nditer(arr):
  print(x)
```

## iterating with different datatypes
```Still pending from w3schools.```
## Iterating With Different Step Size
```Still pending from w3schools.```
## Enumerated Iteration Using ndenumerate()
Enumeration means mentioning sequence number of somethings one by one.
Sometimes we require corresponding index of the element while iterating, the ndenumerate() method can be used for those usecases.

Enumerate on following 1D arrays elements
```code
import numpy as np

arr = np.array([1, 2, 3])

for idx, x in np.ndenumerate(arr):
  print(idx, x)
```
```Output
Output:
(0,) 1
(1,) 2
(2,) 3
```
### Enumerate with 2-D

```code
import numpy as np
arr=np.array([[[1,2,3],[4,5,6]],[[7,8,9],[10,11,12]]])
for id, x in np.ndenumerate(arr):
  print(id,x)

```
```Output
Output
(0, 0, 0) 1
(0, 0, 1) 2
(0, 0, 2) 3
(0, 1, 0) 4
(0, 1, 1) 5
(0, 1, 2) 6
(1, 0, 0) 7
(1, 0, 1) 8
(1, 0, 2) 9
(1, 1, 0) 10
(1, 1, 1) 11
(1, 1, 2) 12
```
## Quiz
### Quiz 1
```code
import numpy as np
arr = np.array(['a', 'b', 'c'])
for x in arr:
  print('Hello ' + x)
```
```Output
Output:
Hello a
Hello b
Hello c
```


