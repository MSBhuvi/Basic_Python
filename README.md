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
    
Sure! Here's a **short and GitHub-friendly** explanation of the **comma operator in Python**:

---

## Comma in Python – Not an Operator!

In Python, the **comma (`,`) is *not* an operator** like in C/C++.
Instead, it's used to **create tuples** or **separate values** in function arguments, assignments, and loops.

---

## Usage Examples:

python
# Tuple creation
a = 1, 2, 3
print(type(a))  # <class 'tuple'>

# Multiple assignment
x, y = 10, 20

# Function arguments
def add(a, b):
    return a + b

result = add(5, 7)

# Loop with multiple variables
for i, val in enumerate(['a', 'b']):
    print(i, val)


---

## Summary:

* **Comma is a separator**, not an operator.
* Often used to **create tuples** or **unpack variables**.

---

---

## Printing Text Using Comma in Python

In Python, commas inside `print()` **separate multiple values** and insert a **space** between them.

---

### ✅ Example:

python
# Printing multiple values using comma
name = "Arun"
age = 25

print("Name:", name, "| Age:", age)


**Output:**


Name: Arun | Age: 25


---

## Notes:

* Commas let you print different types (like strings + numbers) without converting them.
* Adds automatic spaces between items.

---

---

## Printing with `sep` and `end` in Python

Python’s print() function has two useful optional parameters:

* **`sep`**: Defines the **separator** between multiple items.
* **`end`**: Defines what to print at the **end** of the output (default is a newline `\n`).

---

## `sep` – Separator Between Values

By default, print() separates multiple arguments with a space.

python
print("Python", "is", "awesome")  
# Output: Python is awesome


You can change the separator using `sep`:

python
print("Python", "is", "awesome", sep="-")
# Output: Python-is-awesome


---

## `end` – What to Print at the End

By default, `print()` ends with a newline (`\n`):

python
print("Hello")
print("World")
# Output:
# Hello
# World


You can change this using `end`:

python
print("Hello", end=" ")
print("World")
# Output: Hello World

---

## Combine `sep` and `end`

python
print("2025", "07", "04", sep="-", end="!\n")
# Output: 2025-07-04!

---

## Tip

Use `sep` and `end` to format output **without string concatenation**!

---

## Example: Using `sep` in `print()` (Short Version)

python
print("Hello", "World", "2025", sep=" - ")


**Output:**

Hello - World - 2025

The `sep` parameter sets the **separator** between printed values.

## Example: Using `end` Parameter in `print()`

python
print("Hello", end=" ")
print("World!")

**Output:**

Hello World!

 `end=" "` keeps the cursor on the same line with a space instead of a newline.

---

## Printing with **f-Strings** in Python

**f-Strings** (formatted string literals) make it easy to include variables and expressions inside strings using `{}`.
Available from **Python 3.6+**.

---

## Basic Syntax

python
name = "Arun"
print(f"Hello, {name}!")

**Output:**


Hello, Arun!


 Just add an `f` before the opening quote, and put variables or expressions inside `{}`.

---

## With Expressions

python
a = 5
b = 10
print(f"The sum of {a} and {b} is {a + b}")

**Output:**


The sum of 5 and 10 is 15

---

## Formatting Numbers

python
pi = 3.14159
print(f"Value of pi: {pi:.2f}")

**Output:**


Value of pi: 3.14

---

## Example with Date

python
from datetime import datetime
today = datetime.now()
print(f"Today's date: {today:%Y-%m-%d}")

**Output:**

Today's date: 2025-07-04

---

## Clean & Readable

f-Strings are:

* Faster and more readable than `format()` or `%` formatting
* Great for inline calculations and formatting

---

## Short Example: Using `f-string` in Python

python
name = "Arun"
print(f"Hello, {name}!")

**Output:**

Hello, Arun!

🔹 f-strings let you insert variables directly into strings using `{}`.

