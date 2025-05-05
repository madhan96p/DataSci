### 🔁 **Python Loops (`for`, `while`)**

Loops are used to execute a block of code repeatedly until a condition is met.

---

### 🔹 **For Loop (with range)**

```python
for i in range(5):
    print(i)  # 0 to 4
```

---

### 🔹 **While Loop**

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

---

### 🔍 **Looping Through Sequences**

```python
# Loop through list
fruits = ['apple', 'banana', 'cherry']
for fruit in fruits:
    print(fruit)

# Loop through string
for ch in "hello":
    print(ch)
```

---

### 🔧 **Useful Loop Control Statements**

| Keyword    | Description                 | Example               |
| ---------- | --------------------------- | --------------------- |
| `break`    | Exits the loop early        | `if x == 5: break`    |
| `continue` | Skips to the next iteration | `if x == 2: continue` |
| `pass`     | Placeholder (does nothing)  | `if x == 3: pass`     |

---

### 🔂 **`for` with `else`**

```python
for i in range(3):
    print(i)
else:
    print("Loop completed")  # Runs if loop not broken
```

---

### 🔁 **Nested Loops**

```python
for i in range(2):
    for j in range(2):
        print(i, j)
```

---

### 🛑 **Infinite Loop Example (use with caution)**

```python
while True:
    user_input = input("Type 'exit' to stop: ")
    if user_input == "exit":
        break
```

---

### 🧠 **When to Use What?**

| Loop Type | Use Case                                  |
| --------- | ----------------------------------------- |
| `for`     | Known number of iterations or iterable    |
| `while`   | Unknown iterations; condition-based loops |

---
