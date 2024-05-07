![image](https://github.com/anusha-tikarya/Python.md/assets/84814767/89dbbf8c-6a7b-463f-a026-2a8177789caf)
```python
employees = [
    {"name": "Sneha", "experience": 2},
    {"name": "Manju"},
    {"name": "Sai Subash", "experience": 4},
    {"name": "Manasa"},
]
``` 
 
# Task1 : After 1 experience
Output
```python 
[
    {"name": "Sneha", "experience": 3},
    {"name": "Manju",  "experience": 1},
    {"name": "Sai Subash", "experience": 5},
    {"name": "Manasa", "experience": 1},
]```
# Code
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
```
