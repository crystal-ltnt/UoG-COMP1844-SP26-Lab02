# COMP1844 - Information Analysis and Visualisation

## Laboratory Session 2: Data Types

### Overview

This lab session focuses on **one-dimensional arrays** using Python's NumPy library. By definition, an array is a collection of elements of the same type, where each element can be accessed by its index (an integer value starting from zero).

---

## Prerequisites

- Python 3.x
- NumPy library
- Jupyter Notebook (recommended)

```bash
pip install numpy
```

---

## Key Concepts

### NumPy Arrays

NumPy arrays follow similar syntax to C/C++ and Java for accessing individual elements.

### Creating Arrays

**Method 1: Using `empty` (uninitialized array)**

```python
import numpy as np

# Define number of elements
NumberOfElements = 50

# Allocate memory (elements will have "random" values from memory)
MyArray1 = np.empty(shape=NumberOfElements, dtype=int)
```

**Method 2: Using `random.randint` (initialized with random values)**

```python
# Initialise an array with 10 random integer values within [-5, 5)
MyArray2 = np.random.randint(-5, 5, 10, dtype=int)
```

### Iterating Through Arrays

**FOR Loop:**

```python
for i in range(0, 10):
    print(i, MyArray2[i])
```

**WHILE Loop:**

```python
i = int(0)
while i < 10:
    print(i, MyArray2[i])
    i = i + 1
```

---

## Tasks

### Task 1: Array Initialization and Visualization

Initialise a one-dimensional array `A` with 10 random integer numbers from the interval [0, 100] and visualise the elements alongside their indices. Remember that NumPy arrays start from index zero.

### Task 2: Sum and Average

Visualise the sum and the average value of the array.

### Task 3: Min/Max Values

Visualise the minimum and maximum values alongside their indices. Use NumPy functions: `min`, `max`, `argmax`, and `argmin`.

### Task 4: Sorting

Initialise arrays `B` and `C` with values from array `A` arranged in ascending and descending order, respectively. Visualise arrays `B` and `C`.

### Task 5: Manual Implementation

Implement at least one of Tasks 2 to 4 **without using functions from the NumPy library** (apart from initialising the array).

### Task 6: Table Visualization

Visualise arrays `A`, `B`, and `C` as a table. Display the indices of the arrays in the first column of the table.

### Task 7: Arithmetic Sequence

Initialise array `D` with 10 integer values, such that:

- The first value is **10**
- Every consecutive value equals the previous value **plus 4**

Display the array alongside its indices.

### Task 8: Guess the Number Game (Extra)

*(Complete if time permits)*

**Part 1:** Write a script that generates a random integer value between 1 and 10. Use the `random` and `datetime` libraries to guarantee a different random number every time the script is run.

**Part 2:** In another cell, write a script that:

- Reads an integer value entered by the user
- Compares it with the random value from Part 1
- Displays an appropriate message if the entered value is larger or smaller
- Congratulates the user if they guessed correctly

> **Tip:** You can hide the generated random value from the user by scrolling down the Jupyter Notebook page.

---

## Useful NumPy Functions

| Function                | Description                   |
| ----------------------- | ----------------------------- |
| `np.empty()`          | Create an uninitialized array |
| `np.random.randint()` | Generate random integers      |
| `np.sum()`            | Calculate sum of elements     |
| `np.mean()`           | Calculate average of elements |
| `np.min()`            | Find minimum value            |
| `np.max()`            | Find maximum value            |
| `np.argmin()`         | Find index of minimum value   |
| `np.argmax()`         | Find index of maximum value   |
| `np.sort()`           | Sort array in ascending order |

---

## References

1. [NumPy Official Website](https://numpy.org)
2. [NumPy Tutorial on W3Schools](https://www.w3schools.com/python/numpy/)

---

## License

This lab session is part of the COMP1844 module at the University of Greenwich.
