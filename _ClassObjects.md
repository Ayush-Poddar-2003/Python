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

---

### Instance vs Class Variables
```python
class Dog:
  species = "Canis familiaris"  # Class variable
  
  def __init__(self, name):
  self.name = name  # Instance variable

dog1 = Dog("Buddy")
dog2 = Dog("Max")

print(dog1.species)  # Canis familiaris
print(dog2.species)  # Canis familiaris
print(dog1.name)     # Buddy
print(dog2.name)     # Max
```
Class variables are shared by all instances.  
Instance variables are unique to each object