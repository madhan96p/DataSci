### ➕🧮 **Python Arithmetic Operations**

Python supports a wide range of arithmetic operations on numbers (integers, floats, etc.). These operators can also work with complex numbers and support type conversion.

---

#### 📌 **Basic Arithmetic Operators**

| Operator       | Symbol | Example   | Output | Description                   |
| -------------- | ------ | --------- | ------ | ----------------------------- |
| Addition       | `+`    | `5 + 3`   | `8`    | Adds two numbers              |
| Subtraction    | `-`    | `10 - 4`  | `6`    | Subtracts right from left     |
| Multiplication | `*`    | `6 * 3`   | `18`   | Multiplies numbers            |
| Division       | `/`    | `10 / 2`  | `5.0`  | Returns float division result |
| Floor Division | `//`   | `10 // 3` | `3`    | Discards decimal part         |
| Modulus        | `%`    | `10 % 3`  | `1`    | Remainder after division      |
| Exponent       | `**`   | `2 ** 3`  | `8`    | Raises to the power           |

---

#### 🔁 **Operator Precedence (Order of Evaluation)**

| Priority | Operator(s)         | Description                          |
| -------- | ------------------- | ------------------------------------ |
| 1        | `()`                | Parentheses                          |
| 2        | `**`                | Exponent                             |
| 3        | `+`, `-` (Unary)    | Positive/Negative sign               |
| 4        | `*`, `/`, `//`, `%` | Multiplication, division, floor, mod |
| 5        | `+`, `-`            | Addition, subtraction                |

🔹 Example:

```python
result = 5 + 2 * 3 ** 2  # Output: 23
# 3**2 = 9 → 2*9 = 18 → 5+18 = 23
```

---

#### 🔄 **Type Conversion in Arithmetic**

| Expression    | Result Type     |
| ------------- | --------------- |
| `int + int`   | `int`           |
| `int + float` | `float`         |
| `float / int` | `float`         |
| `5 // 2`      | `int` (`2`)     |
| `5 / 2`       | `float` (`2.5`) |

---
