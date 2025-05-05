### 📘 **Python Dictionary Operations**

A **dictionary** in Python is an unordered collection of **key-value pairs**, where each key must be unique and immutable.

---

#### ✅ **Creating Dictionaries**

```python
# Basic dictionary
person = {"name": "Madhan", "age": 25, "country": "India"}

# Using dict constructor
data = dict(a=1, b=2)

# Empty dictionary
empty = {}
```

---

#### 🔎 **Accessing & Modifying Elements**

| Operation                | Example                       | Output / Description             |
| ------------------------ | ----------------------------- | -------------------------------- |
| Access by key            | `person["name"]`              | `"Madhan"`                       |
| Add or update key-value  | `person["age"] = 26`          | Updates age                      |
| Safe access with `get()` | `person.get("gender", "N/A")` | Returns `"N/A"` if key not found |

---

#### 🧰 **Common Dictionary Methods**

| Method     | Example                      | Description               |
| ---------- | ---------------------------- | ------------------------- |
| `keys()`   | `person.keys()`              | Returns all keys          |
| `values()` | `person.values()`            | Returns all values        |
| `items()`  | `person.items()`             | Returns key-value pairs   |
| `get()`    | `person.get("age")`          | Gets value safely         |
| `update()` | `person.update({"age": 27})` | Updates dictionary        |
| `pop()`    | `person.pop("country")`      | Removes and returns value |
| `clear()`  | `person.clear()`             | Clears all items          |
| `copy()`   | `new_dict = person.copy()`   | Shallow copy              |

---

#### 🔁 **Looping Through a Dictionary**

```python
for key, value in person.items():
    print(key, ":", value)
```

---

#### 🔍 **Check Existence**

```python
"name" in person     # True
"gender" not in person  # True
```

---

#### ➕ **Merging Dictionaries**

```python
dict1 = {"a": 1}
dict2 = {"b": 2}
merged = {**dict1, **dict2}   # {'a': 1, 'b': 2}
```

Or in Python 3.9+:

```python
merged = dict1 | dict2
```

---

#### ⚖️ **Dictionary vs List**

| Feature         | Dictionary                | List               |
| --------------- | ------------------------- | ------------------ |
| Structure       | Key-value pairs           | Indexed items      |
| Access Speed    | Fast (via keys)           | Slower (via index) |
| Order (Py 3.7+) | Preserves insertion order | Ordered            |
| Mutability      | Mutable                   | Mutable            |

---
