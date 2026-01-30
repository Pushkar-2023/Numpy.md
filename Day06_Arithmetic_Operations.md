# 📘 Day 06 – Arithmetic Operations in NumPy
📌 Overview

This topic covers element-wise arithmetic operations in NumPy. These operations are widely used in data analysis, numerical computing, and machine learning to perform fast calculations on arrays.
---
🎯 Learning Objectives
---
After completing this topic, you will be able to:

Perform arithmetic operations on NumPy arrays

Understand element-wise computation

Use operators and NumPy built-in functions

Apply scalar operations using broadcasting
---
### 1️⃣ Addition
What it does

Adds elements of two arrays element by element.

#### Example
import numpy as np

- a = np.array([1, 2, 3])
- b = np.array([4, 5, 6])

- a + b
- np.add(a, b)

Output
[5 7 9]
---
### 2️⃣ Subtraction
What it does

Subtracts elements of one array from another element-wise.

#### Example
- a - b
- np.subtract(a, b)

Output
[-3 -3 -3]
---
### 3️⃣ Multiplication
What it does

Multiplies array elements element-wise.

#### Example
- a * b
- np.multiply(a, b)

Output
[ 4 10 18 ]


⚠ Note:
This is not matrix multiplication. For matrix multiplication use @ or np.dot().
---
### 4️⃣ Division
What it does

Divides elements element-wise and returns float values.

#### Example
- b / a
- np.divide(b, a)

Output
[4.  2.5 2. ]
---
### 5️⃣ Floor Division
What it does

Returns the integer part of the division.

#### Example
- b // a
- np.floor_divide(b, a)

Output
[4 2 2]
---
### 6️⃣ Power Operation
What it does

Raises each element to a given power.

#### Example
- a ** 2
- np.power(a, 2)

Output
[1 4 9]
---
### 7️⃣ Modulus (Remainder)
What it does

Returns the remainder after division.

#### Example
- b % a
- np.mod(b, a)

Output
[0 1 0]
---
### 8️⃣ Reciprocal
What it does
Returns the reciprocal (1/x) of each element.

#### Example
- arr = np.array([2, 4, 8])
- np.reciprocal(arr)

**Output**
[0.5   0.25   0.125]
---
### 9️⃣ Scalar Arithmetic (Broadcasting)
What it does

Performs arithmetic between an array and a scalar value.

#### Example
- arr = np.array([10, 20, 30])

- arr + 5
- arr * 2

Output

[15 25 35]

[20 40 60]
---
### 🔁 Operator vs Function Comparison
## 🔁 Operator vs NumPy Function Comparison

| Operation        | Operator | NumPy Function        |
|------------------|----------|-----------------------|
| Addition         | `+`      | `np.add()`            |
| Subtraction      | `-`      | `np.subtract()`       |
| Multiplication   | `*`      | `np.multiply()`       |
| Division         | `/`      | `np.divide()`         |
| Floor Division   | `//`     | `np.floor_divide()`   |
| Power            | `**`     | `np.power()`          |
| Modulus          | `%`      | `np.mod()`            |

