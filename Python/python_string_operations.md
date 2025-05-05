### 📘 **Python String Operations**

---

#### 🔤 Basic Operations

| Operation         | Example             | Output / Explanation        |
| ----------------- | ------------------- | --------------------------- |
| Create string     | `s = "Hello World"` | Assign a string to variable |
| Indexing          | `s[0]`              | `'H'` – First character     |
| Negative Indexing | `s[-1]`             | `'d'` – Last character      |
| Slicing           | `s[0:5]`            | `'Hello'` – From index 0–4  |
| Reverse string    | `s[::-1]`           | `'dlroW olleH'`             |
| Length            | `len(s)`            | `11` – Total characters     |

---

#### 🔡 Case Modification

| Method     | Example          | Output          |
| ---------- | ---------------- | --------------- |
| Uppercase  | `s.upper()`      | `'HELLO WORLD'` |
| Lowercase  | `s.lower()`      | `'hello world'` |
| Title Case | `s.title()`      | `'Hello World'` |
| Capitalize | `s.capitalize()` | `'Hello world'` |

---

#### 🔍 Searching & Counting

| Method          | Example           | Output                  |
| --------------- | ----------------- | ----------------------- |
| Find substring  | `s.find("World")` | `6` – Start index       |
| Count letter    | `s.count("l")`    | `3` – Times 'l' appears |
| Check substring | `"World" in s`    | `True`                  |

---

#### 🔗 Joining & Splitting

| Method       | Example                     | Output               |
| ------------ | --------------------------- | -------------------- |
| Split string | `s.split()`                 | `['Hello', 'World']` |
| Join list    | `",".join(['A', 'B', 'C'])` | `'A,B,C'`            |

---

#### 🔁 Replace & Strip

| Method       | Example                        | Output           |
| ------------ | ------------------------------ | ---------------- |
| Replace text | `s.replace("World", "Python")` | `'Hello Python'` |
| Strip spaces | `"  Hello  ".strip()`          | `'Hello'`        |
| Left strip   | `"  Hello  ".lstrip()`         | `'Hello  '`      |
| Right strip  | `"  Hello  ".rstrip()`         | `'  Hello'`      |

---

#### ➕ Concatenation & Repetition

| Operation   | Example   | Output                     |
| ----------- | --------- | -------------------------- |
| Concatenate | `s + "!"` | `'Hello World!'`           |
| Repeat      | `s * 2`   | `'Hello WorldHello World'` |

---

#### 🧾 String Formatting

| Method      | Example                                            | Output                               |
| ----------- | -------------------------------------------------- | ------------------------------------ |
| f-string    | `f"Hi {name}, you are {age} years old."`           | `'Hi Madhan, you are 25 years old.'` |
| `.format()` | `"Hi {}, you are {} years old.".format(name, age)` | `'Hi Madhan, you are 25 years old.'` |

---

