## Unpacking /Destructing
Unpacking, also known as destructuring, is a feature in Python that allows you to assign the elements of a tuple or list to individual variables. It's particularly useful when you want to extract values from iterables like tuples or lists quickly.

### Unpacking in Tuples:

```python
# Tuple
person = ("Alice", 30, "New York")

# Unpacking tuple into variables
name, age, city = person

print(name)  # Output: Alice
print(age)   # Output: 30
print(city)  # Output: New York
```

In the above example, `name`, `age`, and `city` are individual variables that receive values from the `person` tuple through unpacking.

### Use of Underscore (_) in Unpacking:

```python
# Tuple with unused values
person = ("Alice", 30, "New York", "555-1234")

# Unpacking tuple into variables, ignoring phone number
name, age, city, _ = person

print(name)  # Output: Alice
print(age)   # Output: 30
print(city)  # Output: New York
```

Here, the underscore `_` is used as a placeholder for the value we don't want to use or care about during unpacking.

### Unpacking in Lists:

```python
# List
numbers = [1, 2, 3]

# Unpacking list into variables
first, second, third = numbers

print(first)   # Output: 1
print(second)  # Output: 2
print(third)   # Output: 3
```

### Use of Star (*) in Unpacking:

```python
# List with multiple values
numbers = [1, 2, 3, 4, 5]

# Unpacking list into variables, with * to capture remaining values
first, *rest = numbers

print(first)  # Output: 1
print(rest)   # Output: [2, 3, 4, 5]
```

In this example, `*rest` collects all remaining values from the list after assigning the first value to `first`.

Unpacking is a convenient way to work with collections of data, allowing you to access individual elements quickly and easily

## ------------------------------------------------------------

![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/01618c32-90cd-483a-9da2-1a4f2178f2f9)

![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/fcc09729-03b2-4a77-b7a4-ec49b2a23d01)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/78cb8242-7076-4003-ab5b-a2f92908df32)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/7f74b217-fd14-44ab-b176-7ea54133ded5)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/9c2f779a-9ed7-4bdd-8ca2-b23be33e352b)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/db4b5d09-cfb5-432c-bb6b-358bea094339)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/de19b352-e14f-4307-b888-f4faf1831ece)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/2aca959a-f31c-447f-8d46-4bd3d03b1562)

# Unpacking -> ** Dict
movie = {"name": "John wick", "year": 2014}
 
# Copy
mv1 = {**movie, "actor": "Keanu Reeves"}
mv2 = {**movie, "actor": "Keanu Reeves", "year": 2015}
mv3 = {"actor": "Keanu Reeves", "year": 2015, **movie}
print(mv1)
print(mv2)
print(mv3)
print(movie)


# Task1 : After 1 experience
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/89dbbf8c-6a7b-463f-a026-2a8177789caf)

```python
employees = [
    {"name": "Sneha", "experience": 2},
    {"name": "Manju"},
    {"name": "Sai Subash", "experience": 4},
    {"name": "Manasa"},
]
``` 
 Output
```python 
[
    {"name": "Sneha", "experience": 3},
    {"name": "Manju",  "experience": 1},
    {"name": "Sai Subash", "experience": 5},
    {"name": "Manasa", "experience": 1},
]
```

## Code

```python
for employee in employees:
    employee["experience"]=employee.get("experience",0)+1
print(employees)
```

# Task 2
#  Senior 5 or more, Mid-Level 3 to 5, Junior < 3
Output
```python
[
    {"name": "Sneha", "experience": 3, "status": "Mid-Level"},
    {"name": "Manju", "experience": 1, "status": "Junior"},
    {"name": "Sai Subash", "experience": 5, "status": "Senior"},
    {"name": "Manasa", "experience": 1, "status": "Junior"},
]
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/4ebe28af-e5b7-4c43-a010-2504ae2ea0d0)
(Way of writing in between)
```
## code
```python
for i in employees:
    i["experience"] = i.get("experience",0) + 1
 
    if i.get("experience") >= 5:
        i["status"] = "senior"
    elif i.get("experience") >= 3:
        i["status"] = "mid level"
    else:
        i["status"] = "junior"
print(employees)
```
## Function
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/966d4652-f95f-489f-b8e7-e478103c8e36)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/6fd68cf0-6c25-45d4-a7b6-bc7937fcaecc)

Functions in Python allow you to encapsulate a block of code that can be reused throughout your program. They help in organizing your code, making it more readable, maintainable, and modular. Here's a simple example:

```python
# Define a function to greet a user
def greet_user(name):
    """Function to greet a user by name."""
    print("Hello, " + name + "!")

# Call the function
greet_user("Alice")
greet_user("Bob")
```

In this example:

- We define a function called `greet_user` that takes one parameter `name`.
- Inside the function, it prints a greeting message using the provided name.
- We call the `greet_user` function twice with different names ("Alice" and "Bob").

Functions can take multiple parameters, perform calculations, manipulate data, and return results as needed. They are fundamental building blocks in Python programming and are used extensively in all sorts of applications.

