# NumPy Array Reshaping
### Reshaping arrays
Reshaping means changing the shape of an array.
The shape of an array is the number of elements in each dimension.
By reshaping we can add or remove dimensions or change number of elements in each dimension.
## Reshape From 1-D to 2-D
Convert the following 1-D array with 12 elements into a 2-D array.
The outermost dimension will have 4 arrays, each with 3 elements:
```code
import numpy as np
arr=np.array([1,2,3,4,5,6,7,8,9,10,11,12])
newarr=arr.reshape(3,4);
print(newarr)
```

```Output: 
[[ 1  2  3  4]
 [ 5  6  7  8]
 [ 9 10 11 12]]
```
***As long as the elements required for reshaping are equal in both shapes (rows and cols).***

# Flattening the arrays
Flattening array means converting a multidimensional array into a 1D array.
We can use reshape(-1) to do this.
We can use reshape(-1) to do this.
``Convert the array into a 1D array:```

```code
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

newarr = arr.reshape(-1)

print(newarr)
```

```code
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

newarr = arr.reshape(6)

print(newarr)
```

***Note: There are a lot of functions for changing the shapes of arrays in numpy flatten, ravel and also for rearranging the elements rot90, flip, fliplr, flipud etc. These fall under Intermediate to Advanced section of numpy.***






<br/>
