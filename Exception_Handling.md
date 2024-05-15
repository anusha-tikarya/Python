### What is Error Handling?

Error handling is the process of managing errors that occur while a program runs, preventing it from crashing and handling issues gracefully.

### Why Use Error Handling?

1. **Prevent Crashes**: Keep the program running even when errors happen.
2. **User-Friendly**: Show helpful error messages to users.
3. **Debugging**: Identify and fix where errors occur.
4. **Resource Management**: Ensure resources like files are properly closed.

### Basic Syntax

Python uses `try`, `except`, `else`, and `finally` blocks:

- **try**: Code that might cause an error.
- **except**: Code that runs if an error occurs.
- **else**: Code that runs if no errors occur.
- **finally**: Code that always runs, used for cleanup.

### Example

```python
try:
    # Code that may raise an exception
    num = int(input("Enter a number: "))
    result = 10 / num
    print("The result is", result)
except ValueError:
    # Handles invalid number input
    print("That's not a valid number!")
except ZeroDivisionError:
    # Handles division by zero
    print("You can't divide by zero!")
else:
    # Runs if no exceptions occur
    print("Operation completed successfully.")
finally:
    # Always runs, used for cleanup
    print("End of program.")
```

### How It Works

1. **try block**: Tries to execute the code.
2. **except blocks**: Catch and handle specific errors.
3. **else block**: Runs if no errors occur.
4. **finally block**: Runs no matter what, for cleanup tasks.

### Use Case Example

Handling user input:

```python
try:
    age = int(input("Enter your age: "))
except ValueError:
    print("Please enter a valid number.")
else:
    print(f"Your age is {age}.")
```

This example catches invalid input and asks the user to enter a valid number.

### Conclusion

Error handling helps create stable and user-friendly programs by managing unexpected issues gracefully using `try`, `except`, `else`, and `finally` blocks.
