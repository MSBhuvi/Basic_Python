# Basic_python
PYTHON VARIABLES AND DATA TYPES
    - HI Welcome! If you're just starting out python. This guide will give you a quick overview of the fundamentals. 
   -  Python is a powerfull,readable, and beginner-friendly programming language used in web development,AI,
   -  Data science and more.

1) why python
Simple and readable: beginner friendly syntax
                   Stron community: Supportive and active developer base
                   Massive ecosystem: Thousands of libraries and frameworks


Commom libraries

                     
Area                                         popular libraries

Web development                              django,Flask,fastApi
data science                                 pandas,Numpy,Matplotlib
Machine learning                             scikit-learn,Pytorch,TensorFlow
Automation                                   Requestes,selenium,Pyautogui
                     
HELLO WORLD EXAMPLE 

python
print ("hello world")


---
                                

 ##  Python Variables

 In Python, **variables** are used to store data that can be referenced and manipulated later in your code.
 You don’t need to declare the type—Python is **dynamically typed**, so it figures it out for you.

  Creating Variables

  python
      name = "Arun"       # string
      age = 20             # integer
      height = 5.6         # float
      is_student = True    # boolean

Python uses `=` to assign values.


  Rules for Variable Names

* Must start with a **letter** or an **underscore (`_`)**
*  Cannot start with a number
* Can contain letters, numbers, and underscores
* Are **case-sensitive** (`Name` and `name` are different)

  Valid:

   python
         user_name = "Bob"
          _age = 30


  Invalid:

 python
 2name = "Error"     # starts with number
  user-name = "Error" # hyphen not allowed




  Reassigning & Dynamic Typing

 Variables can change type at runtime:

 python
                              
  x = 42       # int
  x = "hello"  # now it's a string

 Variable Types (Built-in)

| Type    | Example                  |
| ------- | ------------------------ |
| `int`   | `x = 10`                 |  
| `float` | `pi = 3.14`              |
| `str`   | `name = "Eve"`           |
| `bool`  | `is_valid = True`        | 
| `list`  | `nums = [1, 2, 3]`       |
|  `dict` | `user = {"name": "Max"}` |


Best Practices

