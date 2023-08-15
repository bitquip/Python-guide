## 11. Advanced Topics (Optional)

Welcome to the **Advanced Topics** section! In this section, we'll briefly introduce you to some advanced Python concepts that you can explore as you become more comfortable with the language.

### Decorators

Decorators are a powerful feature in Python that allow you to modify or enhance the behavior of functions or methods.

```python
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")

say_hello()
```

### Generators

Generators are a memory-efficient way to iterate over large datasets. They allow you to create iterators without loading the entire dataset into memory.

```python
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        yield a
        a, b = b, a + b

fib = fibonacci(10)
for num in fib:
    print(num)
```

### Context Managers

Context managers are used to manage resources like files, network connections, or databases. They ensure proper setup and cleanup.

```python
with open("file.txt", "r") as file:
    content = file.read()

# File is automatically closed outside the "with" block
```

These advanced topics can significantly enhance your Python skills. Remember, practice and exploration are key to becoming a proficient Python developer. Congratulations, you've completed the Python onboarding tutorial! You're now well-equipped to contribute effectively to projects at [Your Company Name]. Happy coding!