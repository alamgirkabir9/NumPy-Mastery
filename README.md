# 🌟 NumPy Mastery Roadmap

## 📌 1. Introduction to NumPy

### 🔹 What is NumPy?
NumPy (Numerical Python) is a powerful library for numerical computing in Python. It provides support for large multidimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays.

### 🔹 Installing NumPy
```bash
pip install numpy
```

---
## 📌 2. NumPy Arrays

### 🔹 Creating a 1D Array
```python
import numpy as np
arr1d = np.array([1, 2, 3, 4, 5])
print(arr1d)
```

### 🔹 Creating a 2D Array
```python
arr2d = np.array([[1, 2, 3], [4, 5, 6]])
print(arr2d)
```

### 🔹 Checking Array Properties
```python
print(arr1d.shape)  # (5,)
print(arr2d.shape)  # (2,3)
print(arr1d.dtype)  # int32 or int64 depending on the system
print(arr2d.ndim)   # Number of dimensions
```

### 🔹 Special Arrays
```python
print(np.zeros((3,3)))  # Zeros array
print(np.ones((2,3)))   # Ones array
print(np.eye(3))        # Identity matrix
print(np.random.rand(2,3))  # Random array
```

---
## 📌 3. Array Operations

### 🔹 Arithmetic Operations
```python
arr = np.array([1, 2, 3, 4])
print(arr + 2)  # Adds 2 to each element
print(arr * 3)  # Multiplies each element by 3
```

### 🔹 Element-wise Operations
```python
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
print(arr1 + arr2)  # Element-wise addition
print(arr1 * arr2)  # Element-wise multiplication
```

---
## 📌 4. Indexing and Slicing
```python
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr[0, 1])  # Accessing element at row 0, column 1
print(arr[:, 1])  # Accessing the second column
print(arr[1, :])  # Accessing the second row
```

---
## 📌 5. Reshaping and Manipulating Arrays
```python
arr = np.arange(9)  # Creates an array from 0 to 8
reshaped_arr = arr.reshape((3, 3))  # Reshape to 3x3 matrix
print(reshaped_arr)

# Flattening an array
flattened = reshaped_arr.flatten()
print(flattened)
```

---
## 📌 6. Statistical and Mathematical Functions
```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
print(np.mean(arr))  # Mean
print(np.median(arr))  # Median
print(np.std(arr))  # Standard deviation
print(np.sum(arr))  # Sum of elements
print(np.min(arr), np.max(arr))  # Minimum and maximum
```

---
## 📌 7. Broadcasting
```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr + np.array([10, 20, 30]))  # Adds [10,20,30] to each row
```

---
## 📌 8. Linear Algebra with NumPy
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

# Matrix multiplication
print(np.dot(A, B))

# Inverse of a matrix
print(np.linalg.inv(A))

# Determinant
print(np.linalg.det(A))
```

---
## 📌 9. Working with Missing Data
```python
arr = np.array([1, 2, np.nan, 4, 5])
print(np.isnan(arr))  # Identifying NaN values
print(np.nanmean(arr))  # Mean ignoring NaN values
```

---
## 📌 10. Saving and Loading Data
```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
np.save('array.npy', arr)  # Save as .npy file
loaded_arr = np.load('array.npy')  # Load the file
print(loaded_arr)
```

---
## 🎯 Conclusion
This roadmap provides a structured path to mastering NumPy. Practicing these concepts with real-world datasets will solidify your understanding! 🚀