* Use **meaningful names** (e.g. `user_age` instead of `ua`)
* Use **snake\_case** for variable names
* Avoid using Python **keywords** as variable names (e.g. `class`, `def`, `if`)



 *Learn more in the* [Python Docs – Variables](https://docs.python.org/3/reference/datamodel.html#objects-values-and-types)

Let me know if you’d like a visual example, code sandbox, or interactive notebook!

In python, variables are used to store the data that can be referenced
 What is a variable ?

A Variable in python is like a container used to store data you can assign values using = operator

PYTHON

 name = "Arun"
 age = 20
 is_student = True




#  Python Data Types

Python is a dynamically typed language, which means you don't need to declare a variable's type explicitly. Python has several built-in data types categorized into different classes.



##  Basic Built-in Data Types

###  Numeric Types

| Type      | Description                       | Example      |
| --------- | --------------------------------- | ------------ |
| `int`     | Integer numbers                   | `x = 42`     |
| `float`   | Floating point numbers (decimals) | `pi = 3.14`  |
| `complex` | Complex numbers                   | `z = 2 + 3j` |



###  Text Type

| Type  | Description     | Example          |
| ----- | --------------- | ---------------- |
| `str` | Unicode strings | `name = "Alice"` |



###  Boolean Type

| Type   | Description          | Example           |
| ------ | -------------------- | ----------------- |
| `bool` | True or False values | `is_valid = True` |



##  Collection Data Types

###  List

* Ordered, mutable, allows duplicates.

python
fruits = ["apple", "banana", "cherry"]


###  Tuple

* Ordered, immutable, allows duplicates.

python
dimensions = (1920, 1080)


###  Set

* Unordered, no duplicates.

python
colors = {"red", "green", "blue"}


###  Dictionary

* Key-value pairs, unordered (Python 3.6+ preserves order).

python
person = {"name": "Alice", "age": 30}




##  Other Common Types

| Type        | Description                       | Example              |
| ----------- | --------------------------------- | -------------------- |
| `NoneType`  | Represents the absence of a value | `result = None`      |
| `bytes`     | Immutable byte sequences          | `data = b"hello"`    |
| `bytearray` | Mutable byte sequences            | `arr = bytearray(5)` |
| `range`     | Represents a range of numbers     | `range(0, 10)`       |



##  Type Checking

Use the built-in `type()` and `isinstance()` functions:

python
type(42)              # <class 'int'>
isinstance(42, int)   # True




##  Type Hints (Python 3.5+)

Optional type hints using the `typing` module:

python
def greet(name: str) -> str:
return f"Hello, {name}"




##  Summary Table

| Category | Types                              |
| -------- | ---------------------------------- |
| Numeric  | `int`, `float`, `complex`          |
| Text     | `str`                              |
| Sequence | `list`, `tuple`, `range`           |
| Set      | `set`, `frozenset`                 |
| Mapping  | `dict`                             |
| Boolean  | `bool`                             |
| Binary   | `bytes`, `bytearray`, `memoryview` |
| Special  | `NoneType`                         |



##  References

* [Python Official Docs - Data Types](https://docs.python.org/3/library/stdtypes.html)
* [PEP 484 - Type Hints](https://peps.python.org/pep-0484/)





# Python Variable Naming Rules

In Python, variables are used to store data. Naming variables properly is essential for readable and maintainable code.


##  Rules for Naming Variables

## Valid Variable Names

* Must start with a **letter** (`A–Z`, `a–z`) or an **underscore** (`_`)
* Can contain letters, digits (`0–9`), and underscores (`_`)
* **Case-sensitive** (`name`, `Name`, and `NAME` are different variables)
* **Cannot be a Python keyword**

python
# Valid examples
name = "Arun"
_age = 20
user_1 = "admin"
pi_value = 3.1415



## Invalid Variable Names

python
2cool = "nope"        # ❌ Starts with a digit
first-name = "John"   # ❌ Hyphen not allowed
class = "Physics"     # ❌ 'class' is a reserved keyword


##  Best Practices (PEP 8 Style Guide)

* Use **lowercase letters** and **underscores** for variable names:

  python
  user_name = "arun"
  total_amount = 100.0
  

* Use **UPPER\_CASE** for constants:

  python
  MAX_RETRIES = 5
  

* Avoid using:

  * Single characters like `l`, `O`, or `I` (easily confused with numbers)
  * Ambiguous names like `data1`, `data2`, etc.



## Reserved Keywords (Don’t Use as Variable Names)

These are built-in and have special meaning in Python:


  ( False, None, True, and, as, assert, break, class, continue, def, del,
elif, else, except, finally, for, from, global, if, import, in, is,
lambda, nonlocal, not, or, pass, raise, return, try, while, with, yield )


You can get the full list programmatically:

python
import keyword
print(keyword.kwlist)


## Quick Check

| Variable Name | Valid? | Reason                 |
| ------------- | ------ | ---------------------- |
| `_user`       | ✅     | Starts with underscore |
| `user_123`    | ✅     | Alphanumeric + `_`     |
| `123user`     | ❌     | Starts with digit      |
| `user-name`   | ❌     | Hyphen not allowed     |
| `def`         | ❌     | Python keyword         |



##  References

* [PEP 8 - Python Style Guide](https://peps.python.org/pep-0008/#naming-conventions)
* [Python Keywords (Official Docs)](https://docs.python.org/3/reference/lexical_analysis.html#keywords)





##  Declaring Variables in Python

In Python, variables are used to store data values. You **do not need to declare the data type** explicitly—Python automatically detects the type based on the value assigned.

##  Syntax

python
variable_name = value


* `variable_name`: the name you give to the variable.
* `=`: the assignment operator.
* `value`: the data you want to store.

## Example

python
# Integer
age = 25

# String
name = "Arun"

# Float
price = 19.99

# Boolean
is_active = True


## Variable Naming Rules

* Must start with a **letter** or **underscore** (`_`)
* Can contain **letters**, **numbers**, and **underscores**
* **Case-sensitive** (`name` and `Name` are different)
* **Should not use reserved keywords** (like `class`, `if`, `for`)

## Example with Type Check

python
x = 10
print(type(x))  # <class 'int'>

x = "Python"
print(type(x))  # <class 'str'>


## Best Practices

* Use **meaningful names** (`user_name` instead of `x`)
* Use **snake\_case** for variable names (e.g., `total_amount`)
* Use **lowercase letters** (constants can be in UPPERCASE)


##  Creating Variables in Python


## Example: Creating Different Types of Variables

python
# Integer variable
age = 20

# Float variable
height = 5.9

# String variable
name = "Arun"

# Boolean variable
is_student = True

# List variable
hobbies = ["reading", "coding", "gaming"]

# Dictionary variable
user = {
    "name": "Arun",
    "age": 21,
    "is_student": True
}

# Print all variables
print(name, age, height, is_student)
print("Hobbies:", hobbies)
print("User Info:", user)


## Output:

Arun 21 5.9 True
Hobbies: ['reading', 'coding', 'gaming']
User Info: {'name': 'Arun', 'age': 21, 'is_student': True}

## Quick Notes

* No need to use `var`, `int`, `string`, etc.
* Use descriptive names (`name`, `hobbies`) instead of `x`, `a1`.
* Python uses dynamic typing — you can change the type later.


---

##  Printing Variable Values in Python

Use the `print()` function to display variable values in the console.

## Example

python
name = "Arun"
age = 21

# Print individual variables
print(name)
print(age)

# Print with custom message
print("Name:", name)
print("Age:", age)

# Using f-string (Python 3.6+)
print(f"My name is {name} and I am {age} years old.")
```

## Output


Arun
21
Name: Arun
Age: 21
My name is Arun and I am 21 years old. 


---


---

## Python Data Types – Quick Overview 

Python has several **built-in data types** used to store values of different kinds:

## Basic Data Types:

| Type      | Example          | Description                | 
| --------- | ---------------- | -------------------------- | 
| `int`     | `x = 10`         | Integer numbers            |
| `float`   | `y = 3.14`       | Decimal numbers            | 
| `complex` | `z = 2 + 3j`     | Complex numbers            | 
| `bool`    | `flag = True`    | Boolean (`True` / `False`) |
| `str`     | `name = "Alice"` | Text or string values      |

## Collection Data Types: 

| Type    | Example                        | Description                   |
| ------- | ------------------------------ | ----------------------------- |
| `list`  | `fruits = ["apple", "banana"]` | Ordered, mutable collection   |
| `tuple` | `coords = (10, 20)`            | Ordered, immutable collection |
| `set`   | `ids = {1, 2, 3}`              | Unordered, unique values      |
| `dict`  | `person = {"name": "Bob"}`     | Key-value pairs               |

## Type Checking

python
print(type(10))        # <class 'int'>
print(type("hello"))   # <class 'str'>


## Type Conversion

python
int("5")     # → 5
str(10)      # → "10" 
list("abc")  # → ['a', 'b', 'c'] 

---
    









      



   

    
    



    








