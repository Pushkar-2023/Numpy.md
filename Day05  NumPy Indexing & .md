# 📘 Day 5 – NumPy Indexing and Slicing

Indexing and slicing are fundamental NumPy concepts used to **access, filter, and manipulate array data efficiently**.  
They are widely used in **data analysis, machine learning, image processing, and deep learning**.

---

## 🔹 What is Indexing?

**Indexing** is used to access **individual elements** from a NumPy array.

### 📌 Key Rules
- Index starts from **0**
- Negative indexing starts from the **end**
- Works with **1D, 2D, and ND arrays**
---
### 🔹1D Array Indexing


import numpy as np

a = np.array([10, 20, 30, 40, 50])

- print(a[0])      , First element
- print(a[2])      , Third element
- print(a[-1])     , Last element
- print(a[-2])     , Second last element

### 🔹 1D Array Slicing
Slicing is used to extract a portion of an array.

### 📌 Syntax

array[start : stop : step]
✅ Examples

- print(a[1:4])    , Index 1 to 3
- print(a[:3])     , Start to index 2
- print(a[2:,)     , Index 2 to end
- print(a[::2])    , Every second element
- print(a[::-1])   , Reverse array
🧠 Notes
start → included

stop → excluded

Faster than loops
---
### 🔹 Indexing in 2D Array
2D arrays work like tables (rows × columns).

✅ Example

b = np.array([
    [10, 20, 30],
    [40, 50, 60],
    [70, 80, 90]
])

- print(b[1, 1])     ,50
- print(b[0, 2])     , 30
- print(b[-1, -1])   , 90
📌 Format

array[row, column]

### 🔹 Slicing in 2D Array
Used for row-wise and column-wise operations.

✅ Examples

- print(b[0:2, 0:2])     # Top-left 2x2 matrix
- print(b[:, 1])         # All rows, column index 1
- print(b[1, :])         # Entire second row
- print(b[:, ::-1])      # Reverse columns
---
### 🔹 Indexing in 3D Array
3D arrays are commonly used in images and deep learning.

✅ Example

c = np.array([
    [[1, 2, 3], [4, 5, 6]],
    [[7, 8, 9], [10, 11, 12]]
])

- print(c[0])          , First block
- print(c[1, 0])       , First row of second block
- print(c[0, 1, 2])    , Single element
📌 Format

array[depth, row, column]

### 🔹 Slicing in 3D Array
✅ Examples

- print(c[:, 1, :])     , All blocks, row index 1
- print(c[:, :, 0])     , First column from all blocks
- print(c[1, :, ::-1])  , Reverse columns in second block
---
### 🔹 Indexing vs Slicing

| Feature | Indexing | Slicing |
|--------|----------|---------|
| Output | Single value | Sub-array |
| Speed | Fast | Fast |
| Usage | Specific element | Range selection |

