## 7. Modules and Packages

Welcome to the **Modules and Packages** section! In this section, we'll explore how to organize your code using modules and packages, and how to leverage external libraries.

### Importing Modules

Python has a rich standard library with built-in modules that provide various functionalities. You can import and use these modules in your code.

```python
# Importing the math module
import math

# Using functions from the math module
sqrt = math.sqrt(25)  # Calculates the square root of 25
```

### Creating Your Own Module

You can create your own Python modules to organize and reuse your code. Save the following code as `my_module.py`:

```python
# my_module.py
def say_hello():
    print("Hello from my_module!")
```

Then, in another file, you can import and use this module:

```python
# Importing and using the my_module module
import my_module

my_module.say_hello()  # Outputs: Hello from my_module!
```

### Exploring Packages

Packages are collections of related modules. They help organize code into meaningful hierarchies.

```plaintext
my_package/
├── __init__.py
├── module1.py
└── module2.py
```

In this example, `my_package` is a package containing two modules, `module1` and `module2`.

### Using External Packages

Python has a vast ecosystem of third-party packages that can greatly enhance your projects. You can install external packages using tools like `pip`.

```bash
pip install package_name
```

For example, to install the popular `requests` package:

```bash
pip install requests
```

Then, you can import and use it in your code:

```python
import requests

response = requests.get("https://www.example.com")
```

In the next section, we'll explore how to work with files in Python. If you're ready, let's proceed!