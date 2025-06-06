### 1. Conditional Statements (if, elif, else)

```python
x = 10

if x > 0:
    print("Positive")
elif x == 0:
    print("Zero")
else:
    print("Negative")
```

###  2. Loops
FOR LOOP -
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

for i in range(5):
    print(i)
```
WHILE LOOP -
```python
count = 0
while count < 5:
    print(count)
    count += 1
```
BREAK VS CONTINUE -
```python
for i in range(10):
    if i == 5:
        break #Exits the current loop immediately.
    print(i)
```
```python
for i in range(5):
    if i == 2:
        continue #Skips the rest of the current loop iteration.
    print(i)

```
```python
# when a statement is syntactically required but no action is needed.
for i in range(3):
    pass 
```

```python
command = "start"

match command:
    case "start":
        print("System starting")
    case "stop":
        print("System stopping")
    case _:
        print("Unknown command")
```