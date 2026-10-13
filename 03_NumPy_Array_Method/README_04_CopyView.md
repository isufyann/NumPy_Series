# NumPy Array Copy vs View

### The Difference Between Copy and View

The main difference between a copy and a view of an array is that the copy is a new array, and the view is just a view of the original array.
The copy owns the data and any changes made to the copy will not affect original array, and any changes made to the original array will not affect the copy.
The view does not own the data and any changes made to the view will affect the original array, and any changes made to the original array will affect the view.

## COPY:

Make a copy, change the original array, and display both arrays:

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
x = arr.copy()
arr[0] = 42

print(arr)
print(x)
```

**The copy SHOULD NOT be affected by the changes made to the original array.**

## VIEW:

Make a view, change the original array, and display both arrays:

```code
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

x = arr.view()

arr[0] = 42

print(arr)
print(x)
```

**The view SHOULD be affected by the changes made to the original array.**
