# Random Permutations (Tabdeel krna, ulat pulat)

## Random Permutations of Elements

A permutation refers to an arrangement of elements. e.g. [3, 2, 1] is a permutation of [1, 2, 3] and vice-versa.

The NumPy Random module provides two methods for this: ```shuffle()``` and ```permutation()```.

## Shuffling Arrays
Shuffle means changing arrangement of elements in-place. i.e. in the array itself.

### Example

Randomly shuffle elements of following array:

```
from numpy import random
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

random.shuffle(arr)

print(arr)
```
***Shuffle() will change the original Array.***


## Generating Permutation of Arrays

### Example

Generate a random permutation of elements of following array:

```
from numpy import random
import numpy as np
arr=np.array([1,2,3,4,5])
print("Original array", arr)
print("Permuted array", random.permutation(arr))
```

***The permutation() method returns a re-arranged array (and leaves the original array un-changed).***














<br/>
