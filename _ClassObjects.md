# <CENTER>CLASS OBJECT
```PYTHON
class MyClass:
  x = 5

p1 = MyClass()
print(p1.x)
```
---
### _ _ init _ _ Function

All classes have a function called `__init__()`,  
which is always executed when the class is being initiated

```python
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age


p1 = Person("John", 36)
print(p1.name)
print(p1.age)
```
> The self parameter is a reference to the current instance of the class, and is used to access variables that belong to the class.  
> It does not have to be named self, you can call it whatever you like, but it has to be the first parameter of any function in the class:

```python
del p1.age
```