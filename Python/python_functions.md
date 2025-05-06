# 🧠 Python Functions

Functions in Python allow you to **encapsulate code** for reuse, modularity, and better organization.

---

## ✅ Function Definition and Syntax

```python
# Basic function
def greet(name):
    print("Hello", name)
```

---

## 🔙 Return Values

```python
# Function with return
def add(x, y):
    return x + y

result = add(3, 4)  # returns 7
```

---

## 📥 Function Arguments

### 1. **Positional Arguments**

```python
def subtract(a, b):
    return a - b

subtract(10, 5)  # 5
```

### 2. **Keyword Arguments**

```python
def full_name(first, last):
    return f"{first} {last}"

full_name(last="Doe", first="John")
```

### 3. **Default Arguments**

```python
def power(base, exponent=2):
    return base ** exponent

power(3)       # 9
power(3, 3)    # 27
```

### 4. **Variable-Length Arguments (`*args`, `**kwargs`)**

```python
# *args: accepts any number of positional arguments
def total_sum(*args):
    return sum(args)

total_sum(1, 2, 3, 4)  # 10

# **kwargs: accepts any number of keyword arguments
def display_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

display_info(name="Alice", age=25)
```

---

## 🔁 Higher-Order Functions

Functions that take other functions as arguments or return functions.

```python
def shout(text):
    return text.upper()

def whisper(text):
    return text.lower()

def greet(func, name):
    return func(name)

greet(shout, "hello")  # 'HELLO'
```

---

## ⚡ Lambda (Anonymous) Functions

```python
# Syntax: lambda arguments: expression
square = lambda x: x * x
print(square(5))  # 25
```

---

## 🔧 Built-in Functional Tools

| Function   | Description                                   | Example                             |
| ---------- | --------------------------------------------- | ----------------------------------- |
| `map()`    | Applies a function to all items in iterable   | `map(str.upper, ["a", "b"])`        |
| `filter()` | Filters items using a condition               | `filter(lambda x: x > 5, [1, 6])`   |
| `reduce()` | Applies rolling computation (via `functools`) | `reduce(lambda x, y: x+y, [1,2,3])` |
| `all()`    | Returns True if all are True                  | `all([True, True])`                 |
| `any()`    | Returns True if any are True                  | `any([False, True])`                |

```python
from functools import reduce
print(list(map(lambda x: x*2, [1, 2, 3])))       # [2, 4, 6]
print(list(filter(lambda x: x % 2 == 0, [1, 2]))) # [2]
print(reduce(lambda a, b: a + b, [1, 2, 3]))     # 6
```

---

## 🔄 Nested Functions

```python
def outer():
    print("Outer")

    def inner():
        print("Inner")

    inner()

outer()
```

---

## 🔁 Recursive Functions

```python
def factorial(n):
    if n == 1:
        return 1
    return n * factorial(n - 1)

factorial(5)  # 120
```

---

## 🌍 Scope and Lifetime

| Scope Type | Description                              |
| ---------- | ---------------------------------------- |
| Local      | Defined inside function                  |
| Global     | Defined outside all functions            |
| Enclosing  | Outer function in nested functions       |
| Built-in   | Python built-ins like `len()`, `print()` |

```python
x = "global"

def outer():
    x = "enclosing"
    def inner():
        x = "local"
        print(x)
    inner()

outer()  # local
```

---

## 📦 Function Annotations (Optional Type Hints)

```python
def add(a: int, b: int) -> int:
    return a + b
```

---

## 🧩 Full Function Structure Template

```python
def function_name(param1: type = default, *args, **kwargs) -> return_type:
    """
    Optional docstring
    """
    # logic here
    return something
```

---

## ✅ Summary Table

| Feature             | Example                | Use Case                      |
| ------------------- | ---------------------- | ----------------------------- |
| Regular func        | `def my_func():`       | Basic reusable code block     |
| Lambda              | `lambda x: x*2`        | Small one-liner functions     |
| \*args / \*\*kwargs | `*args`, `**kwargs`    | Flexible arguments            |
| Higher-order        | `map(func, list)`      | Pass/return functions         |
| Recursion           | `func(n-1)`            | Loop-like logic via self-call |
| Annotations         | `def f(x: int) -> str` | Type hinting for clarity      |

---