## Rounding to Two Decimal Places in Python (Shortly)

Use the built-in `round()` function:

python
num = 3.14159
rounded = round(num, 2)
print(rounded)

**Output:**

3.14

 round(number, 2) rounds the number to 2 decimal places.

---

## Comments in Python

**Comments** are notes in your code to explain what it does. They are **ignored by the Python interpreter**.

---

## Single-Line Comments

Use the `#` symbol:

python
# This is a single-line comment
print("Hello, World!")  # This prints a message

---

## Multi-Line Comments (Workaround)

Python doesn’t have official multi-line comment syntax, but you can use multiple `#`:

python
# This is a comment
# that spans multiple lines
print("Done")

Or use a **docstring** (not recommended unless for documentation):

python
"""
This is a multi-line string
which can act like a comment
"""

>  Note: Triple-quoted strings are not true comments — they are stored as string objects if not assigned.

---

## Best Practices

* Use comments to explain **why**, not **what** (if code is self-explanatory)
* Keep them **short and clear**
* Update comments when code changes

---

## Why Are Comments Used in Python? 

**Comments** are used to:

* Explain code for better readability
* Make the code easier to understand and maintain
* Help other developers (and your future self) know **why** something was done
* Temporarily disable code during debugging

 Comments are ignored by the Python interpreter.

##  Example: Comments in Python

python
# This prints a welcome message
print("Welcome to Python!")

🔹 The `#` makes everything after it a comment (ignored by Python).

---

## Printing a String Multiple Times in Python

Use the `*` operator to repeat a string:

python
print("Hello " * 3)

**Output:**

Hello Hello Hello 

 The `*` operator repeats the string **n** times.

---

## Example: Multi-line String in Python

You can use triple quotes (`'''` or `"""`) to create a multi-line string:

python
message = """Hello,
This is a multi-line
string in Python."""
print(message)

**Output:**

Hello,
This is a multi-line
string in Python.

🔹 Triple quotes preserve line breaks and spacing.

---

## Type Casting in Python

**Type casting** means converting a value from one data type to another (e.g., `int` to `float`, `str` to `int`, etc.).

Python provides built-in functions for casting:

---

## Common Type Casting Functions

| Function  | Converts to... |
| --------- | -------------- |
| `int()`   | Integer        |
| `float()` | Floating point |
| `str()`   | String         |
| `bool()`  | Boolean        |

---

## Examples

python
# String to int
num = int("10")         # 10

# Float to int (truncates)
x = int(3.7)            # 3

# Int to float
y = float(5)            # 5.0

# Number to string
text = str(123)         # "123"

# Non-zero to True
val = bool(1)           # True

---

## Note

Type casting may raise errors if the conversion is invalid:

python
int("abc")  #  ValueError

---

## Use Cases

* Accepting user input (`input()` returns a string)
* Mathematical operations
* Data processing and validation

---

---

## Calculating Total Salary in Python

## **Theory**

To calculate total salary, you typically use:

total_salary = basic_salary + allowances - deductions

Where:

* **basic\_salary**: Fixed base salary
* **allowances**: Extra income (e.g., HRA, travel, etc.)
* **deductions**: Amounts subtracted (e.g., tax, PF, etc.)

You can use variables and simple arithmetic to compute this.

---

## **Python Code Example**

python
# Define salary components
basic_salary = 25000
allowances = 5000
deductions = 3000

# Calculate total salary
total_salary = basic_salary + allowances - deductions

# Display the result
print(f"Total Salary: ₹{total_salary}")

---

### 📌 Output:

Total Salary: ₹27000

---

## Tip

You can also use `input()` to take user input for dynamic salary calculation:

python
basic = float(input("Enter basic salary: "))
allow = float(input("Enter allowances: "))
deduct = float(input("Enter deductions: "))

total = basic + allow - deduct
print(f"Total Salary: ₹{total}")

---





      



   

    
    



    








