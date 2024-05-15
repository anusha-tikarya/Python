##  DICTONARIES
Dictionaries in Python are a powerful data structure used to store collections of key-value pairs. Each key in a dictionary must be unique, and it's used to access its corresponding value. Dictionaries are mutable, meaning they can be modified after creation. Here's a bit more detail on dictionaries and their functions:

1. **Creating a Dictionary**:
   
   You can create a dictionary by enclosing a comma-separated list of key-value pairs within curly braces `{}`. Each key is separated from its value by a colon `:`.

   ```python
   my_dict = {"name": "John", "age": 30, "city": "New York"}
   ```

2. **Accessing Values**:

   You can access the value associated with a particular key using square brackets `[]` and providing the key.

   ```python
   print(my_dict["name"])  # Output: John
   ```

3. **Adding or Modifying Elements**:

   You can add new key-value pairs or modify existing ones.

   ```python
   my_dict["email"] = "john@example.com"  # Adding a new key-value pair
   my_dict["age"] = 31  # Modifying an existing value
   ```

4. **Removing Elements**:

   You can remove elements from a dictionary using the `del` keyword or the `pop()` method.

   ```python
   del my_dict["city"]  # Removing a key-value pair
   popped_value = my_dict.pop("age")  # Removing and returning the value associated with a key
   ```

5. **Getting Keys and Values**:

   You can retrieve all keys or values from a dictionary using the `keys()` and `values()` methods, respectively.

   ```python
   keys = my_dict.keys()
   values = my_dict.values()
   ```

6. **Iterating Over a Dictionary**:

   You can iterate over a dictionary using a `for` loop to access its keys or key-value pairs.

   ```python
   for key in my_dict:
       print(key, my_dict[key])
   ```

7. **Checking Membership**:

   You can check if a key exists in a dictionary using the `in` operator.

   ```python
   if "name" in my_dict:
       print("Name exists in the dictionary.")
   
   ```
8. **get**
```python
# Define a dictionary
person = {"name": "Alice", "age": 30, "city": "New York"}

# Accessing values using keys
name = person["name"]
age = person.get("age")

print("Name:", name)  # Output: Alice
print("Age:", age)    # Output: 30
```

In this example:
- We have a dictionary `person` with keys `"name"`, `"age"`, and `"city"`.
- We access the values associated with keys `"name"` and `"age"` using square brackets `[]` and the `get()` method, respectively.
- Assigning these values to variables allows us to work with them in the program.
Dictionaries are incredibly useful for tasks like storing settings, representing complex data structures, and much more. They provide a convenient way to organize and manipulate data in Python.

