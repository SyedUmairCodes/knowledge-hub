# Data Structures for Algorithms

>[!Warning]
>The book focuses on using Python as the primary language so most of the Data Structures discussed will be specific to Python.

Data structures provide a way to organize and store data in a way that is efficient for the algorithm to access and manipulate. If an algorithm needs to be able to quickly search for a particular piece of data, a data structure such as a hash table can be used.

Certain data structures are particularly well-suited for certain types of algorithms. For example, a recursive algorithm may be more easily implemented using nested data structures. Choosing the right data structure can make a significant difference in the performance of an algorithm.

Data structures can provide utility functions that make them easier to use in algorithms. Lists have functions for adding and removing elements, slicing, and iterating over the elements.

The time complexity of an algorithm can be affected by the choice of data structure. Inserting an element at the end of a list typically has a constant time complexity, but deleting an element from a list can have a time complexity of _O(n)_ in its worst-case scenario. This is because deleting an element may require shifting all of the subsequent elements in the list.

## Python's Built-in Data Structures

- A list is a mutable, ordered sequence of elements that can be nested.
- Tuples are same as lists but are immutable.
- A dictionary is an unordered collection of key-value pairs. The keys in a dictionary must be hash able.
- A set is an unordered collection of unique elements. Meaning the same value cannot be inserted twice.

**Time Complexity of Lists**

- Appending an element to the end of the list will always be a constant _O(1)_ no matter how big the element is.
- Removing an element from a list can have a time complexity of _O(n)_ depending upon where the element was located in the list and the list size.
- Slicing the list will have a time complexity of _O(n)_ depending upon the slice.
- Copying the list will have a time complexity of _O(n)_ depending upon the size of the list.

> The Time complexity of Tuples is the same as lists since the only difference if mutability.

**Time Complexity of Dictionaries**

- Searching and retrieving a value when you know the key is a constant-time operation, _O(1)._
- Adding and removing a key-value pair has a time complexity of _O(1)._
- Copying a dictionary has a time complexity of _O(n)._

**Time Complexity of Sets**

- Adding or removing an element to a set has a time complexity of _O(1)._
- Searching and retrieving an element from a set a time complexity of _O(1)._
- Copying a set has a time complexity of _O(n)_ based on the length and size of the set.

## Matrices
A matrix is a two-dimensional data structure with a fixed number of columns and rows. Each element of a matrix can be referred to by its column and the row. We can create matrices using the numpy library's arrays or using a list.

> Accessing or adding an element to a matrix has a time complexity of O(n).

NumPy arrays excel in matrix multiplication. Traditional matrix multiplication algorithms have a time complexity of O(n^3) for n x n matrices. However, NumPy employs optimized algorithms, such as the Strassen algorithm, which significantly reduce this complexity.