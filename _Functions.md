# Python Functions



```python
def greet(name):
    print("Hello,", name)

greet("Ayush")  # Output: Hello, Ayush
```

```python
def add(a, b):
    return a + b

result = add(3, 4)
print(result)  # Output: 7
```

```python
def greet(name="Guest"):
    print("Hello,", name)

greet()          # Output: Hello, Guest
greet("Ayush")   # Output: Hello, Ayush
```

## 🧰 Built-in Functions

```python
print(len("Ayush"))      # 5
print(max(3, 5, 7))      # 7
print(min(2, 1))         # 1
print(abs(-5))           # 5
print(sum([1, 2, 3]))    # 6
```
## <center> Local vs Global Scope

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

## <center>Arbitrary Arguments (*args)

Use `*args` to pass a variable number of arguments (as a **tuple**):

```python
def add_numbers(*args):
    return sum(args)

print(add_numbers(1, 2, 3, 4))  # Output: 10
```

Use `**kwargs` to pass keyword arguments (as a dictionary):

```python
def profile(**kwargs):
    for key, value in kwargs.items():
        print(key, ":", value)

profile(name="Ayush", age=21)
```

---


## <center> Lambda Functions

Small anonymous functions with one expression.

```python
add = lambda x, y: x + y
print(add(5, 3))  # Output: 8
```


## <center> Docstrings

Documentation inside functions:

```python
def greet():
    """This function greets the user."""
    print("Hello!")

print(greet.__doc__)
```

