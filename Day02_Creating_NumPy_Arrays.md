

## 1️⃣ `np.array()` – Create Array from Python Objects

### 🔹 What it does

Creates a NumPy array from Python lists, tuples, or other iterable objects.

### 🔹 Syntax

```python
np.array(object, dtype=None, ndmin=0)
```

### 🔹 Example

```python
import numpy as np

arr = np.array([1, 2, 3, 4])
print(arr)
print(type(arr))
```

### 🔹 Output

```
[1 2 3 4]
<class 'numpy.ndarray'>
```

### 🔹 Key Points

* Faster than Python lists
* Supports multi-dimensional arrays
* Can force minimum dimensions using `ndmin`

---

## 2️⃣ `np.zeros()` – Array Filled with Zeros

### 🔹 What it does

Creates an array of given shape filled entirely with **0** values.

### 🔹 Syntax

```python
np.zeros(shape, dtype=float)
```

### 🔹 Examples

```python
np.zeros(5)
np.zeros((2, 3))
```

### 🔹 Output

```
[0. 0. 0. 0. 0.]
[[0. 0. 0.]
 [0. 0. 0.]]
```

### 🔹 Use Case

* Initialize arrays before calculations
* Machine learning weight initialization

---

## 3️⃣ `np.ones()` – Array Filled with Ones

### 🔹 What it does

Creates an array of given shape filled with **1** values.

### 🔹 Syntax

```python
np.ones(shape, dtype=float)
```

### 🔹 Example

```python
np.ones((3, 2))
```

### 🔹 Output

```
[[1. 1.]
 [1. 1.]
 [1. 1.]]
```

### 🔹 Use Case

* Bias initialization
* Masking and scaling operations

---

## 4️⃣ `np.empty()` – Uninitialized Array

### 🔹 What it does

Creates an array **without initializing values** (contains garbage values).

### 🔹 Syntax

```python
np.empty(shape)
```

### 🔹 Example

```python
np.empty(4)
```

### 🔹 Important Note

⚠ Values are random because memory is allocated but **not cleared**.

### 🔹 Use Case

* Faster array creation when values will be overwritten

---

## 5️⃣ `np.arange()` – Range-Based Array

### 🔹 What it does

Creates an array with evenly spaced values within a given range.

### 🔹 Syntax

```python
np.arange(start, stop, step)
```

### 🔹 Examples

```python
np.arange(5)
np.arange(1, 10, 2)
```

### 🔹 Output

```
[0 1 2 3 4]
[1 3 5 7 9]
```

### 🔹 Difference from `range()`

* Returns NumPy array
* Supports float steps

---

## 6️⃣ `np.linspace()` – Linearly Spaced Array

### 🔹 What it does

Generates **fixed number of values** evenly spaced between two numbers.

### 🔹 Syntax

```python
np.linspace(start, stop, num)
```

### 🔹 Example

```python
np.linspace(1, 10, 5)
```

### 🔹 Output

```
[ 1.    3.25  5.5   7.75 10. ]
```

### 🔹 When to Use

* Graph plotting
* Scientific calculations

---

## 7️⃣ `np.eye()` – Identity Matrix

### 🔹 What it does

Creates a **square matrix** with 1s on the diagonal and 0s elsewhere.

### 🔹 Syntax

```python
np.eye(N)
```

### 🔹 Example

```python
np.eye(3)
```

### 🔹 Output

```
[[1. 0. 0.]
 [0. 1. 0.]
 [0. 0. 1.]]
```

### 🔹 Use Case

* Linear algebra
* Machine learning algorithms

---

## 📊 Quick Comparison Table

| Function   | Purpose                | Values         |
| ---------- | ---------------------- | -------------- |
| array()    | Create array from data | User-defined   |
| zeros()    | Initialize with 0      | All zeros      |
| ones()     | Initialize with 1      | All ones       |
| empty()    | Fast allocation        | Garbage values |
| arange()   | Range values           | Step-based     |
| linspace() | Fixed count values     | Even spacing   |
| eye()      | Identity matrix        | Diagonal 1s    |



