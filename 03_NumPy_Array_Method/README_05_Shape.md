# NumPy Array Shape

### Shape of an Array

The shape of an array is the number of elements in each dimension.

## Get the Shape of an Array

NumPy arrays have an attribute called shape that returns a tuple with each index having the number of corresponding elements. **(number of colums, number of rows)**

```code
import numpy as np

arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

print(arr.shape)
```

**The example above returns (2, 4), which means that the array has 2 dimensions, where the first dimension has 2 elements and the second has 4.**

### Other example

```code
Import numpy as np
Arr=np.array([[]1,2,3,4],[5,6,7,8]])
X=arr.copy()
Print(x.shape())
```

***If 1,2,3 or so on arrays are not same, this will create an error.***
