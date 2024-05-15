## LIST
In Python, a list is a versatile data structure used to store a collection of items. It's mutable, meaning you can change its contents after creation. Here's an explanation of some common list functions:

1. **Append**: The `append()` method adds an element to the end of the list.

   ```python
   my_list = [1, 2, 3]
   my_list.append(4)
   print(my_list)  # Output: [1, 2, 3, 4]
   ```

2. **Remove**: The `remove()` method removes the first occurrence of a specified value from the list.

   ```python
   my_list = [1, 2, 3, 2]
   my_list.remove(2)
   print(my_list)  # Output: [1, 3, 2]
   ```

3. **Pop**: The `pop()` method removes and returns the element at the specified index (default is the last element).

   ```python
   my_list = [1, 2, 3]
   popped_element = my_list.pop(1)
   print(popped_element)  # Output: 2
   print(my_list)         # Output: [1, 3]
   ```

4. **Insert**: The `insert()` method inserts an element at a specified position in the list.

   ```python
   my_list = [1, 2, 3]
   my_list.insert(1, 5)
   print(my_list)  # Output: [1, 5, 2, 3]
   ```

5. **Extend**: The `extend()` method appends elements of an iterable (list, tuple, string, etc.) to the end of the list.

   ```python
   my_list = [1, 2, 3]
   my_list.extend([4, 5])
   print(my_list)  # Output: [1, 2, 3, 4, 5]
   ```

6. **Clear**: The `clear()` method removes all elements from the list.

   ```python
   my_list = [1, 2, 3]
   my_list.clear()
   print(my_list)  # Output: []
   ```

7. **Index**: The `index()` method returns the index of the first occurrence of a value in the list.

   ```python
   my_list = [1, 2, 3, 2]
   index = my_list.index(2)
   print(index)  # Output: 1
   ```

8. **Count**: The `count()` method returns the number of occurrences of a value in the list.

   ```python
   my_list = [1, 2, 3, 2]
   count = my_list.count(2)
   print(count)  # Output: 2
   ```

9. **Join** : The `join()` method in Python is actually a string method, not a list method. It joins the elements of a sequence (such as a list) into a string, using a specified delimiter.

```python
my_list = ["apple", "banana", "orange"]
delimiter = ", "
result = delimiter.join(my_list)
print(result)  # Output: "apple, banana, orange"
```

In this example, the elements of the `my_list` are joined into a single string with `,` and a space `, ` as the separator between each element. The `join()` method is called on the delimiter (`", "`), and the list to be joined is passed as an argument to this method.

It's important to note that `join()` works only on lists where all elements are strings. If there are non-string elements, you need to convert them to strings before using `join()`.


