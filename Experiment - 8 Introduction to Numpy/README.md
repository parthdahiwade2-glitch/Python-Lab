Parth Dahiwadde

EnTC A3 | PRN: 25070123177

Exp - 8 Study of NumPy Library in Python

___

Aim

The aim of this project is to study the NumPy (Numerical Python) library and understand how it is used for numerical computations. This includes creating arrays, performing mathematical operations, understanding array properties, indexing and slicing, and performing statistical and matrix operations.

___

Introduction

NumPy, short for Numerical Python, is one of the most powerful and widely used Python libraries for numerical and scientific computing. It provides support for large multi-dimensional arrays, mathematical functions, linear algebra, and statistical operations.

What makes NumPy stand out from regular Python lists is that it is implemented in C under the hood, which means it runs significantly faster and uses memory much more efficiently. For anyone working with data, NumPy is usually the first library they reach for.

___

Theory

1. Importing NumPy

Before using NumPy, it needs to be imported into the program. The standard convention is to import it with the alias np so we don't have to type out "numpy" every time:
pythonimport numpy as np

2. Creating NumPy Arrays

Arrays are the core of NumPy. They are created using the np.array() function:
pythonarr = np.array([1, 2, 3, 4])
Unlike Python lists, NumPy arrays are faster, use less memory, and support vectorized operations — meaning you can perform operations on an entire array at once rather than looping through it element by element.

3. Types of Arrays

NumPy arrays can exist in one, two, or three dimensions depending on the problem at hand.

A 1D array is the simplest — just a flat list of values:
pythonnp.array([1, 2, 3])

A 2D array behaves like a table or matrix with rows and columns:
pythonnp.array([[1, 2], [3, 4]])

A 3D array adds another layer of depth, useful for things like image data:
pythonnp.array([[[1, 2], [3, 4]]])

4. Array Attributes

Every NumPy array carries some useful information about itself through its attributes:

arr.ndim — tells you how many dimensions the array has

arr.shape — gives the number of rows and columns

arr.size — total count of all elements

arr.dtype — the data type stored inside (e.g., int64, float64)

For example:

pythonarr = np.array([[1, 2, 3], [4, 5, 6]])

print(arr.shape)   # Output: (2, 3)

5. Special Array Creation Functions

NumPy offers several handy shortcuts for creating arrays without typing out values manually.

zeros() fills an array entirely with zeros — useful when initializing arrays before filling them in:

pythonnp.zeros((2, 3))

ones() does the same but with ones:

pythonnp.ones((2, 3))

arange() creates an array of evenly spaced values across a range, much like Python's built-in range():

pythonnp.arange(1, 10)

linspace() is similar but lets you specify exactly how many values you want between two endpoints:

pythonnp.linspace(0, 10, 5)

6. Indexing and Slicing

Indexing lets you pick out specific elements from an array:

pythonarr[0]      # first element

arr[1, 2]   # row 1, column 2 (in a 2D array)

Slicing lets you grab a range of elements at once:

pythonarr[0:2]    # first two rows

arr[:, 1]   # entire second column

NumPy's slicing works similarly to Python lists, but it shines in multi-dimensional arrays where you can slice along multiple 
axes simultaneously.

7. Mathematical Operations

One of NumPy's biggest strengths is how naturally it handles math. Operations are applied element-wise across the entire array without needing any loops:

pythonarr + 5      # adds 5 to every element

arr * 2      # doubles every element

arr1 + arr2  # adds two arrays together

It supports all the basic operations — addition, subtraction, multiplication, division, and exponentiation — and they all run much faster than doing the same thing with a regular Python loop.

8. Statistical Functions
NumPy comes with a built-in set of statistical functions that make it easy to analyze data:

np.sum() — total of all elements

np.mean() — average value

np.median() — middle value

np.max() — largest value

np.min() — smallest value

np.std() — standard deviation

For example, finding the average of an array is as simple as:

pythonnp.mean(arr)

9. Reshaping Arrays

Sometimes you have data in one shape but need it in another. The reshape() function lets you rearrange an array's structure without changing its data:

pythonarr.reshape(2, 3)

The one rule to keep in mind is that the total number of elements must stay the same before and after reshaping. You can't add or remove elements — only rearrange them.

10. Matrix Operations

NumPy makes matrix operations straightforward. Matrix multiplication can be done two ways:
pythonnp.dot(arr1, arr2)

# or more cleanly:

arr1 @ arr2

Beyond multiplication, NumPy also supports transposing a matrix with arr.T, computing determinants, and finding inverses through its linear algebra module.

11. Broadcasting

Broadcasting is one of NumPy's more clever features. It allows operations between arrays of different shapes by automatically expanding the smaller one to match the larger:
pythonarr + 10
Here, the single value 10 is effectively applied to every element in the array. This eliminates the need for manual loops and makes code much cleaner to read and write.

Advantages of NumPy

NumPy is faster than Python lists, uses memory more efficiently, supports arrays of any number of dimensions, comes packed with mathematical and statistical tools, and is the foundation library for nearly everything in data science and machine learning.

Applications

NumPy finds use across a surprisingly wide range of fields — from data science and machine learning to scientific computing, financial analysis, signal processing, and even image processing.

___

Conclusion

NumPy is an essential library for anyone doing serious numerical work in Python. Through this study, we covered how to create arrays of different dimensions, access and modify elements through indexing and slicing, perform mathematical and statistical operations efficiently, reshape arrays as needed, and appreciate why NumPy consistently outperforms plain Python lists.
A solid understanding of NumPy is the natural first step before moving on to more advanced tools like Pandas, Scikit-learn, and the broader ecosystem of data science and AI libraries.
