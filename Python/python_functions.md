# 🧠 Python Functions

Functions in Python allow you to **encapsulate code** for reuse, modularity, and better structure.

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

result = add(3, 4)  # 7
```

---

## 📥 Function Arguments

### 1️⃣ Positional Arguments

```python
def subtract(a, b):
    return a - b

subtract(10, 5)  # 5
```

### 2️⃣ Keyword Arguments

```python
def full_name(first, last):
    return f"{first} {last}"

full_name(last="Doe", first="John")
```

### 3️⃣ Default Arguments

```python
def power(base, exponent=2):
    return base ** exponent

power(3)       # 9
power(3, 3)    # 27
```

### 4️⃣ Variable-Length Arguments

#### A. `*args` — Accepts any number of positional arguments as a tuple

```python
def total_sum(*args):
    return sum(args)

total_sum(1, 2, 3, 4)  # 10
```

#### B. `**kwargs` — Accepts keyword arguments as a dictionary

```python
def display_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

display_info(name="Alice", age=25)
```

### 5️⃣ Keyword-Only Arguments

```python
def student(name, *, grade):
    print(f"{name} got grade {grade}")

student("Sara", grade="A")   # ✅
# student("Sara", "A")       # ❌ Error
```

---

## 🧪 Full Function with All Argument Types

```python
def demo(a, b=10, *args, c=20, **kwargs):
    print("a:", a)
    print("b:", b)
    print("args:", args)
    print("c:", c)
    print("kwargs:", kwargs)

demo(1, 2, 3, 4, 5, c=30, d=40, e=50)
```

### Output:

```
a: 1
b: 2
args: (3, 4, 5)
c: 30
kwargs: {'d': 40, 'e': 50}
```

---

## ✅ Argument Types Summary Table

| Argument Type | Description                            | Example           |
| ------------- | -------------------------------------- | ----------------- |
| Positional    | Ordered, based on position             | `f(1, 2)`         |
| Keyword       | Named arguments                        | `f(a=1, b=2)`     |
| Default       | Uses fallback if not provided          | `def f(x=10)`     |
| `*args`       | Variable positional (tuple)            | `def f(*args)`    |
| `**kwargs`    | Variable keyword (dict)                | `def f(**kwargs)` |
| Keyword-only  | Must be passed using keyword after `*` | `def f(*, x)`     |

---

## 🔁 Higher-Order Functions

Functions that take other functions as arguments or return them.

```python
def shout(text):
    return text.upper()

def greet(func, name):
    return func(name)

greet(shout, "hello")  # 'HELLO'
```

---

## ⚡ Lambda (Anonymous) Functions

```python
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
| `all()`    | True if all values are true                   | `all([True, True])`                 |
| `any()`    | True if at least one is true                  | `any([False, True])`                |

```python
from functools import reduce

print(list(map(lambda x: x*2, [1, 2, 3])))         # [2, 4, 6]
print(list(filter(lambda x: x % 2 == 0, [1, 2])))  # [2]
print(reduce(lambda a, b: a + b, [1, 2, 3]))       # 6
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

| Scope Type | Description                             |
| ---------- | --------------------------------------- |
| Local      | Defined inside function                 |
| Enclosing  | Outer function in nested structure      |
| Global     | Defined at module level                 |
| Built-in   | Python's built-in names (e.g., `print`) |

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

## ✅ Master Summary Table

| Feature             | Example                  | Description                    |
| ------------------- | ------------------------ | ------------------------------ |
| Regular Function    | `def my_func():`         | Reusable code block            |
| Lambda              | `lambda x: x*2`          | One-liner anonymous function   |
| `*args`, `**kwargs` | `def f(*args, **kwargs)` | Handle variable number of args |
| Higher-order        | `map(func, data)`        | Pass function as argument      |
| Recursion           | `func(n-1)`              | Function calling itself        |
| Annotation          | `def f(x: int) -> str`   | Type hinting                   |

---
