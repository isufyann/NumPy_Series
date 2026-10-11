
### NumPy as Python Library

```text
NumPy is a Python library.
NumPy is used for working with arrays.
NumPy is short for "Numerical Python".
```


###  What is NumPy?
NumPy is a Python library used for working with arrays.
It also has functions for working in domain of linear algebra, fourier transform, and matrices.
NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely.
NumPy stands for Numerical Python.

--- 

### Why Use NumPy?
In Python we have lists that serve the purpose of arrays, but they are slow to process.
NumPy aims to provide an array object that is up to 50x faster than traditional Python lists.
The array object in NumPy is called ndarray, it provides a lot of supporting functions that make working with ndarray very easy.
Arrays are very frequently used in **data science**, where speed and resources are very important.

``` Data Science: is a branch of computer science where we study how to store, use and analyze data for deriving information from it.```

### Why is NumPy Faster Than Lists?
NumPy arrays are stored at one continuous place in memory unlike lists, so processes can access and manipulate them very efficiently.
This behavior is called locality of reference in computer science.
This is the main reason why NumPy is faster than lists. Also it is optimized to work with latest CPU architectures.

### Which Language is NumPy written in?
NumPy is a Python library and is written partially in Python, but most of the parts that require fast computation are written in ```C or C++.```

```The source code for NumPy is located at this github repository https://github.com/numpy/numpy```

```github: enables many people to work on the same codebase.```

---

# NumPy Getting Started

## Installation of NumPy

Use **Google Colab**



# NumPy as np

NumPy is usually imported under the np alias.

> ```alias: In Python alias are an alternate name for referring to the same thing.```

>> We can change alias name from np to other like ns or else.

## Checking NumPy Version

The version string is stored under __version__ attribute.

```code
import numpy as np

print(np.__version__)
```

--- 

NumPy is used to work with arrays. The array object in NumPy is called ndarray.

We can create a NumPy ndarray object by using the array() function.

```
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)

print(type(arr))
```

```type(): This built-in Python function tells us the type of the object passed to it. Like in above code it shows that arr is numpy.ndarray type.```


<br/>
 
