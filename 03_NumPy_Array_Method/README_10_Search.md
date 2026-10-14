# NumPy Searching Arrays

### Searching Arrays

You can search an array for a certain value, and return the indexes that get a match.

To search an array, use the ```where()``` method.

Find the indexes where the value is 4:

```import numpy as np

arr = np.array([1, 2, 3, 4, 5, 4, 4])
x = np.where(arr == 4)
print(x)
```

Find modulus in array find index of this answer

```
import numpy as np
arr=np.array([1,2,3,4,5,6])
findArray=np.where(arr%2==0)
print(findArray)
print(arr[findArray])
```

```Here we got [1,3,5] and at that index we got [2,4,6]```

## Search Sorted

There is a method called searchsorted() which performs a binary search in the array, and returns the index where the specified value would be inserted to maintain the search order.


***The searchsorted() method is assumed to be used on sorted arrays.***
***It check where to fit the given value in the array.***

```
import numpy as np

# Input array MUST be sorted
arr = np.array([10, 20, 30, 40, 50])

# Find where '25' fits to maintain sorted order
index = np.searchsorted(arr, 25)
print(index)  # Output: 2 (because 25 would sit between 20 and 30)

# You can also pass an array of search values
indices = np.searchsorted(arr, [5, 35, 60])
print(indices)  # Output: [0, 3, 5]
```


### Multiple Values

Find the indexes where the values 2, 4, and 6 should be inserted:

```
import numpy as np

arr = np.array([1, 3, 5, 7])

x = np.searchsorted(arr, [2, 4, 6])

print(x)

**Output: [1 2 3]**
```










<br/>
