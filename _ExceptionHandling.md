# <center> EXCEPTION HANDLING

The `try` block lets you test a block of code for errors.  
The `except` block lets you handle the error.  
The `else` block lets you execute code when there is no error.
The `finally` block lets you execute code, regardless of the result of the try- and except blocks.


```PYTHON
try:
  print("Hello")
except:
  print("Something went wrong")
else:
  print("Nothing went wrong")
finally:
  print("The 'try except' is finished")
```
To throw (or raise) an exception, use the `raise` keyword.

```PYTHON
x = -1
if x < 0:
  raise Exception("Sorry, no numbers below zero")
```