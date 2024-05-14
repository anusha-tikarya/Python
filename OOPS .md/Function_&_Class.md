## Functions 

### definig Function
  ```python
def function_name():# def stands for defining
    print("hii")
```

### Calling Funtion
  ```python
function_name() #hii
```
### Function Parameters
  ```python
def function_name(Para):
   print(f'hii {Para}')
function_name("Anusha")   # hii Anusha
```
### Function Return
  ```python
def sum(a,b):# def stands for defining
    return (a+b)

print(sum(1,3)) # 4
```
## Pip & Modules

### PIP (Python Package Installer):

- **What?** PIP is a package manager for Python.
- **Why?** It's used to install, upgrade, and manage Python packages.
- **Use?** Install packages with `pip install`, upgrade with `pip install --upgrade`, uninstall with `pip uninstall`, list installed packages with `pip list`.

### Modules in Python:

- **What?** Modules are Python files containing reusable code.
- **Why?** They help organize code and avoid naming conflicts.
- **Use?** Import modules with `import`, use functions/classes with dot notation.
- **Example?** `import math` and use `math.sqrt(4)` to calculate the square root of 4.

In essence, PIP helps manage external Python packages, while modules organize your own code for reuse.
## Class
### Introduction To Class

- **What?** A class is like a recipe or a blueprint that defines how to create objects in Python.
- **Why?** It helps keep code organized and makes it easier to reuse.
- **Encapsulation?** It's like putting your data and actions in a box, hiding them from outside interference.
- **Use?** You define a class using the `class` keyword, then create objects (instances) based on that class.
## Creating A Class & Object
- **Example:**
```python
  class Dog:
      def __init__(self, name, age):# __init__ is a default constructor
          self._name = name  # Encapsulation: using underscore to indicate it's a private variable
          self._age = age
      
      def bark(self):
          print(f"{self._name} says woof!") # f-string, lets you put variables or expressions directly into a string by using curly braces `{}`. It's like a quick way to mix words with values.
  ```
In this example, `Dog` is a class that defines how to make dogs. `_name` and `_age` are like secret variables that only the `Dog` class knows about, keeping them safe from outside meddling.
  ### Creating A Class 
```python
class Class_name:
  def __init__(self, name , brand, engine, milage):
      self.name= name
      self.brand= brand
      self.engine= engine
      self.milage= milage
```
#### Creating An Object
```python
obj_Name1 = Class_name("M4", "BMW", 4300, 10)
obj_Name2 = Class_name("F430", "Ferrari", 5600, 10)
```
### Working Of Class And Objec
```python
print(obj_Name1.name) #M4
```
