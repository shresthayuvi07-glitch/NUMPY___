# NumPy Learning Repository

A beginner-friendly repository for learning **NumPy (Numerical Python)** from the basics to practical data-analysis operations.

## 📌 About NumPy

**NumPy** is a fundamental Python library for numerical computing. It provides powerful tools for working with arrays, mathematical operations, statistics, linear algebra, and multidimensional data.

NumPy is widely used in:

* 📊 Data Analysis
* 🤖 Machine Learning
* 🧠 Artificial Intelligence
* 📈 Data Science
* 🔬 Scientific Computing
* 📐 Mathematical Computing

---

## 🚀 Installation

Install NumPy using `pip`:

```bash
pip install numpy
```

Check the installed version:

```python
import numpy as np

print(np.__version__)
```

---

## 📚 Topics Covered

This repository covers the following NumPy concepts:

### 1. NumPy Introduction

* What is NumPy?
* Why use NumPy?
* Installing NumPy
* Importing NumPy
* Checking NumPy version

### 2. NumPy Arrays

Creating arrays:

```python
import numpy as np

arr = np.array([10, 20, 30, 40, 50])

print(arr)
```

### 3. Dimensions of Arrays

NumPy arrays can have different dimensions:

* 0-D — Scalar
* 1-D — Vector
* 2-D — Matrix
* 3-D — Tensor
* N-D — Multidimensional array

Example:

```python
arr = np.array([
    [1, 2, 3],
    [4, 5, 6]
])

print(arr.ndim)
```

Output:

```text
2
```

---

## 🔢 Array Attributes

Important NumPy attributes:

```python
arr.ndim
arr.shape
arr.size
arr.dtype
```

Example:

```python
arr = np.array([
    [10, 20, 30],
    [40, 50, 60]
])

print("Dimensions:", arr.ndim)
print("Shape:", arr.shape)
print("Size:", arr.size)
print("Data Type:", arr.dtype)
```

---

## 🏗️ Creating Special Arrays

### Zeros

```python
np.zeros((3, 4))
```

### Ones

```python
np.ones((3, 4))
```

### Full

```python
np.full((2, 3), 7)
```

### Identity Matrix

```python
np.eye(3)
```

### Range

```python
np.arange(1, 11)
```

### Evenly Spaced Values

```python
np.linspace(0, 10, 5)
```

---

## 🔍 Indexing and Slicing

NumPy supports indexing and slicing similar to Python lists.

```python
arr = np.array([10, 20, 30, 40, 50])

print(arr[0])
print(arr[2])
print(arr[1:4])
```

For a 2-D array:

```python
arr = np.array([
    [1, 2, 3],
    [4, 5, 6]
])

print(arr[0, 1])
print(arr[:, 1])
```

---

## ➕ NumPy Mathematical Operations

NumPy allows mathematical operations directly on arrays.

```python
a = np.array([10, 20, 30])
b = np.array([1, 2, 3])

print(a + b)
print(a - b)
print(a * b)
print(a / b)
```

---

## 📊 Statistical Functions

Common statistical functions:

```python
np.mean(arr)
np.median(arr)
np.std(arr)
np.var(arr)
np.min(arr)
np.max(arr)
np.sum(arr)
```

Example:

```python
marks = np.array([70, 80, 90, 60, 85])

print("Mean:", np.mean(marks))
print("Maximum:", np.max(marks))
print("Minimum:", np.min(marks))
```

---

## 🔄 Reshaping Arrays

Change the shape of an array using `.reshape()`:

```python
arr = np.arange(1, 13)

new_arr = arr.reshape(3, 4)

print(new_arr)
```

Output:

```text
[[ 1  2  3  4]
 [ 5  6  7  8]
 [ 9 10 11 12]]
```

---

## 🔗 Joining Arrays

### Concatenate

```python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

result = np.concatenate((a, b))

print(result)
```

### Stack

```python
np.vstack((a, b))
np.hstack((a, b))
```

---

## 🔎 Filtering Arrays

NumPy supports Boolean indexing.

```python
arr = np.array([10, 20, 30, 40, 50])

result = arr[arr > 25]

print(result)
```

Output:

```text
[30 40 50]
```

---

## 🧮 Universal Functions

NumPy provides many mathematical functions:

```python
np.sqrt(arr)
np.square(arr)
np.abs(arr)
np.round(arr)
np.exp(arr)
np.log(arr)
```

Example:

```python
numbers = np.array([1, 4, 9, 16])

print(np.sqrt(numbers))
```

---

## 🔀 Sorting Arrays

```python
arr = np.array([50, 10, 40, 20, 30])

print(np.sort(arr))
```

Output:

```text
[10 20 30 40 50]
```

---

## 🎲 Random Numbers

NumPy provides a random module for generating random data.

```python
np.random.randint(1, 100, 10)
```

Generate random decimal values:

```python
np.random.rand(5)
```

Set a random seed:

```python
np.random.seed(42)
```

---

## ⚡ Why Use NumPy?

Compared with normal Python lists, NumPy arrays are designed for efficient numerical operations.

### Python List

```python
numbers = [1, 2, 3, 4, 5]
```

### NumPy Array

```python
numbers = np.array([1, 2, 3, 4, 5])
```

NumPy provides:

* Faster numerical operations
* Multidimensional arrays
* Vectorized calculations
* Mathematical functions
* Statistical functions
* Linear algebra tools
* Efficient memory usage

---

## 📁 Repository Structure

A possible structure for this repository:

```text
NumPy/
│
├── README.md
│
├── 01_Introduction/
│   └── introduction.py
│
├── 02_Arrays/
│   └── arrays.py
│
├── 03_Dimensions/
│   └── dimensions.py
│
├── 04_Indexing_Slicing/
│   └── indexing.py
│
├── 05_Array_Operations/
│   └── operations.py
│
├── 06_Array_Functions/
│   └── functions.py
│
├── 07_Reshaping/
│   └── reshape.py
│
├── 08_Statistics/
│   └── statistics.py
│
├── 09_Filtering/
│   └── filtering.py
│
├── 10_Random/
│   └── random.py
│
└── 11_Linear_Algebra/
    └── linear_algebra.py
```

---

## 🛠️ Requirements

* Python 3.x
* NumPy

Install NumPy:

```bash
pip install numpy
```

---

## 🎯 Learning Goals

After completing this repository, you should be able to:

* Understand NumPy arrays
* Work with multidimensional data
* Use indexing and slicing
* Perform mathematical operations
* Calculate statistics
* Reshape arrays
* Filter array data
* Generate random data
* Perform basic linear algebra
* Use NumPy for data-analysis tasks

---

## 🔗 NumPy Documentation

Official NumPy documentation:

https://numpy.org/doc/

---

## 📖 Recommended Learning Path

```text
Python Basics
      ↓
NumPy
      ↓
Pandas
      ↓
Matplotlib
      ↓
Seaborn
      ↓
Data Analysis
```

---

## 👨‍💻 Author

**Yubaraj Shrestha**

This repository is created for learning and practicing **NumPy and Python data analysis**.

---

## ⭐ Support

If you find this repository useful, consider giving it a ⭐ on GitHub!
