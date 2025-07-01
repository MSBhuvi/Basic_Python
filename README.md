# basic_python
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

---


