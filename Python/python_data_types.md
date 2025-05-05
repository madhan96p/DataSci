### 📘 **Python Data Types**

Python has several built-in data types that are used to store and manipulate different kinds of data.

---

#### 🧮 **Basic Data Types**

| Data Type | Example           | Description                     |
| --------- | ----------------- | ------------------------------- |
| `int`     | `x = 5`           | Integer (whole number)          |
| `float`   | `y = 3.14`        | Floating point number (decimal) |
| `complex` | `z = 2 + 3j`      | Complex number                  |
| `bool`    | `is_true = True`  | Boolean (True or False)         |
| `str`     | `name = "Madhan"` | String (textual data)           |

---

#### 📦 **Sequence Data Types**

| Data Type | Example         | Description                                 |
| --------- | --------------- | ------------------------------------------- |
| `list`    | `l = [1, 2, 3]` | Ordered, mutable, allows duplicates         |
| `tuple`   | `t = (1, 2, 3)` | Ordered, immutable, allows duplicates       |
| `range`   | `r = range(5)`  | Immutable sequence of numbers from 0 to n-1 |
| `str`     | `"hello"`       | Sequence of characters                      |

---

#### 🗂 **Mapping Data Type**

| Data Type | Example                | Description                              |
| --------- | ---------------------- | ---------------------------------------- |
| `dict`    | `d = {"a": 1, "b": 2}` | Key-value pairs, unordered (as of < 3.7) |

---

#### 🔢 **Set Data Types**

| Data Type   | Example             | Description              |
| ----------- | ------------------- | ------------------------ |
| `set`       | `{1, 2, 3}`         | Unordered, no duplicates |
| `frozenset` | `frozenset([1, 2])` | Immutable version of set |

---

#### 📄 **Binary Data Types**

| Data Type    | Example                    | Description                              |
| ------------ | -------------------------- | ---------------------------------------- |
| `bytes`      | `b = b"hello"`             | Immutable sequence of bytes              |
| `bytearray`  | `ba = bytearray([65, 66])` | Mutable sequence of bytes                |
| `memoryview` | `mv = memoryview(b"abc")`  | View object of another bytes-like object |

---

#### 🔄 **Type Checking & Conversion**

| Function  | Example        | Output            |
| --------- | -------------- | ----------------- |
| `type()`  | `type(5)`      | `<class 'int'>`   |
| `int()`   | `int("5")`     | `5`               |
| `float()` | `float("3.5")` | `3.5`             |
| `str()`   | `str(123)`     | `'123'`           |
| `list()`  | `list("abc")`  | `['a', 'b', 'c']` |

---
