## SET
A set in Python is an unordered collection of unique elements. It's similar to lists and dictionaries, but with some distinct characteristics:

1. **Uniqueness**: A set cannot contain duplicate elements. If you try to add a duplicate element to a set, it won't be added multiple times.

2. **Unordered**: Unlike lists, sets are unordered, meaning the elements are not stored in any particular order. When you iterate over a set, the order of elements is not guaranteed.

3. **Mutability**: Sets are mutable, meaning you can add or remove elements after creation.

Here's how you can create and use sets in Python:

**Creating a Set**:
You can create a set by enclosing comma-separated values within curly braces `{}`.

```python
my_set = {1, 2, 3, 4, 5}
```

**Adding Elements**:
You can add elements to a set using the `add()` method.

```python
my_set.add(6)
```
In Python, you can add more values to a set using the `.add()` method to add a single element or the `.update()` method to add multiple elements. Here's how you can use them:

**Using `.add()` to Add a Single Element:**
```python
# Define a set
my_set = {1, 2, 3}

# Add a single element to the set
my_set.add(4)

print(my_set)  # Output: {1, 2, 3, 4}
```

In this example, the `.add()` method adds the element `4` to the set `my_set`.

**Using `.update()` to Add Multiple Elements:**
```python
# Define a set
my_set = {1, 2, 3}

# Add multiple elements to the set
my_set.update([4, 5, 6])

print(my_set)  # Output: {1, 2, 3, 4, 5, 6}
```

In this example, the `.update()` method adds the elements `[4, 5, 6]` to the set `my_set`.

Both `.add()` and `.update()` methods modify the original set in place. If you try to add elements that are already present in the set, they will be ignored, as sets do not allow duplicate elements.

**Removing Elements**:
You can remove elements from a set using the `remove()` or `discard()` method.

```python
my_set.remove(3)
```

**Operations on Sets**:

- **Union**: Combines elements from two sets into a new set.

  ```python
  set1 = {1, 2, 3}
  set2 = {3, 4, 5}
  union_set = set1.union(set2)
  ```

- **Intersection**: Finds common elements between two sets.

  ```python
  intersection_set = set1.intersection(set2)
  ```

- **Difference**: Finds elements in one set but not the other.

  ```python
  difference_set = set1.difference(set2)
  ```

- **Symmetric Difference**: Finds elements that are in either of the sets, but not in both.

  ```python
  symmetric_difference_set = set1.symmetric_difference(set2)
  ```

- **Subset and Superset Checking**:

  ```python
  is_subset = set1.issubset(set2)
  is_superset = set1.issuperset(set2)
  ```

Sets are useful for various tasks like eliminating duplicates from a list, checking for membership, and performing set operations like union, intersection, etc. They are particularly efficient for membership testing and eliminating duplicates from a sequence.

 ## Tuples
Tuples in Python are another data structure, similar to lists, but with a few key differences:

1. **Immutable**: Tuples are immutable, meaning once they are created, their elements cannot be changed or modified. However, if an element is itself mutable (like a list), it can be modified.

2. **Ordered**: Like lists, tuples are ordered collections, meaning the order of elements in a tuple is preserved.

3. **Heterogeneous Elements**: Tuples can contain elements of different data types, including other tuples.

Here's how you can create and use tuples in Python:

**Creating Tuples**:
You can create tuples by enclosing comma-separated values within parentheses `()`.

```python
my_tuple = (1, 2, 3, "apple", "banana")
```

**Accessing Elements**:
You can access individual elements of a tuple using indexing, similar to lists.

```python
print(my_tuple[0])  # Output: 1
```

**Slicing**:
You can slice tuples to extract sub-tuples.

```python
print(my_tuple[1:3])  # Output: (2, 3)
```

**Tuple Packing and Unpacking**:
You can pack multiple values into a tuple, and also unpack a tuple into multiple variables.

```python
# Tuple packing
my_packed_tuple = 1, 2, "apple"

# Tuple unpacking
x, y, z = my_packed_tuple
print(x, y, z)  # Output: 1 2 apple
```

**Iterating Over Tuples**:
You can iterate over the elements of a tuple using a `for` loop.

```python
for item in my_tuple:
    print(item)
```

**Tuple Operations**:

- Concatenation: You can concatenate tuples using the `+` operator.
- Repetition: You can repeat a tuple using the `*` operator.

**Functions and Methods**:
Tuples have built-in functions like `len()`, `max()`, `min()`, and methods like `count()` and `index()`.

```python
print(len(my_tuple))
print(my_tuple.count(2))
```

Tuples are often used in situations where immutability and order are required, such as representing fixed collections of data, returning multiple values from functions, and as keys in dictionaries.



