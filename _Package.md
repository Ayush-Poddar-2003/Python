What is a Package?  
A package is a collection of Python modules  
grouped in a directory with a special `__init__.py` file.

Why Use Packages?  
Organize code in large projects, Avoid naming conflicts, 
Reuse and share code easily, Create distributable libraries (e.g., pip install packages)

---
```bash
my_package/
│
├── __init__.py         # Makes this folder a package
├── greetings.py        # Module 1
└── calculations.py     # Module 2
```

📁 Inside Folder: my_package
```python
# greetings.py
def say_hello(name):
    return f"Hello, {name}!"
```
```python
#calculations.py
def add(a, b):
    return a + b
```

```python
# init.py
Can be empty / used to initialize package
```

---
Using the Package
```py
from my_package.greetings import say_hello
from my_package.calculations import add

print(say_hello("Ayush"))  # Hello, Ayush!
print(add(5, 3))            # 8
```