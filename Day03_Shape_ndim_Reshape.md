# Day 03 – Shape, ndim & Reshape in NumPy



This document covers **array dimensions, shape manipulation, and reshaping techniques** in NumPy. These concepts are **very important for Data Analysis, Machine Learning, and Interviews**.

---

## 🎯 Learning Objectives

By the end of this day, you will understand:

* What dimensions mean in NumPy
* How to check array shape and number of dimensions
* How to reshape arrays correctly
* How NumPy automatically calculates dimensions using `-1`

---

## 1️⃣ Dimensions in NumPy

### 🔹 What is a Dimension?

A dimension represents the **level of depth** in an array.

| Array Type | Example           | Dimensions |
| ---------- | ----------------- | ---------- |
| Scalar     | `10`              | 0D         |
| Vector     | `[1, 2, 3]`       | 1D         |
| Matrix     | `[[1,2],[3,4]]`   | 2D         |
| Tensor     | `[[[1,2],[3,4]]]` | 3D         |

---

## 2️⃣ `.ndim` – Number of Dimensions

### 🔹 What it does

Returns the **number of dimensions** of a NumPy array.

### 🔹 Example

```python
import numpy as np

a = np.array([1, 2, 3])
b = np.array([[1, 2, 3], [4, 5, 6]])

print(a.ndim)  # 1
print(b.ndim)  # 2
```

### 🔹 Interview Tip

> ndim tells **how complex** the data structure is.

---

## 3️⃣ `.shape` – Structure of the Array

### 🔹 What it does

Returns a tuple representing **number of rows and columns** (or more for higher dimensions).

### 🔹 Example

```python
arr = np.array([[1, 2, 3],
                [4, 5, 6]])

print(arr.shape)
```

### 🔹 Output

```
(2, 3)
```

### 🔹 Meaning

* 2 → rows
* 3 → columns

---

## 4️⃣ `ndmin` – Force Minimum Dimensions

### 🔹 What it does

Forces NumPy to create an array with **at least given number of dimensions**.

### 🔹 Example

```python
arr = np.array([1, 2, 3], ndmin=5)
print(arr)
print(arr.shape)
```

### 🔹 Output

```
[[[[[1 2 3]]]]]
(1, 1, 1, 1, 3)
```

### 🔹 Key Point

Extra dimensions are added **at the beginning**.

---

## 5️⃣ `.reshape()` – Change Shape of Array

### 🔹 What it does

Changes the shape of an array **without changing the data**.

### 🔹 Rule

Total number of elements **must remain the same**.

### 🔹 Example

```python
arr = np.array([1, 2, 3, 4, 5, 6])

new_arr = arr.reshape(2, 3)
print(new_arr)
```

### 🔹 Output

```
[[1 2 3]
 [4 5 6]]
```

---

## 6️⃣ Using `-1` in Reshape (Auto Calculation)

### 🔹 What `-1` Means

> "NumPy, you calculate this dimension for me."

### 🔹 Example 1: Flattening

```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
flat = arr.reshape(-1)
print(flat)
```

### 🔹 Output

```
[1 2 3 4 5 6]
```

### 🔹 Example 2: Auto Columns

```python
arr = np.array([1, 2, 3, 4, 5, 6])
reshaped = arr.reshape(3, -1)
print(reshaped)
```

### 🔹 Output

```
[[1 2]
 [3 4]
 [5 6]]
```

### ⚠ Important Rule

* Only **one `-1`** is allowed in reshape

---

## 7️⃣ Practical Use Cases

* Preparing data for machine learning models
* Converting 1D data into matrix form
* Flattening images or matrices
* Feature engineering

---

## 📌 Common Errors to Avoid

❌ Using reshape with mismatched size
❌ Using more than one `-1`
❌ Assuming reshape changes data values

---




