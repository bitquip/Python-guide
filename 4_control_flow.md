## 4. Control Flow

Welcome to the **Control Flow** section! Here, we'll learn how to make decisions and repeat tasks using conditional statements and loops.

### Conditional Statements

Conditional statements allow your program to make decisions based on conditions. The `if`, `elif`, and `else` keywords are used for this purpose.

```python
age = 18

if age < 18:
    print("You are a minor.")
elif age >= 18 and age < 60:
    print("You are an adult.")
else:
    print("You are a senior citizen.")
```

### Loops

Loops are used to execute a block of code repeatedly. Python offers two main types of loops: `for` loops and `while` loops.

#### For Loop

```python
# Printing numbers from 0 to 4
for i in range(5):
    print(i)
```

#### While Loop

```python
age = 20
while age < 30:
    print("Age:", age)
    age += 1
```

### Break and Continue

You can use `break` to exit a loop prematurely and `continue` to skip the rest of the current iteration and proceed to the next one.

```python
for i in range(10):
    if i == 5:
        break     # Exit the loop when i is 5
    print(i)
```

```python
for i in range(10):
    if i % 2 == 0:
        continue  # Skip even numbers
    print(i)
```

Understanding control flow is crucial for building complex programs. In the next section, we'll explore functions, which allow you to group code for reuse. If you're ready, let's proceed!

<br>

<div style="display: flex; justify-content: space-between; align-items: center;">
    <a href="https://bitquip.github.io/.NET-TDD/3_syntax_datatypes" style="margin: 10px; text-decoration: none;">← Syntax</a>
    <span style="margin: 10px;"></span>
    <a href="https://bitquip.github.io/.NET-TDD/5_functions" style="margin: 10px; text-decoration: none;">Functions →</a>
</div>
