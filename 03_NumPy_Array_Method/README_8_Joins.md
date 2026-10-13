
# NumPy Joining Array
### Joining NumPy Arrays
Joining means putting contents of two or more arrays in a single array.
In SQL we join tables based on a key, whereas in NumPy we join arrays by axes.
We pass a sequence of arrays that we want to join to the concatenate() function, along with the axis. If axis is not explicitly passed, it is taken as 0.
## Join two arrays
```code
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.concatenate((arr1, arr2))

print(arr)
```
***If forgot 2 brackets, we found error.***

### Join two 2-D arrays along rows (axis=1):
```code
import numpy as np

arr1 = np.array([[1, 2], [3, 4]])

arr2 = np.array([[5, 6], [7, 8]])

arr = np.concatenate((arr1, arr2), axis=1)

print(arr)
```
**Check change axis 0 & 1. This will work on 2-D array**

```Output
Output: with axis=1
[[1 2 5 6]
 [3 4 7 8]]
```
```Output
Output:with axis=0
[[1 2]
 [3 4]
 [5 6]
 [7 8]]
```
## Joining Arrays Using Stack Functions
Stacking is same as concatenation, the only difference is that stacking is done along a new axis.
We can concatenate two 1-D arrays along the second axis which would result in putting them one over the other, ie. stacking.
We pass a sequence of arrays that we want to join to the stack() method along with the axis. If axis is not explicitly passed it is taken as 0.
```code
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.stack((arr1, arr2), axis=1)

print(arr)

```Output
Output:
[42]
0s
[[1 4]
 [2 5]
 [3 6]]
```
**Try this with axis 0 & 1.**


|Stacking Method	|Visual Behavior	|Resulting Array	|Output Shape|
|-------------------------|-------------------------|----------------------------|---------------|
|np.stack((a, b), axis=0)	|Places arrays one below another (as new rows)	|[[1, 2, 3], [4, 5, 6]]	|(2, 3)
|np.stack((a, b), axis=1)	|Pairs matching indices together (as new columns)	|[[1, 4], [2, 5], [3, 6]]	|(3,2)

### Stacking Along Rows
NumPy provides a helper function: hstack() to stack along rows.
```code
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.hstack((arr1, arr2))

print(arr)
```
### Stacking Along Rows (hstack)
NumPy provides a helper function: hstack()  to stack along colums.
```code
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.hstack((arr1, arr2))

print(arr)
```
```Output
Output:
[1 2 3 4 5 6]
```

### Stacking Along Columns (vstack)
NumPy provides a helper function: vstack()  to stack along columns.
```code
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.vstack((arr1, arr2))

print(arr)
```
```Output
Output:
[1 2 3]
[4 5 6]
```
## Stacking Along Height (depth)

NumPy provides a helper function: dstack() to stack along height, which is the same as depth.

```code
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.dstack((arr1, arr2))

print(arr)
```









<br/>