## PARAMETER AND ARGUMENT
```python
#Parameter: name
def greet_user(name):
    print("Hello, " + name + "!")

#Argument: "Alice"
greet_user("Alice")
```

![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/d6ca3aeb-05d9-400e-8707-033e7da23c9a)
here parameter are a & b and values we will provide in the place of a , b are arguments like 8 ,10
and every time we call function (add (_ ,_) ) is function calling .

## DEFAULT VALUE IN FUNCTION
Default parameter values in Python allow you to define a default value for a parameter in a function. If the function is called without providing a value for that parameter, it will use the default value instead. Here's an example with a driving test scenario:

```python
def take_driving_test(name, age, car='sedan'):
    """Function to simulate taking a driving test."""
    print(f"{name}, aged {age}, is taking the driving test with a {car}.")

# Calling the function without specifying the car
take_driving_test("Alice", 20)

# Calling the function with a specified car
take_driving_test("Bob", 22, "SUV")
```

In this example:

- The function `take_driving_test` has three parameters: `name`, `age`, and `car` (with a default value of `'sedan'`).
- When the function is called without providing a value for `car`, it uses the default value.
- The first call to `take_driving_test` only provides values for `name` and `age`, so `car` defaults to `'sedan'`.
- The second call to `take_driving_test` provides values for all three parameters, so the default value for `car` is overridden.

The main difference is that default parameter values allow you to specify a default value for a parameter, which is used when the function is called without providing a value for that parameter. This provides flexibility and convenience when calling the function, as you can choose to override the default value if needed.

## Types Of Argument:

In Python, there are two types of arguments that can be passed to a function: positional arguments and keyword arguments.

1. **Positional Arguments**:(FIRST)
   - Positional arguments are passed to a function based on their position or order in the function call.
   - They are defined in the function signature in the order they are expected to be received.
   - When calling the function, you must provide values for these arguments in the same order.

Example:
```python
def greet(name, age):
    print(f"Hello, {name}! You are {age} years old.")

# Positional arguments: "Alice" and 25
greet("Alice", 25)
```

2. **Keyword Arguments**:(LAST)
   - Keyword arguments are passed with a keyword and a corresponding value.
   - They are not dependent on the order in which they are passed, as long as their keyword matches the parameter name in the function signature.
   - Keyword arguments are useful when you want to specify only certain arguments and leave the others with their default values, or when the order of the arguments is not obvious.

Example:
```python
# Keyword arguments: age=30 and name="Bob"
greet(age=30, name="Bob")
```

In summary, positional arguments are passed based on their position in the function call, while keyword arguments are passed with explicit keyword-value pairs, allowing flexibility and clarity, especially when dealing with functions with many parameters.


# Task 1

**Add Book Function: Write a function add_book(library, new_book)**

![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/0b285ed3-9a29-4c88-82ce-df074395c1ac)

TASK-1
```python
def add_book(library_list,book):
    library_list.append(book)
    return library_list
print(add_book(library_list,book))
```

# Task 2

 **Search Books by Author Function: Write a function search_by_author(library, author_name)**
 
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/95199aa8-2e89-44a4-95ad-23309729b529)

TASK-2
```python
def search_book(library_list,author_name):
    for book in library_list:
        if(book["author"]==author_name):
            print(book)
print(search_book(library_list,"Mark Lutz"))
```

# Task 3
 **Check Out Book Function: Write a function check_out_book(library, title) that marks a book as not available if it exists and is available in the library.**
**1. Book available**
**2. Book unavailable**
 **3. Book doesn't exists**
 ![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/2541d858-e950-4a9f-b0e1-c74714671c7a)


## ways to end a function:
In Python, there are two common ways to end a function:

1. **Using the `return` statement**:
   - The `return` statement is used to exit a function and return a value (if any) back to the caller.
   - It can be used anywhere within the function to exit prematurely.
   - If a `return` statement is not explicitly included in a function, the function will implicitly return `None` when it reaches the end.

Example:
```python
def add(a, b):
    return a + b
```

2. **Reaching the end of the function block**:
   - If no `return` statement is encountered during the execution of a function, or if the function block ends without encountering a `return` statement, the function will implicitly return `None`.
   - This happens when the function block executes all its statements without encountering a `return` statement.

Example:
```python
def greet(name):
    print("Hello, " + name + "!")
    # No return statement
```

Both ways are valid and can be used based on the requirements of the function. The choice depends on whether the function needs to return a value or not.
## =======================================================
def own_max(*nums):
    print(nums, type(nums))
 
 
own_max(5, 6, 10)
own_max(5, 6, 10, 7, 80, 60)

 
def own_max(*nums):
    # Implement max logic
    print(nums, type(nums))
 
 
own_max(5, 6, 10)
own_max(5, 6, 10, 7, 80, 60)


 ```python
def own_max(*nums):
     max = nums[0]
     for num in nums:
          if num > max:
               max = num
     return max
```
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/2ac3f9a9-e297-45ba-8f91-4c00435b80c5)

