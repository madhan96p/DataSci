### 🧠 **Python If-Else and Comparisons**

Conditional statements let you control the flow of logic in your program based on certain conditions.

---

### ✅ **Basic If Statement**

```python
x = 10
if x > 5:
    print("x is greater than 5")
```

---

### 🔁 **If-Else Statement**

```python
x = 3
if x > 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")
```

---

### 🔀 **If-Elif-Else Statement**

```python
x = 5
if x > 5:
    print("Greater than 5")
elif x == 5:
    print("Equal to 5")
else:
    print("Less than 5")
```

---

### ⚖️ **Comparison Operators**

| Operator | Description              | Example  | Result |
| -------- | ------------------------ | -------- | ------ |
| `==`     | Equal to                 | `3 == 3` | `True` |
| `!=`     | Not equal to             | `4 != 5` | `True` |
| `>`      | Greater than             | `5 > 2`  | `True` |
| `<`      | Less than                | `3 < 7`  | `True` |
| `>=`     | Greater than or equal to | `5 >= 5` | `True` |
| `<=`     | Less than or equal to    | `2 <= 3` | `True` |

---

### 🔗 **Logical Operators (Used with Conditions)**

| Operator | Description                  | Example            | Result             |
| -------- | ---------------------------- | ------------------ | ------------------ |
| `and`    | True if both are true        | `x > 2 and x < 10` | `True`             |
| `or`     | True if at least one is true | `x < 2 or x == 5`  | `True`             |
| `not`    | Inverts the result           | `not(x > 5)`       | `True` if `x <= 5` |

---

### 🧪 **Nested If Statements**

```python
x = 15
if x > 10:
    if x < 20:
        print("x is between 10 and 20")
```

---

### ✨ **Ternary (One-Line If-Else)**

```python
x = 10
result = "Even" if x % 2 == 0 else "Odd"
print(result)
```

---
