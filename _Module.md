What is a Module?  
A module is a Python file (.py) that contains functions, classes, or variables — designed to be reused in other programs.

Why Use Modules?  
Code reusability, 
Better organization (cleaner files), 
Easy collaboration, 
Built-in and third-party power tools

---
### 1. Built-in Modules
Pre-installed with Python,  
for eg math, datetime, random, os
```python
import math
print(math.sqrt(25))  # 5.0
```

---
### 2. User-defined Modules
customized .py files  

Create a file named mymodule.py
```python
# mymodule.py
def greet(name):
    return "Hello" + name
    
# In other file
import mymodule
print(mymodule.greet("Ayush"))  # Hello Ayush
```
---

### 3. External Modules
Installed using pip  
For eg numpy, requests, pandas
```bash
pip install pandas
```
```python

```

## <center> 
| Syntax                    | Description                         |
| ------------------------- | ----------------------------------- |
| `import module`           | Imports whole module                |
| `import module as alias`  | Use alias name                      |
| `from module import func` | Import specific item                |
| `from module import *`    | Import everything (not recommended) |
