
# Dimensions in Arrays

A dimension in arrays is one level of array depth (nested arrays).

```nested array: are arrays that have arrays as their elements.```

### 0-D Array

```
import numpy as np

arr = np.array(42)

print(arr)
```

This have only 42, which is 0 dimensional. 

### 1-D Array

```
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
```

```Create a 1-D array containing the values 1,2,3,4,5:```

### 2-D Array

An array that has 1-D arrays as its elements is called a 2-D array.

```
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

print(arr)
```

```Create a 2-D array containing two arrays with the values 1,2,3 and 4,5,6```

### 3-D Array

An array that has 2-D arrays (matrices) as its elements is called 3-D array.

```
import numpy as np

arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(arr)
```

```Create a 3-D array with two 2-D arrays, both containing two arrays with the values 1,2,3 and 4,5,6:```

## Check Number of Dimensions?

NumPy Arrays provides the **ndim** attribute that returns an integer that tells us how many dimensions the array have.

```
import numpy as np

a = np.array(42)
b = np.array([1, 2, 3, 4, 5])
c = np.array([[1, 2, 3], [4, 5, 6]])
d = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(a.ndim)
print(b.ndim)
print(c.ndim)
print(d.ndim)
```







<br/>

