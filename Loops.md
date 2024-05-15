## LOOPS
In Python, loops are used to iterate over a sequence of elements or perform a block of code repeatedly. There are mainly two types of loops in Python: `for` loops and `while` loops.

1. **For Loops**:

   For loops are used to iterate over a sequence (such as a list, tuple, string, or range) or any iterable object.

   ```python
   for item in sequence:
       # do something with item
   ```

   Example:

   ```python
   fruits = ["apple", "banana", "cherry"]
   for fruit in fruits:
       print(fruit)
   ```

   Output:
   ```
   apple
   banana
   cherry
   ```

2. **While Loops**:

   While loops are used to execute a block of code repeatedly as long as a specified condition is true.

   ```python
   while condition:
       # do something
   ```

   Example:

   ```python
   count = 0
   while count < 5:
       print(count)
       count += 1
   ```

   Output:
   ```
   0
   1
   2
   3
   4
   ```

3. **Loop Control Statements**:

   - **Break**: Terminates the loop prematurely.
   
     ```python
     for i in range(5):
         if i == 3:
             break
         print(i)
     ```

   - **Continue**: Skips the rest of the code inside the loop for the current iteration and continues with the next iteration.
   
     ```python
     for i in range(5):
         if i == 3:
             continue
         print(i)
     ```

   - **Pass**: Acts as a placeholder and does nothing. It is used when a statement is syntactically required but you want to do nothing.
   
     ```python
     for i in range(5):
         if i == 3:
             pass
         print(i)
     ```

Loops are fundamental in programming and are used extensively for various tasks like iterating over elements, implementing algorithms, and controlling program flow.

