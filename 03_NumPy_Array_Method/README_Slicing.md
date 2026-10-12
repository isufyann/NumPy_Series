# NumPy Array Slicing

## Slicing arrays

Slicing in python means taking elements from one given index to another given index.
We pass slice instead of index like this: [start:end].
We can also define the step, like this: [start:end:step].
If we don't pass start its considered 0
If we don't pass end its considered length of array in that dimension
If we don't pass step its considered 1
in python means taking elements from one given index to another given index.

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7])

print(arr[1:5])
```

```Note: The result includes the start index, but excludes the end index.```


## Example

Slice elements from index 4 to the end of the array:

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7])

print(arr[4:])
```

### Example

Slice elements from the beginning to index 4 (not included):

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7])

print(arr[:4])
```

## Negative Slicing

### Example

Slice from the index 3 from the end to index 1 from the end:

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7])

print(arr[-3:-1])
```


# STEP

## Use the step value to determine the step of the slicing:

### Example

Return every other element from index 1 to index 5:

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7,8,9,10])

print(arr[1:10:2])
```
```Output: [ 2  4  6  8 10]```

### Example

Return every other element from the entire array:

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7])

print(arr[::2])
```

```Output: [1,3,5,7,9]```

# Slicing 2-D Arrays

From the second element, slice elements from index 1 to index 4 (not included):

```code
import numpy as np

arr = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10],[11,12,13,14,15]])

print(arr[2, 1:4])

```

```Output: [12 13 14]```

***Note: Remember that second element has index 1***

From both elements, return index 2:

```code
import numpy as np

arr = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10],[11,12,13,14,15]])

print(arr[0:3, 2])

```

From both elements, slice index 1 to index 4 (not included), this will return a 2-D array:

```code
import numpy as np

arr = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])

print(arr[0:2, 1:4])
```












<br/>
