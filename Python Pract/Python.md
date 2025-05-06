# Python Keywords Table

This table contains all the Python reserved keywords, neatly arranged into columns. It provides a quick reference to the Python language keywords, split across 5 columns.

| Col 1     | Col 2     | Col 3    | Col 4    | Col 5    |
|-----------|-----------|----------|----------|----------|
| False     | None      | True     | and      | as       |
| assert    | async     | await    | break    | class    |
| continue  | def       | del      | elif     | else     |
| except    | finally   | for      | from     | global   |
| if        | import    | in       | is       | lambda   |
| nonlocal  | not       | or       | pass     | raise    |
| return    | try       | while    | with     | yield    |

---

# Python Built-in Functions Table
This table contains a list of **Python’s built-in functions**, neatly arranged into columns for quick reference.

| Col 1         | Col 2          | Col 3            | Col 4           | Col 5          |
| ------------- | -------------- | ---------------- | --------------- | -------------- |
| `abs()`       | `all()`        | `any()`          | `bin()`         | `bool()`       |
| `bytearray()` | `callable()`   | `chr()`          | `classmethod()` | `compile()`    |
| `complex()`   | `delattr()`    | `dict()`         | `dir()`         | `divmod()`     |
| `enumerate()` | `eval()`       | `exec()`         | `filter()`      | `float()`      |
| `format()`    | `frozenset()`  | `getattr()`      | `globals()`     | `hasattr()`    |
| `hash()`      | `help()`       | `hex()`          | `id()`          | `input()`      |
| `int()`       | `isinstance()` | `issubclass()`   | `iter()`        | `len()`        |
| `list()`      | `locals()`     | `map()`          | `max()`         | `memoryview()` |
| `min()`       | `next()`       | `object()`       | `oct()`         | `open()`       |
| `ord()`       | `pow()`        | `print()`        | `property()`    | `range()`      |
| `repr()`      | `reversed()`   | `round()`        | `set()`         | `setattr()`    |
| `slice()`     | `sorted()`     | `staticmethod()` | `str()`         | `sum()`        |
| `super()`     | `tuple()`      | `type()`         | `vars()`        | `zip()`        |

---

# Python Built-in Types Table
This table contains **Python’s built-in types**, neatly arranged into columns for quick reference.

| Col 1      | Col 2   | Col 3       | Col 4       |
| ---------- | ------- | ----------- | ----------- |
| `int`      | `float` | `complex`   | `bool`      |         
| `list`     | `tuple` | `set`       | `frozenset` |        
| `NoneType` | `bytes` | `bytearray` | `range`     |  
| `object`   | `str`   |  `dict`     | `memoryview`|              

---

## 🔹 Why are there both `set` and `set()` in Python?

The **names** like `set`, `str`, `int`, etc., are **built-in types** in Python. But when you write `set()` or `str()`, you're **calling the constructor** of that type — i.e., creating an instance of that type.

---

### ✅ Think of it this way:

| Type Name | Used As  | Meaning                           |
| --------- | -------- | --------------------------------- |
| `int`     | `int()`  | Creates an integer (default is 0) |
| `str`     | `str()`  | Creates an empty string `""`      |
| `list`    | `list()` | Creates an empty list `[]`        |
| `set`     | `set()`  | Creates an empty set `set()`      |
| `dict`    | `dict()` | Creates an empty dictionary `{}`  |

---

So in Python:

* `int` is the **type**
* `int()` is calling its **constructor**
* Both refer to the same underlying thing — the **type object**, but the usage differs.

---

### ⚠️ Bonus:

You can check their identity:

```python
type(5) == int        # True
isinstance("hello", str)  # True
```

---
Here’s a **mini-hint summary (Markdown)** version of your `🧠 Python Functions` content, styled like your **Keywords / Built-in / Types** tables for your `py_fun.md`:

---

# 🧠 Python Functions – Quick Reference

This section provides a **quick and structured overview** of Python function concepts for fast interview revision.

---

## 📦 Types of Function Arguments

| Type            | Syntax / Example                   | Use Case                  |
| --------------- | ---------------------------------- | ------------------------- |
| Positional      | `func(a, b)`                       | Basic fixed-order inputs  |
| Keyword         | `func(x=10, y=20)`                 | Specifying by name        |
| Default         | `def greet(name="Guest")`          | Provide fallback          |
| Variable-length | `*args`, `**kwargs`                | Accept flexible arguments |
| Mixed           | `def mix(a, b=0, *args, **kwargs)` | Combine types             |

---

## 🧠 Higher-Order Functions

Functions that take other functions as input/output:

| Function           | Description                           |
| ------------------ | ------------------------------------- |
| `map()`            | Apply a function to each element      |
| `filter()`         | Filter elements via condition         |
| `reduce()`         | Accumulate result (needs `functools`) |
| `sorted(key=func)` | Sort using custom logic               |

---

## 🌍 Scope Rules (LEGB)

| Level     | Meaning                       |
| --------- | ----------------------------- |
| Local     | Inside current function       |
| Enclosing | Outer function                |
| Global    | Top-level of script/module    |
| Built-in  | Python defaults (`len`, etc.) |

---
