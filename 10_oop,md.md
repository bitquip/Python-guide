## 10. Object-Oriented Programming

Welcome to the **Object-Oriented Programming (OOP)** section! In this section, we'll dive into the concepts of OOP and how they're implemented in Python.

### Classes and Objects

Classes are blueprints for creating objects. Objects are instances of a class. OOP allows you to model real-world entities and their interactions in a program.

```python
# Creating a class
class Rectangle:
    def __init__(self, width, height):
        self.width = width
        self.height = height

    def area(self):
        return self.width * self.height
```

### Creating Objects

Once you've defined a class, you can create objects based on that class.

```python
# Creating an object
rect = Rectangle(5, 10)

# Calling methods on the object
area = rect.area()
print("Area:", area)
```

### Inheritance

Inheritance allows you to create a new class based on an existing class. The new class inherits attributes and behaviors from the parent class.

```python
# Creating a subclass
class Square(Rectangle):
    def __init__(self, side_length):
        super().__init__(side_length, side_length)

square = Square(7)
print("Square Area:", square.area())
```

### Encapsulation and Access Control

OOP provides mechanisms to control access to the internal attributes and methods of a class.

- Private attributes/methods are denoted by a leading underscore: `_private_attr`.
- Protected attributes/methods are denoted by a leading underscore: `_protected_attr`.

```python
class Student:
    def __init__(self, name, age):
        self._name = name       # Protected attribute
        self.__age = age        # Private attribute

    def _protected_method(self):
        pass

    def __private_method(self):
        pass
```

OOP allows you to create structured and modular code. In the final section, we'll touch on some advanced topics that you can explore on your own. If you're ready, let's proceed!

<br>

<div style="display: flex; justify-content: space-between; align-items: center;">
    <a href="https://bitquip.github.io/.NET-TDD/9_exceptions" style="margin: 10px; text-decoration: none;">← Exceptions</a>
    <span style="margin: 10px;"></span>
    <a href="https://bitquip.github.io/.NET-TDD/11_adv_intro" style="margin: 10px; text-decoration: none;">Advanced →</a>
</div>
