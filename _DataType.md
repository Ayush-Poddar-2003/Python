# Built-in Data Types

1. Numeric Types   :	int, float, complex

```python
a = 10
print(type(a))  # <class 'int'>
b = 3.14
print(type(b))  # <class 'float'>
c = 2 + 3j
print(type(c))  # <class 'complex'>
```


2. Text Type       :	str (no char in python)

```python
name = "Ayush"
print(type(name))  # <class 'str'>
```

4. Boolean Type    :	bool
```python
is_active = True
print(type(is_active))  # <class 'bool'>

```


5. Sequence Types  :	list[], tuple(), range()
```python
fruits = ["apple", "banana", "cherry"]
print(type(fruits))  # <class 'list'>

coordinates = (4, 5)
print(type(coordinates))  # <class 'tuple'>

numbers = range(5)
print(type(numbers))  # <class 'range'>
```

6. Mapping Type    :	dict{key:value}
```python
person = {"name": "Ayush", "age": 21}
print(type(person))  # <class 'dict'>
```
7. Set Types       :	set{}, frozenset
```python
unique_numbers = {1, 2, 3}
print(type(unique_numbers))  # <class 'set'>

# Immutable version of set
fset = frozenset([1, 2, 3])
print(type(fset))  # <class 'frozenset'>
```
1. Binary Types    :	bytes, bytearray, memoryview
```python
x = b"hello"
print(type(x))  # <class 'bytes'>

y = bytearray(5)
print(type(y))  # <class 'bytearray'>

z = memoryview(bytes(5))
print(type(z))  # <class 'memoryview'>
```
1. None Type       :	NoneType
```python

```

