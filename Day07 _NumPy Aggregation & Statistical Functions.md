# 📘 Day 07 – NumPy Aggregation & Statistical Functions

---

## 🎯 Learning Objectives
- Understand aggregation functions in NumPy
- Perform basic statistical analysis on arrays
- Use axis parameter for row-wise and column-wise operations
- Apply NumPy statistics in data analysis

---

## 1️⃣ Aggregation Functions in NumPy

### 🔹 Definition
Aggregation functions **summarize multiple values into a single value**.

### 🔹 Common Aggregation Functions
- `sum()`
- `mean()`
- `min()`
- `max()`
- `std()`
- `var()`

---

## 2️⃣ `sum()` – Total of Elements

### 🔹 Example

import numpy as np
- arr = np.array([10, 20, 30, 40])
- print(np.sum(arr))
- 🔹 Output
    100
---
## 3️⃣ mean() – Average Value
🔹 Example

- print(np.mean(arr))
- 🔹 Output

    25.0
---
## 4️⃣ min() and max()
🔹 Example

- print(np.min(arr))
- print(np.max(arr))
- 🔹 Output

    10 , 
    40
---
## 5️⃣ std() – Standard Deviation
🔹 Definition
Measures how much values deviate from the mean.

🔹 Example

- print(np.std(arr))
- 🔹 Output

     11.18
---
## 6️⃣ var() – Variance
🔹 Definition
Square of standard deviation.

🔹 Example

- print(np.var(arr))
🔹 Output

    125.0
---
## 7️⃣ Aggregation with axis
🔹 Definition
The axis parameter controls row-wise or column-wise operations.

🔹 Example

- arr2d = np.array([[1, 2, 3],
                  [4, 5, 6]])

- print(np.sum(arr2d, axis=0))
- 
- print(np.sum(arr2d, axis=1))

- 🔹 Output

   [5 7 9]
   [ 6 15]

🔹 Explanation
- axis=0 → Column-wise

- axis=1 → Row-wise
---
## 8️⃣ Practical Example

🔹 Example

- marks = np.array([[80, 70, 60],
                  [90, 85, 88]])

- print("Average Marks:", np.mean(marks))
- print("Highest Marks:", np.max(marks))
---
## 📌 Summary Table
| Function | Purpose |
|---------|---------|
| `sum()` | Total of elements |
| `mean()` | Average value |
| `min()` | Smallest value |
| `max()` | Largest value |
| `std()` | Standard deviation |
| `var()` | Variance |
| `axis` | Direction of operation |


