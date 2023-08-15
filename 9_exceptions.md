## 9. Exception Handling

Welcome to the **Exception Handling** section! In this section, we'll learn how to handle errors using exception handling.

### Handling Exceptions

Exception handling allows you to gracefully handle errors that may occur during the execution of your code.

```python
try:
    result = 10 / 0  # Division by zero
except ZeroDivisionError:
    print("Cannot divide by zero.")
```

### The `finally` Block

The `finally` block is used to execute code that should run regardless of whether an exception occurred or not.

```python
try:
    # Code that might raise an exception
except SomeException:
    # Handle the exception
finally:
    # This block will execute regardless
```

### Raising Exceptions

You can raise exceptions using the `raise` keyword when a certain condition isn't met.

```python
age = -5

if age < 0:
    raise ValueError("Age cannot be negative.")
```

Exception handling is crucial for writing robust code that can handle unexpected situations. In the next section, we'll explore the world of object-oriented programming (OOP) in Python. If you're ready, let's proceed!