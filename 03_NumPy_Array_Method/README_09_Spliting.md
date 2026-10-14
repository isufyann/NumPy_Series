# NumPy Splitting Array

### Splitting NumPy Arrays

Splitting is reverse operation of Joining.

Joining merges multiple arrays into one and Splitting breaks one array into multiple.

We use array_split() for splitting arrays, we pass it the array we want to split and the number of splits.

**Split the array in 3 parts:**

```code
import numpy as np

arr=np.array([1,2,3,4,5,6])

newarr=np.array_split(arr,3)

print(newarr)
```

```Output:
Output:
[array([1, 2]), array([3, 4]), array([5])]
```
We can split it into 3,4,5 parts.

***Note: The return value is a list containing three arrays.***

**Note: We also have the method split() available but it will not adjust the elements when elements are less in source array for splitting like in example above, array_split() worked properly but split() would fail.**


## Split Into Arrays

The return value of the array_split() method is a list containing each of the split as an array.

If you split an array into 3 arrays, you can access them from the result just like any array element:

Access the splitted arrays:

```
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6])

newarr = np.array_split(arr, 3)

print(newarr[0])
print(newarr[1])
print(newarr[2])
```











<br/>
