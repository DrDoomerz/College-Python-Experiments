# 🧪 Experiment 9 – Study of NumPy Library

---

## 🎯 Aim

To study the NumPy library in Python and understand array creation, array properties, mathematical operations, statistical functions, and basic linear algebra operations using NumPy.

---

## 📚 Theory

### 🔹 Introduction to NumPy

NumPy (Numerical Python) is a powerful Python library used for:

* Fast numerical computations
* Handling multi-dimensional arrays
* Performing mathematical and statistical operations
* Executing linear algebra computations

NumPy is faster than Python lists because:

* Data is stored in contiguous memory locations
* Operations are implemented using optimized C code
* It supports vectorized operations (no explicit loops required)

NumPy also forms the base for advanced libraries like **Pandas, SciPy, and Matplotlib**.

---

# 🔍 Commands Used in the Experiment

---

## 1️⃣ Importing NumPy

```python
import numpy as np
```

* Imports the NumPy library.
* `np` is an alias for easier access to NumPy functions.

---

## 2️⃣ Creating Arrays

```python
a = np.array([1,10,20,30,40,50,100])
b = np.array([[1,2,3],[4,5,6],[7,8,9]])
```

### `np.array()`

* Converts Python lists into NumPy arrays.
* Can create:

  * 1D arrays (vectors)
  * 2D arrays (matrices)
  * Multi-dimensional arrays

`a` → 1D array
`b` → 2D array (3 × 3 matrix)

---

## 3️⃣ Array Properties

### 🔹 `ndim`

```python
a.ndim
b.ndim
```

* Returns number of dimensions of the array.
* `a.ndim = 1`
* `b.ndim = 2`

---

### 🔹 `size`

```python
a.size
b.size
```

* Returns total number of elements.
* `a.size = 7`
* `b.size = 9`

---

### 🔹 `shape`

```python
a.shape
b.shape
```

* Returns tuple representing dimensions.
* `a.shape = (7,)`
* `b.shape = (3,3)`

---

### 🔹 `dtype`

```python
a.dtype
b.dtype
```

* Returns datatype of elements.
* Default datatype depends on input.
* In this experiment → `int64`.

---

## 4️⃣ Displaying Arrays

```python
display(a)
display(b)
```

* Used in Google Colab / Jupyter Notebook.
* Displays formatted array output.
* More structured than `print()`.

---

## 5️⃣ Built-in Array Creation Functions

---

### 🔹 `np.zeros((rows, columns))`

```python
np.zeros((2,3))
```

* Creates a matrix filled with zeros.
* Default datatype: float.

---

### 🔹 `np.ones((rows, columns))`

```python
np.ones((3,3))
```

* Creates a matrix filled with ones.

---

### 🔹 `np.eye(n)`

```python
np.eye(3)
```

* Creates an identity matrix of order `n`.
* Diagonal elements = 1, others = 0.

---

### 🔹 `np.arange(start, stop, step)`

```python
np.arange(1,10,2)
```

* Generates values from start to stop (exclusive).
* Step size controls spacing.
* Output: `[1 3 5 7 9]`

---

### 🔹 `np.linspace(start, stop, num)`

```python
np.linspace(0,1,4)
```

* Generates evenly spaced numbers.
* Includes both start and stop values.
* Step size formula:

[
\text{Step Size} = \frac{(stop - start)}{(num - 1)}
]

---

## 6️⃣ Arithmetic (Vectorized) Operations

```python
b * 2
a + 5
```

* NumPy performs element-wise operations.
* No loops required.
* Faster execution.
* Automatically applies operation to each element.

---

## 7️⃣ Statistical Functions

---

### 🔹 `np.mean()`

```python
np.mean(a)
np.mean(b)
```

* Returns arithmetic mean.

---

### 🔹 `np.median()`

```python
np.median(a)
np.median(b)
```

* Returns middle value after sorting.

---

### 🔹 `np.max()` and `np.min()`

```python
np.max(a)
np.min(a)
```

* Returns maximum and minimum values.

---

### 🔹 `np.sum()`

```python
np.sum(a)
```

* Returns sum of all elements.

---

### 🔹 `np.std()`

```python
np.std(a)
```

* Returns standard deviation.
* Measures dispersion of data.

---

### 🔹 `np.var()`

```python
np.var(a)
```

* Returns variance.
* Square of standard deviation.

---

## 8️⃣ Linear Algebra Operations

---

### 🔹 Transpose

```python
A.T
```

* Converts rows into columns.

---

### 🔹 Determinant

```python
np.linalg.det(A)
```

* Computes determinant of matrix.
* If determinant ≠ 0 → matrix is invertible.

---

### 🔹 Inverse

```python
np.linalg.inv(A)
```

* Computes inverse of matrix.
* Only possible if determinant is non-zero.

---

### 🔹 Matrix Multiplication

```python
np.dot(A, A)
```

* Performs matrix multiplication.
* Follows row × column multiplication rule.

---

# 📊 Observations

* NumPy arrays are more efficient than Python lists.
* Vectorized operations eliminate the need for loops.
* Built-in statistical functions simplify data analysis.
* Linear algebra operations can be easily performed using NumPy.

---

# Conclusion

The experiment successfully demonstrated the functionality of the NumPy library for array creation, manipulation, statistical analysis, and linear algebra operations.

NumPy provides a structured, efficient, and high-performance environment for numerical computation and forms the foundation for advanced data science and engineering applications.

---

## 👨‍🎓 Student Details

* **Name:** Rachit Jajoo
* **PRN:** 25070123088
* **Branch:** Electronics and Telecommunication (ENTC)
* **Batch:** B1
* **Institute:** Symbiosis Institute of Technology, Pune
