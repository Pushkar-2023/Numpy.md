# 📘 Introduction to NumPy

NumPy (Numerical Python) is an open-source Python library used for numerical and scientific computing.
It provides support for large, multi-dimensional arrays and matrices, along with a large collection
of high-level mathematical functions.

NumPy is the foundation library for:
- Data Science
- Machine Learning
- Artificial Intelligence
- Image Processing
- Scientific Research

---

## ❓ Why NumPy Instead of Python Lists?

| Feature | Python List | NumPy Array |
|------|------------|-------------|
| Speed | Slow | Very Fast |
| Memory | More | Less |
| Operations | Loop required | Vectorized |
| Data Type | Mixed | Same type |

NumPy arrays store data in **contiguous memory**, which makes operations faster.

---

## 🔑 Key Features of NumPy

### 1️⃣ ndarray (N-Dimensional Array)
- Core data structure in NumPy
- Faster than Python lists
- Stores homogeneous data

### 2️⃣ Vectorized Operations
- No loops required
- Operations apply to entire arrays at once

### 3️⃣ Broadcasting
- Allows operations between arrays of different shapes

### 4️⃣ Mathematical Functions
- Linear algebra
- Trigonometry
- Statistics

### 5️⃣ Integration
- Works seamlessly with Pandas, Matplotlib, Scikit-learn

---

## 🔎 Example

```python
import numpy as np

arr = np.array([1, 2, 3])
print("Array:", arr)
print("Array + 10:", arr + 10)
