## Inheritance
Inheritance in Python is like passing down traits from a parent to a child. 

- **What?** Inheritance allows a class (child class) to inherit properties and methods from another class (parent class).
- **Why?** It promotes code reuse and helps in organizing code by creating a hierarchy of classes.
- **Use?** Define a child class by specifying the parent class in parentheses after the child class name.
### Syntax:
```python
class ChildClassName(ParentClassName):
    # class body
    pass
```
### Example:
```python
# Parent class
class Animal:
    def speak(self):
        print("Animal speaks")

# Child class inheriting from Animal
class Dog(Animal):
    def bark(self):
        print("Dog barks")

# Create an object of the child class
my_dog = Dog()

# Call methods from both parent and child classes
my_dog.speak()  # Output: Animal speaks
my_dog.bark()   # Output: Dog barks
```

In this example:
- `Animal` is the parent class.
- `Dog` is the child class that inherits from `Animal`.
- `Dog` automatically gains access to the `speak()` method defined in the `Animal` class, without needing to redefine it. This is the essence of inheritance.
- 
```python
  class Normal_Car:
    def color(self):
        print("red, blue, white, black")
    
    def seats(self):
        print("2 to 4 seats")
      
class Super_Car(Normal_Car):#as a super car also have properties of a Normal Car so we inherit it
    def cost(self):
        print("Costly cars")
    
    def status(self):
        print("status icon")

obj_Name1 = Super_Car()  # Create object
obj_Name1.color()  # Call color() method
obj_Name1.status()  # Call status() method
```
