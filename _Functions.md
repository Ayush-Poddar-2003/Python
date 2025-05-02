# Python Functions

Functions are reusable blocks of code that perform a specific task. They help make programs more modular, readable, and organized.

---

## ✅ 1. Defining a Function

Use the `def` keyword:

```python
def greet():
    print("Hello, Ayush!")
```

---

## ▶️ 2. Calling a Function

```python
greet()  # Output: Hello, Ayush!
```

---

## 📥 3. Function with Parameters

```python
def greet(name):
    print("Hello,", name)

greet("Ayush")  # Output: Hello, Ayush
```

---

## 🧮 4. Function with Return Value

```python
def add(a, b):
    return a + b

result = add(3, 4)
print(result)  # Output: 7
```

---

## 🎯 5. Default Parameters

```python
def greet(name="Guest"):
    print("Hello,", name)

greet()          # Output: Hello, Guest
greet("Ayush")   # Output: Hello, Ayush
```

---

## 🔢 6. Arbitrary Arguments (*args)

Use `*args` to pass a variable number of arguments (as a tuple):

```python
def add_numbers(*args):
    return sum(args)

print(add_numbers(1, 2, 3, 4))  # Output: 10
```

---

## 🔠 7. Keyword Arguments (**kwargs)

Use `**kwargs` to pass keyword arguments (as a dictionary):

```python
def profile(**kwargs):
    for key, value in kwargs.items():
        print(key, ":", value)

profile(name="Ayush", age=21)
```

---

## 🧵 8. Scope: Local vs Global

```python
x = 10  # Global variable

def func():
    x = 5  # Local variable
    print(x)

func()     # 5
print(x)   # 10
```

Use `global` to modify a global variable:

```python
x = 10

def change():
    global x
    x = 20

change()
print(x)  # 20
```

---

## 🔁 9. Recursive Function

A function that calls itself:

```python
def factorial(n):
    if n == 1:
        return 1
    return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

---

## 💡 10. Lambda Functions

Small anonymous functions with one expression.

```python
add = lambda x, y: x + y
print(add(5, 3))  # Output: 8
```

---

## 🧰 11. Built-in Functions (Examples)

```python
print(len("Ayush"))      # 5
print(max(3, 5, 7))      # 7
print(min(2, 1))         # 1
print(abs(-5))           # 5
print(sum([1, 2, 3]))    # 6
```

---

## 🧪 12. Docstrings

Documentation inside functions:

```python
def greet():
    """This function greets the user."""
    print("Hello!")

print(greet.__doc__)
```

---

## 🧩 Summary

| Feature         | Example                              |
|----------------|--------------------------------------|
| Basic function  | `def my_func():`                    |
| With params     | `def add(a, b):`                    |
| Return value    | `return a + b`                      |
| *args           | `def myfunc(*args):`                |
| **kwargs        | `def myfunc(**kwargs):`             |
| Lambda          | `lambda x: x * 2`                   |
| Recursive       | `def fact(n): return n * fact(n-1)` |

---
