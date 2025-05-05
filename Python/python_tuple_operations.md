### 📦 **Python Tuple Operations**

Tuples are ordered, immutable collections in Python. They are similar to lists, but cannot be changed after creation.

---

#### ✅ **Creating Tuples**

```python
empty = ()
single = (5,)              # Note the comma
nums = (1, 2, 3)
mixed = (1, "a", 3.5, True)
nested = ((1, 2), (3, 4))
```

---

#### 🔄 **Accessing Elements & Slicing**

| Operation      | Example     | Output   | Description                 |
| -------------- | ----------- | -------- | --------------------------- |
| Indexing       | `nums[0]`   | `1`      | Access by index             |
| Negative Index | `nums[-1]`  | `3`      | Access last element         |
| Slicing        | `nums[1:3]` | `(2, 3)` | Sub-tuple from index 1 to 2 |
| Length         | `len(nums)` | `3`      | Number of elements          |

---

#### 🧰 **Tuple Methods**

| Method    | Example         | Description                  |
| --------- | --------------- | ---------------------------- |
| `count()` | `nums.count(2)` | Number of times value occurs |
| `index()` | `nums.index(3)` | Index of first occurrence    |

---

#### ⚖️ **Tuple vs List**

| Feature     | Tuple      | List            |
| ----------- | ---------- | --------------- |
| Mutable     | ❌ No       | ✅ Yes           |
| Syntax      | `(1, 2)`   | `[1, 2]`        |
| Performance | Faster     | Slightly slower |
| Use Cases   | Fixed data | Dynamic data    |

---

#### 🔁 **Looping Through Tuple**

```python
for item in nums:
    print(item)
```

---

#### 🔍 **Membership Check**

```python
2 in nums     # True
99 in nums    # False
```

---

#### ➕ **Tuple Operations**

| Operation     | Example           | Output            | Description      |
| ------------- | ----------------- | ----------------- | ---------------- |
| Concatenation | `(1, 2) + (3, 4)` | `(1, 2, 3, 4)`    | Joins two tuples |
| Repetition    | `('a',) * 3`      | `('a', 'a', 'a')` | Repeats contents |

---

#### ♻️ **Tuple Packing and Unpacking**

```python
# Packing
person = ("Madhan", 25, "India")

# Unpacking
name, age, country = person
print(name)     # Madhan
```

---
