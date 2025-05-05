### 📋 **Python List Operations**

Lists in Python are ordered, mutable collections used to store multiple items in a single variable.

---

#### ✅ **Creating Lists**

```python
empty_list = []
numbers = [1, 2, 3, 4]
mixed = [1, "two", 3.0, True]
nested = [[1, 2], [3, 4]]
```

---

#### 🔄 **Accessing & Slicing**

| Operation      | Example        | Output   | Description                |
| -------------- | -------------- | -------- | -------------------------- |
| Indexing       | `numbers[0]`   | `1`      | Access first element       |
| Negative index | `numbers[-1]`  | `4`      | Access last element        |
| Slicing        | `numbers[1:3]` | `[2, 3]` | Elements from index 1 to 2 |
| Step slicing   | `numbers[::2]` | `[1, 3]` | Every 2nd element          |

---

#### 🧰 **Common List Methods**

| Method      | Example                   | Description                       |
| ----------- | ------------------------- | --------------------------------- |
| `append()`  | `numbers.append(5)`       | Adds item to end                  |
| `insert()`  | `numbers.insert(2, 99)`   | Inserts at position               |
| `extend()`  | `numbers.extend([6, 7])`  | Appends another iterable          |
| `pop()`     | `numbers.pop()`           | Removes and returns last element  |
| `remove()`  | `numbers.remove(2)`       | Removes first occurrence of value |
| `clear()`   | `numbers.clear()`         | Removes all items                 |
| `index()`   | `numbers.index(3)`        | Returns index of first match      |
| `count()`   | `numbers.count(1)`        | Counts occurrences                |
| `sort()`    | `numbers.sort()`          | Sorts list in ascending order     |
| `reverse()` | `numbers.reverse()`       | Reverses the list                 |
| `copy()`    | `copied = numbers.copy()` | Copies the list                   |

---

#### 🔁 **Looping Through a List**

```python
for item in numbers:
    print(item)
```

---

#### 🔍 **Membership Check**

```python
3 in numbers       # True
99 not in numbers  # Depends on contents
```

---

#### ➕ **List Operators**

| Operator | Use Case      | Example           | Result         |
| -------- | ------------- | ----------------- | -------------- |
| `+`      | Concatenation | `[1, 2] + [3, 4]` | `[1, 2, 3, 4]` |
| `*`      | Repetition    | `[1, 2] * 2`      | `[1, 2, 1, 2]` |

---
