## 8. File Handling

Welcome to the **File Handling** section! In this section, we'll learn how to work with files in Python, including reading and writing data.

### Reading from a File

Python provides various methods for reading data from files. The `with` statement ensures that the file is properly closed after usage.

```python
# Reading from a file
with open("data.txt", "r") as file:
    content = file.read()

print(content)
```

### Writing to a File

You can write data to a file using the `write()` method. Remember to specify the mode as `"w"` (write).

```python
# Writing to a file
with open("output.txt", "w") as file:
    file.write("This is some text.")
```

### Appending to a File

To add content to an existing file without overwriting it, open the file in append mode (`"a"`).

```python
# Appending to a file
with open("output.txt", "a") as file:
    file.write("\nThis text will be appended.")
```

In the next section, we'll delve into exception handling, which allows you to gracefully manage errors in your code. If you're ready, let's continue!