![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/01618c32-90cd-483a-9da2-1a4f2178f2f9)

![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/fcc09729-03b2-4a77-b7a4-ec49b2a23d01)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/78cb8242-7076-4003-ab5b-a2f92908df32)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/7f74b217-fd14-44ab-b176-7ea54133ded5)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/9c2f779a-9ed7-4bdd-8ca2-b23be33e352b)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/db4b5d09-cfb5-432c-bb6b-358bea094339)
![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/de19b352-e14f-4307-b888-f4faf1831ece)

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
