## 12. Threading and Concurrency (Advanced)

Welcome to the **Threading and Concurrency** section! In this advanced section, we'll introduce you to threading, which allows your Python programs to handle multiple tasks concurrently.

### Understanding Threads

Threads are lightweight units of execution that allow programs to perform multiple tasks simultaneously. Python's `threading` module provides the tools to work with threads.

```python
import threading

def print_numbers():
    for i in range(1, 6):
        print("Number:", i)

def print_letters():
    for letter in 'abcde':
        print("Letter:", letter)

# Create two threads
thread1 = threading.Thread(target=print_numbers)
thread2 = threading.Thread(target=print_letters)

# Start the threads
thread1.start()
thread2.start()

# Wait for both threads to finish
thread1.join()
thread2.join()

print("Both threads have finished.")
```

### Global Interpreter Lock (GIL)

Python has a Global Interpreter Lock (GIL) that restricts the execution of multiple threads in a single process. This means that Python threads are not suitable for CPU-bound tasks, but they can be useful for I/O-bound tasks.

### Concurrent Futures

Python's `concurrent.futures` module provides a high-level interface for asynchronously executing functions using threads or processes.

```python
from concurrent.futures import ThreadPoolExecutor

def square(number):
    return number * number

numbers = [1, 2, 3, 4, 5]
with ThreadPoolExecutor() as executor:
    results = executor.map(square, numbers)

for result in results:
    print(result)
```

Keep in mind that threading introduces complexities like synchronization and potential race conditions. Consider using higher-level concurrency libraries like `asyncio` for more complex use cases.

Congratulations on reaching the end of this advanced section! You've now covered threading and concurrency in Python, which can greatly enhance the performance and efficiency of your programs.

With this knowledge, you're well-prepared to tackle a wide range of projects here at Vizient. 

Happy coding!


<br>

<div style="display: flex; justify-content: space-between; align-items: center;">
    <a href="https://bitquip.github.io/.NET-TDD/11_adv_intro" style="margin: 10px; text-decoration: none;">← Advanced</a>
    <span style="margin: 10px;"></span>
</div>
