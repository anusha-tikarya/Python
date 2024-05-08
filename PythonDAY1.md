###  Printing Strings and Numbers
```python
# Printing Strings and Numbers
print("hello World , I'm Anusha")
print("I am 21")
print(21)
print(21 + 22)
```
### Variables and Data Types
```python
# Variables and Data Types
name = "shradha"
age = 12
score = 90.9
age2 = age + 3
print("My name is:", name)
print(name, "is", age2, "years old")
print(type(name))
print(type(age2))
print(type(score))
```
### Booleans and None
```python
# Booleans and None
old = True
a = None
print(type(old))
print(type(a))
```
###  Function to Sum Two Numbers
```python
# Function to Sum Two Numbers
def sum(a, b):
    sum = a + b
    return sum

print(sum(1, 2))
```
### String Operations \n , \t
```python
# String Operations
str = "I am happy \n I am healthy \t I am wealthy"    # \n for new line and \t for tab
print(str)
```
### Concatenation
```python
# Concatenation
a = "hello"
b = "Indore"
print(a + " " + b)
print(len(a))  # len used for length
ch = a[2]  # Access value of a at the index of 2, similar we cannot assign the value
print(ch)
```
###  Slicing

```python
# Slicing
str = "apple is red"
print(str[1:])
print(str[:6])
print(str[-5:-1])
print(str[:-3])
```
### endswith , capitalize , replace , find , count
```python
print(str.endswith("app"))  # endswith function tells if a function ends with a particular string or not
print(str.capitalize())  # capitalize makes the first letter of the string capital.
print(str.replace("apple", "cherry"))
print(str.find("c"))  # -1 as it doesn't exist
print(str.find("apple"))  # name starts at index _
print(str.count("e"))  # count no. of occurrence of a particular string
```

