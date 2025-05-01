# <center> JSON?
JavaScript Object Notation  
Lightweight data format used for storing & exchanging data.  
Works across all programming languages  
Most APIs (especially REST APIs) use JSON as the standard format

---
**SYNTAX**  
- Data is in key-value pairs  
- Keys and strings are enclosed in double quotes  
- Data is separated by commas  
- Curly braces { } represent objects  
- Square brackets [ ] represent arrays

```JSON
{
  "device": "temperature_sensor",
  "value": 23.7,
  "timestamp": "2025-05-01T14:30:00Z"
}

This can be written same as dictionary in python
```
---
**PYTHON**  
Python has a built-in package called json, which can be used to work with JSON data.


```python
# json to python
import json
x =  '{ "name":"John", "age":30, "city":"New York"}'

# json -> dictionary and storing in y
y = json.loads(x)
print(y["age"])
```

```python
# python to json
import json
x = {
  "name": "John",
  "age": 30,
  "city": "New York"
}
y = json.dumps(x)
print(y)