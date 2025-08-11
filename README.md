# Basic_python
                                                                          CHAPTER 1

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

## Example: A  ( Calculating Total Salary in Python )

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

Example: B  coverting string to float

The following code converts Ivan's salary from a string to float;otherwise, the program generates an error.
Arun's wage is not enclosed with a double quote;therefore, it is already a number and doesn't need to be covrerted

calculator.py

salary_ivan=3200
salary_Arun="2800"
total_salary=salary_ivan+float(salary_Arun)
print("Total salaries:$",total_salary)

OUTPUT

Total salaries:$6000.0

---
Example: C  coverting string to Int

To calculate the age difference between two individuals, you must covert the second age to int type because the second age is a string
      
calculate.py 

age1=22
age2"34"
age_difference=int(age2)-age1
print("Age Difference:",age_difference)

OUTPUT

Age Difference: 12

---
   
---

## Escape Sequences in Python

**Escape sequences** are special characters used in strings to represent characters that are otherwise difficult to include directly, like newlines, tabs, quotes, etc.

They begin with a **backslash (`\`)**.

---

## Common Escape Sequences:

| Escape | Meaning          | Example Output                |
| ------ | ---------------- | ----------------------------- |
| `\n`   | New line         | Splits the text to a new line |
| `\t`   | Tab (horizontal) | Adds a tab space              |
| `\\`   | Backslash        | Prints `\` character          |
| `\'`   | Single quote     | Prints `'` in a string        |
| `\"`   | Double quote     | Prints `"` in a string        |

---

## Example:

python
# Using escape sequences
print("Hello\nWorld")     # New line
print("Python\tRocks")    # Tab space
print("He said: \"Yes\"") # Double quotes inside string
print('It\'s awesome!')   # Single quote inside string

---

## Output:


Hello
World
Python	Rocks
He said: "Yes"
It's awesome!

---

## Tip:

You can also use **raw strings** (`r"..."`) to **ignore escape sequences**.

python
print(r"This is a raw string:\nNo new line here.")

🧾 Output:

This is a raw string:\nNo new line here.

---

---

## Escape Sequence Quiz (Python)

Test your knowledge of escape sequences!
**Choose the correct output or fill in the blanks.**

---

## 1. What will this code print?

python
print("Hello\nPython")


A. Hello Python
B. Hello\nPython
C. Hello
        Python
D. Error

> ✅ **Answer:** C

---

## 2. Which escape sequence is used to insert a tab space?

A. \\n
B. \t
C. \n
D. \b

> ✅ **Answer:** B

---

 QUIZ: 2
 
## 1. Fill in the blank to print this output:

He said: "Hello"

python
print("He said: _______")

> ✅ **Answer:** "He said: \"Hello\""

---

## 2. What is the output of this code?

python
print('It\'s easy!')


A. It's easy!
B. Its easy!
C. It\'s easy!
D. Error

> ✅ **Answer:** A

---

---

## Escape Sequence Quiz – *Total Weight in a Lift*

**Scenario:**
You're building a Python program to display the **total weight of 3 people** inside a lift.
Use **escape sequences** to format the output nicely.

---

## Task:

Fill in the blanks ( ___ ) to complete the program.

python
# Lift Weight Calculator

person1 = 65.5
person2 = 72.0
person3 = 58.3

# Calculate total weight
total_weight = person1 + person2 + person3

# Print the result using escape sequences
print("Lift Weight Report\n")
print("Person 1:\t", person1, "kg")
print("Person 2:\t", person2, "kg")
print("Person 3:\t", person3, "kg")
print("\nTotal:\t\t", total_weight, "kg")

---

## Quiz Questions:

1. What does \n do in the print statement?

   * A. Adds a new line
   * B. Adds a tab
   * C. Prints a slash
   * D. None of the above

2. What is the purpose of \t in this code?

   * A. New paragraph
   * B. Adds a tab space for alignment
   * C. Skips the line
   * D. None

3. What is the **total weight** calculated in the program?

---

## Expected Output:

Lift Weight Report

Person 1:	 65.5 kg
Person 2:	 72.0 kg
Person 3:	 58.3 kg

Total:		 195.8 kg

---

---

## Escape Sequence Exercise – *Printing Variable Values & Types*

** Objective:**
Practice using **escape sequences** (`\n`, `\t`) along with `print()`, `type()`, and variables.

---

###  Instructions:

1. Declare 3 different variables with different data types.
2. Use print() to:

   * Show each variable's **value**
   * Show its **type**
   * Use **\n for new lines** and **\t for indentation**
3. Try to format the output to look clean and readable.

---

###  Sample Code (Complete This):

python
# Variable Declarations
name = "Alice"
age = 25
height = 5.4

# Print values and types using escape sequences
print("Variable Info:\n")

print("Name:\t", name)
print("Type:\t", type(name), "\n")

print("Age:\t", age)
print("Type:\t", type(age), "\n")

print("Height:\t", height)
print("Type:\t", type(height), "\n")

---

## Expected Output:

Variable Info:

Name:	 Alice
Type:	 <class 'str'>

Age:	 25
Type:	 <class 'int'>

Height:	 5.4
Type:	 <class 'float'>

---

## Challenge Yourself:

* Try with bool and list types too.
* Use f-strings instead of commas in print() for cleaner formatting.

---

## Exercise: Print a Shape Using Escape Sequences

** Task:**
Use **\n** (new line) and **\t** (tab) escape sequences to print the following triangle shape:

	    *
	   * *
	  * * *
	 * * * *

---

## Starter Code:

python
# Print triangle using escape sequences
print("\t\t\t*")
print("\t\t  * *")
print("\t    * * *")
print("      * * * *")

---

## Instructions:

* Use \t for horizontal spacing (tab).
* Use \n if printing all lines together in a single `print()` statement.
* Try modifying the shape or adding more lines!

---

---

## Python Operators – Quick Guide

**Operators** are special symbols used to perform **operations** on variables and values.

---

## 1. **Arithmetic Operators**

Used for basic math.

| Operator | Description        | Example        |
| -------- | ----------------- | -------------- |
| +      | Addition            | `3 + 2 = 5`    |
| -      | Subtraction         | `5 - 1 = 4`    |
| *      | Multiplication      | `4 * 2 = 8`    |
| /      | Division            | `10 / 2 = 5.0` |
| //     | Floor Division      | `10 // 3 = 3`  |
| %      | Modulus (Remainder) | `10 % 3 = 1`   |
| **     | Exponentiation      | `2 ** 3 = 8`   |

---

## 2. **Comparison Operators**

Compare two values and return `True` or `False`.

| Operator | Description      | Example         |
| -------- | ---------------- | --------------- |
| `==`     | Equal to         | `5 == 5 → True` |
| `!=`     | Not equal to     | `3 != 4 → True` |
| `>`      | Greater than     | `7 > 2 → True`  |
| `<`      | Less than        | `2 < 5 → True`  |
| `>=`     | Greater or equal | `5 >= 5 → True` |
| `<=`     | Less or equal    | `4 <= 6 → True` |

---

### 🔹 3. **Assignment Operators**

Used to assign values.

| Operator | Meaning             | Example              |
| -------- | ------------------- | -------------------- |
| `=`      | Assign              | `x = 10`             |
| `+=`     | Add and assign      | `x += 5 → x = x + 5` |
| `-=`     | Subtract and assign | `x -= 3 → x = x - 3` |
| `*=`     | Multiply and assign | `x *= 2`             |
| `/=`     | Divide and assign   | `x /= 4`             |

---

### 🔹 4. **Logical Operators**

Used to combine conditions.

| Operator | Description           | Example            |
| -------- | --------------------- | ------------------ |
| `and`    | True if both are true | `x > 5 and x < 10` |
| `or`     | True if one is true   | `x < 3 or x > 8`   |
| `not`    | Reverses the result   | `not(x == 5)`      |

---

### 🔹 5. **Identity Operators**

Used to compare object identity.

| Operator | Meaning             | Example      |
| -------- | ------------------- | ------------ |
| `is`     | True if same object | `x is y`     |
| `is not` | True if not same    | `x is not y` |

---

### 🔹 6. **Membership Operators**

Check if a value exists in a sequence.

| Operator | Meaning              | Example              |
| -------- | -------------------- | -------------------- |
| `in`     | Value exists         | `"a" in "apple"`     |
| `not in` | Value does not exist | `"z" not in "apple"` |

---

## Example Code:

python
x = 10
y = 5

print(x + y)       # Arithmetic
print(x > y)       # Comparison
print(x == 10 and y == 5)  # Logical
x += 2             # Assignment
print(x)

---

# Example for Arithmetic Operators in Python

a = 10
b = 3

# Addition
print("Addition:", a + b)

# Subtraction
print("Subtraction:", a - b)

# Multiplication
print("Multiplication:", a * b)

# Division
print("Division:", a / b)

# Floor Division
print("Floor Division:", a // b)

# Modulus
print("Modulus:", a % b)

# Exponentiation
print("Exponentiation:", a ** b)

## Modulus (`%`) in Python – Short Explanation

The **modulus operator %** returns the **remainder** of a division.

#### Example:

python
print(10 % 3)  # Output: 1

 Here, 10 ÷ 3 = 3 with a **remainder of 1** → so 10 % 3 gives 1.

## Use Cases:

* Check if a number is even/odd:

  python
  print(7 % 2)  # Output: 1 → odd
  print(8 % 2)  # Output: 0 → even
  
* Looping in cycles, e.g., `i % 4` cycles 0,1,2,3,0,...
* Useful in clock-based logic or round-robin systems.

---

python
# Modulus Example

a = 17
b = 5

result = a % b
print("Remainder:", result)  # Output: 2

 **Explanation:** 17 ÷ 5 = 3 remainder **2**, so 17 % 5 = 2.

---

## Floor Division in Python (`//`) 

**Floor division** returns the **quotient** of a division, **rounded down** to the nearest whole number.

## Syntax:

python
a // b

## Example:

---

# Floor Division Example

a = 17
b = 5

result = a // b
print("Quotient:", result)  # Output: 3

 **Explanation:**
17 ÷ 5 = 3.4 → floor division 17 // 5 = 3 (rounds down).

Common use: Get whole number part of a division without decimals.

---
    
## Assignment Operator in Python — Short & GitHub-Friendly

The **assignment operator `=`** is used to **assign a value** to a variable.

## Example:

# Assignment Operator Example

x = 10  # Assigns 10 to variable x
print("x =", x)


## Other compound assignment operators:

python
x += 5   # x = x + 5
x -= 2   # x = x - 2
x *= 3   # x = x * 3
x /= 2   # x = x / 2

 **Tip:** Assignment operators help update variable values concisely.
    
---

# Assignment Operator Example

x = 5
print("x =", x)  # Output: x = 5

 This assigns the value 5 to the variable x.

---

##  Using `+` and `+=` with Strings in Python 

####  `+` Operator → **Concatenates** strings (joins them)

greeting = "Hello, " + "World!"
print(greeting)  # Output: Hello, World!

## `+=` Operator → **Appends** to an existing string

message = "Hello"
message += ", Python!"
print(message)  # Output: Hello, Python!

 **Tip:**

* + creates a **new string**
* += updates the **existing string variable**

 Useful for building strings in loops or step-by-step.

---
Example for concatenate strings using "+"

# String Concatenation using +

first = "Hello"
second = "World"
result = first + " " + second
print(result)  # Output: Hello World

---

 Here's a short example for **concatenating strings using `+=`**:

# String Concatenation using +=

text = "Hello"
text += " World"
print(text)  # Output: Hello World

 += adds " World" to the existing text string.

---

## Comparison Operators in Python 

**Comparison operators** are used to **compare values**. They return either True or False.

## List of Comparison Operators:

| Operator | Meaning               | Example           |
| -------- | --------------------- | ----------------- |
| `==`     | Equal to              | `5 == 5` → `True` |
| `!=`     | Not equal to          | `5 != 3` → `True` |
| `>`      | Greater than          | `7 > 2` → `True`  |
| `<`      | Less than             | `3 < 4` → `True`  |
| `>=`     | Greater than or equal | `5 >= 5` → `True` |
| `<=`     | Less than or equal    | `2 <= 3` → `True` |

## Example:

a = 10
b = 5

print(a > b)   # True
print(a == b)  # False

 **Tip:** Commonly used in `if` statements, loops, and filters.

---

 A short example for **comparison operators** in Python:


# Comparison Operator Example

a = 7
b = 5

print(a > b)   # True
print(a == b)  # False

 Compares values and returns True or False.

---

## Logical Operators in Python 

**Logical operators** are used to combine conditional statements. They return True or False.

## Types of Logical Operators:

| Operator | Description                      | Example                    |
| -------- | -------------------------------- | -------------------------- |
| `and`    | True if **both** are True        | `True and False` → `False` |
| `or`     | True if **at least one** is True | `True or False` → `True`   |
| `not`    | Reverses the result              | `not True` → `False`       |

## Example:

python
a = 5
b = 10

print(a > 2 and b > 8)   # True
print(a < 3 or b == 10)  # True
print(not(a == b))       # True


**Tip:** Used in if statements to combine multiple conditions.

---

  A short example for **logical operators** in Python:

python
# Logical Operator Example

x = 10
y = 5

print(x > 5 and y < 10)   # True
print(x < 5 or y == 5)    # True
print(not(x == y))        # True

 Combines conditions using and, or, not.

---

## Identity Operators in Python 

**Identity operators** are used to **compare the memory location** of two objects.

## Types of Identity Operators:

| Operator | Description                                      | Example      |
| -------- | ------------------------------------------------ | ------------ |
| `is`     | Returns `True` if **both refer to same object**  | `a is b`     |
| `is not` | Returns `True` if **they are different objects** | `a is not b` |

## Example:

a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)      # True  (same object)
print(a is c)      # False (different object with same value)
print(a is not c)  # True

 **Note:** Use == to compare **values**, is to compare **identity**.

---

A short example for **identity operators** in Python:

# Identity Operator Example

a = [1, 2]
b = a
c = [1, 2]

print(a is b)      # True
print(a is c)      # False
print(a is not c)  # True

 `is` checks if both refer to the **same object in memory**.

---

## Membership Operators in Python 

**Membership operators** are used to **check if a value exists** in a sequence (like a list, string, tuple, etc).

## Types of Membership Operators:

| Operator | Description                                | Example                       |
| -------- | ------------------------------------------ | ----------------------------- |
| `in`     | Returns `True` if value is present         | `"a" in "apple"` → `True`     |
| `not in` | Returns `True` if value is **not** present | `3 not in [1, 2, 4]` → `True` |

## Example:

fruits = ["apple", "banana", "cherry"]

print("apple" in fruits)     # True
print("grape" not in fruits) # True

 **Tip:** Great for searching in strings, lists, and other collections.

 ---

 A short quiz on **arithmetic operators**:

---

## **Quiz:**

What will be the output of the following code?

x = 8
y = 3
print(x % y + x // y)

**A.** 3
**B.** 5
**C.** 4
**D.** 6

---

 A short quiz on the **assignment operator**:

---

## **Quiz: Assignment Operator**

**Question:**
What will be the output of the following code?

x = 10
x += 5
print(x)

**A.** 10
**B.** 5
**C.** 15
**D.** Error

---

 **Answer:** C. 15
**Explanation:** `x += 5` means `x = x + 5`, so `10 + 5 = 15`.

--- 

Sure! Here's a short quiz for comparison operators in Python:

---

** Quiz: Comparison Operator in Python**

**Question:**
What will be the output of the following code?

x = 10
y = 20
print(x > y)

**A.** True
**B.** False
**C.** 10
**D.** 20

---

*Correct Answer:* **B. False**
**Explanation:** `10 > 20` is not true, so it returns `False`.

---


## **Quiz: Identity Operator in Python**

**Question:**
What will be the output of the following code?

x = [1, 2, 3]
y = x
z = [1, 2, 3]

print(x is y)
print(x is z)

**Options:**
A) `True` `True`
B) `True` `False`
C) `False` `True`
D) `False` `False`

---

**Answer:**  **B) True False**

**Explanation:**

* `x is y` → `True` because `y` refers to the same object as `x`.
* `x is z` → `False` because `z` is a new list with the same values, but it's a different object in memory.

---

##  User Input & Strings in Python

## Getting User Input

Python uses the input() function to get data from the user.

name = input("Enter your name: ")
print("Hello,", name)

* input() always returns data as a **string**.

## Working with Strings

You can use **string methods** to manipulate text:

text = "  python is FUN!  "

print(text.strip())       # Removes leading/trailing spaces
print(text.lower())       # Converts to lowercase
print(text.upper())       # Converts to uppercase
print(text.replace("FUN", "awesome"))  # Replaces words

## Concatenating Strings

Join strings using `+` or `f-strings`:

first = "Hello"
last = "World"

print(first + " " + last)        # Using +
print(f"{first} {last}!")        # Using f-string

---

 **Tip:** Always convert input to the needed type (e.g., `int(input())` for numbers).

---

## **User Input in Python (Short)**

Python uses the `input()` function to take input from the user.

name = input("Enter your name: ")
print("Hello,", name)

* input() **always returns a string**.
* You can convert input to other types using `int()`, `float()`, etc.

age = int(input("Enter your age: "))
print("You will be", age + 1, "next year.")

---

Example: To create a triangle using user input:

rows = int(input("Enter number of rows: "))

for i in range(1, rows + 1):
    print("*" * i)

## Sample Output:

If user enters `5`:

*
**
***
****
*****

This prints a **right-angled triangle** of stars (`*`).

Example: to calculate **total weight** using user input:

item1 = float(input("Enter weight of item 1 (kg): "))
item2 = float(input("Enter weight of item 2 (kg): "))
total = item1 + item2

print("Total weight:", total, "kg")

## Sample Output:

Enter weight of item 1 (kg): 2.5  
Enter weight of item 2 (kg): 3.2  
Total weight: 5.7 kg

Example: to check the **variable types** using `type()` in Python:

name = "Alice"
age = 25
height = 5.6
is_student = True

print(type(name))      # <class 'str'>
print(type(age))       # <class 'int'>
print(type(height))    # <class 'float'>
print(type(is_student))# <class 'bool'>

## Output:

<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>

---

Example for converting strings to integers using user input:

# Get user input
num = input("Enter a number: ")

# Convert string to integer
num = int(num)

# Display result
print("You entered:", num)

 **Note:** `input()` always returns a string. Use `int()` to convert it to an integer.

---

explanation of **strings and substrings** in Python:

---

## Strings in Python

* A **string** is a sequence of characters enclosed in quotes (' ' or " ").
* Example:

  message = "Hello, Python!"
  
## Substrings

* A **substring** is a part of a string.

* You can extract substrings using **slicing**:

  text = "Programming"
  print(text[0:6])  # Output: Progra
  
* You can also **check** if a substring exists:

  "gram" in text   # True
  
---

**Tip:** Python strings are **zero-indexed**.

 **Test it out**:

word = "education"
print(word[1:4])         # duc
print("cat" in word)     # True

---

 Explanation of **string indexing** in Python:

---

## String Index in Python

* **Indexing** lets you access individual characters in a string.
* Index starts at **0** (zero-based indexing).

text = "Python"
print(text[0])  # P
print(text[5])  # n

* You can also use **negative indexes** to count from the end:

print(text[-1])  # n (last character)
print(text[-3])  # h

---

 **Tip:** Use indexes to loop, slice, or manipulate characters in strings.

A short example for **string index**:

name = "Python"
print(name[0])   # Output: P
print(name[3])   # Output: h
print(name[-1])  # Output: n (last character)

 This shows how to access characters using positive and negative indexes.

  A explanation of **substrings** in Python:

---

## Substrings in Python

* A **substring** is a part of a string.

* Use **slicing** to get substrings:

  text = "HelloWorld"
  print(text[0:5])  # Output: Hello
  
* Check if a substring exists:

  print("World" in text)  # True

---

 **Syntax:** string[start:end]
(start index is included, end index is excluded)

 **Try this:**

word = "education"
print(word[2:5])       # uca
print("cat" in word)   # True

---

 explanation of using **operators with strings** in Python:

---

## Using Operators with Strings

Python allows some operators to work with strings:

## `+` (Concatenation)

* Joins two strings:

  first = "Hello"
  second = "World"
  result = first + " " + second
  print(result)  # Output: Hello World
  
## `*` (Repetition)

* Repeats a string multiple times:

  text = "Hi "
  print(text * 3)  # Output: Hi Hi Hi 

## Comparison Operators

* Strings can be compared using `==`, `!=`, `<`, `>`, etc.

  print("apple" == "apple")  # True
  print("a" < "b")           # True
  
---

 **Tip:** Use `+` to build strings, and `*` to repeat patterns.

---

short example for **comparing strings**:

a = "apple"
b = "banana"

print(a == b)   # False
print(a < b)    # True (because "apple" comes before "banana")

 You can use `==`, `!=`, `<`, `>`, `<=`, `>=` to compare strings alphabetically.

---
## Comparing Strings in Python

> **Quick guide, perfect for dropping into a GitHub README.**

| Comparison   | What it checks                                               | Example                                       | Result |
| ------------ | ------------------------------------------------------------ | --------------------------------------------- | ------ |
| == / !=  | Exact equality / inequality                                  | "cat" == "cat"                                    | True   |
| < > <= >=  | Lexicographic (alphabetical) order, Unicode‐code‑point based | "apple" < "banana"                          | True |
| casefold() | Case‑insensitive equality (better than `lower()`)            | "straße".casefold() == "STRASSE".casefold() | True |
| in         | Substring membership                                         | "py" in "python"                            | True |

# basic equality
if user_input == secret_word:
    print("Match!")

# alphabetical sorting
words = ["Banana", "apple", "Cherry"]
print(sorted(words, key=str.casefold))  # ['apple', 'Banana', 'Cherry']

# case‑insensitive compare
if name.casefold() == "alice":
    ...

# natural‑order compare (e.g., file2 < file10)
import natsort
from natsort import natsorted
files = ["file10.txt", "file2.txt"]
print(natsorted(files))  # ['file2.txt', 'file10.txt']

>  **Remember**
>
> * `==` compares *contents*; `is` compares *object identity* (don’t use `is` for strings unless you really mean it).
> * Lexicographic order is Unicode‑based; for locale‑aware sorting (e.g., accented letters), use `locale.strxfrm` or a library like `PyICU`.

---

## Cheat‑sheet for quick reference

s1, s2 = "Python", "python"

equal        = s1 == s2              # False
ci_equal     = s1.casefold() == s2.casefold()  # True
before_after = s1 < s2               # True ('P' < 'p' in Unicode)
contains     = "tho" in s1           # True


Drop this snippet into your repo’s **docs** or **README.md** for an instant, developer‑friendly explanation of string comparison in Python.

---

## Example: Find Substring Within a String (Python)

text = "Python programming is fun"
if "programming" in text:
    print("Found!")

**Output:**

Found!

Use `in` to check if a substring exists.
Case-sensitive by default. Use `.lower()` or `.casefold()` for case-insensitive checks.

---

## String Functions in Python 

Python provides many **built-in string methods**. Here's a quick reference:

| Function                        | Description              | Example                                |
| ------------------------------- | ------------------------ | -------------------------------------- |
| len()                           | Returns string length    | len("Hello") → 5                     |
| .lower() / .upper()             | Changes case             | "Hi".lower() → "hi"                  |
| .strip()                      | Removes spaces           | "  text  ".strip() → "text"          |
| .replace()                    | Replaces part of string  | "a-b".replace("-", ":") → "a:b"      |
| .split()                      | Splits into list         | "a,b,c".split(",") → ['a', 'b', 'c'] |
| .find()                       | Finds index of substring | "hello".find("l") → 2                |
| .count()                      | Counts substring         | "hello".count("l") → 2               |
| .startswith() / .endswith() | Checks start/end         | "file.txt".endswith(".txt") → True"  |

## Example:

message = " Hello Python! "
print(message.strip().lower().replace("python", "world"))

**Output:**

hello world!

>  Most string methods **don't change the original string** — they return a **new string**.
> You can chain methods like `.strip().lower()` for clean processing.

---

## Example: Using String Functions in Python (GitHub-Friendly)

name = "  Hello World!  "

# Clean and format the string
cleaned = name.strip().lower().replace("world", "Python")
print(cleaned)

**Output:**

hello python!

 **Used functions:**

* .strip() → removes spaces
* .lower() → converts to lowercase
* .replace() → replaces text

---

##Example: Boolean Function in Python (GitHub-Friendly)

def is_even(n):
    return n % 2 == 0

print(is_even(4))   # True
print(is_even(7))   # False

 **Explanation**:

* is_even() returns a **boolean** (True or False)
* You can use it in conditions like if is_even(x): ...

---
 Here's a **short quiz** on **string manipulation** in Python:
---

## **Quiz: String Manipulation**

**Question:**
What will be the output of the following code?

text = " Hello, Python! "
result = text.strip().replace("Python", "World").upper()
print(result)

**Options:**
A) HELLO, PYTHON!
B) HELLO, WORLD!
C) HELLO, WORLD!
D) Hello, World!

---

** Answer:** **B) HELLO, WORLD!**

**Explanation:**

* strip() removes spaces
* replace("Python", "World") replaces the word
* upper() converts to uppercase

---

Sure! Here's a **short quiz** on **string indexing** in Python:

---

## **Quiz: String Indexing**

**Question:**
What will be the output of the following code?

text = "Python"
print(text[3])

**Options:**
A) h
B) t
C) o
D) n

---

** Answer:** **A) h**

**Explanation:**

* Indexing starts at 0
* text[3] gives the **4th character**, which is 'h' in "Python"

---

Sure! Here's a **short explanation** of **conditional statements** in Python:

---

## Conditional Statements in Python 

Conditional statements let your program make decisions based on conditions.

## Syntax:

if condition:
    # code runs if condition is True
elif another_condition:
    # runs if previous is False and this is True
else:
    # runs if all conditions are False

## Example:

age = int(input("Enter your age: "))

if age >= 18:
    print("You are an adult.")
elif age > 12:
    print("You are a teenager.")
else:
    print("You are a child.")

---


Sure! Here's a **short explanation** of the **`if` statement** in Python:

---

# **if Statement **

The if statement is used to run code **only if a condition is True**.

## Syntax:

if condition:
    # code to run if condition is True

## Example:

age = 20

if age >= 18:
    print("You can vote.")

**Output:**
You can vote.

---

Use if to **control program flow** based on conditions. Let me know if you need elif and else too!

---

 a **short explanation** of the **if-else statement** in Python:

---

## **if-else Statement **

Use if-else to run **one block if a condition is True**, and another if it's False.

## Syntax:

if condition:
    # runs if condition is True
else:
    # runs if condition is False

### 🔍 Example:

age = 16

if age >= 18:
    print("Adult")
else:
    print("Minor")

**Output:**
Minor

---

 **short explanation** of **if-elif-else** in Python:

---

## **if-elif-else Statement **

Use if-elif-else to check **multiple conditions** in order.

## Syntax:

if condition1:
    # runs if condition1 is True
elif condition2:
    # runs if condition2 is True
else:
    # runs if none are True

## Example:

marks = 75

if marks >= 90:
    print("Grade A")
elif marks >= 60:
    print("Grade B")
else:
    print("Grade C")


**Output:**
Grade B

---

It checks top-down and runs the **first True block only**.

---

Sure! Here's a **short quiz** on the **`if` statement** in Python:

---

## **Quiz: if Statement**

**Question:**
What will be the output of this code?

x = 10

if x > 5:
    print("High")

**Options:**
A) High
B) Low
C) Error
D) Nothing is printed

---

** Answer:** **A) High**

**Explanation:**
The condition x > 5 is True, so "High" is printed.

---

 Here's a **short quiz** on the **`if-elif` statement**:

---

## **Quiz: if-elif Statement**

**Question:**
What will be the output of this code?

num = 0

if num > 0:
    print("Positive")
elif num == 0:
    print("Zero")

**Options:**
A) Positive
B) Zero
C) Negative
D) Nothing is printed

---

**✅ Answer:** **B) Zero**

**Explanation:**

* num > 0 is False
* num == 0 is True, so "Zero" is printed.

---

Sure! Here's a **short quiz** on **logical operators** in Python:

---

## **Quiz: Logical Operator**

**Question:**
What will be the output of the following code?

x = 10
y = 5

if x > 5 and y < 10:
    print("Condition True")
else:
    print("Condition False")

**Options:**
A) Condition True
B) Condition False
C) Error
D) No output

---

** Answer:** **A) Condition True**

**Explanation:**

* x > 5 → True
* y < 10 → True
* True and True → True

---

**short explanation** of **loop statements** in Python:

---

## **Loop Statements in Python **

Loops are used to **repeat a block of code** multiple times.

---

## `for` Loop

Used to iterate over a sequence (like list, string, range).

for i in range(5):
    print(i)

**Output:**
0 1 2 3 4

---

## `while` Loop

Repeats **as long as** the condition is True.

i = 0
while i < 5:
    print(i)
    i += 1

**Output:**
0 1 2 3 4

---

Use break to stop a loop early, and continue to skip an iteration.

---

 **short explanation** of the **`while` loop** in Python:

---

## **while Loop (Short)**

The while loop runs a block of code **as long as a condition is `True`**.

## Syntax:

while condition:
    # code to repeat

## Example:

i = 1
while i <= 3:
    print(i)
    i += 1

**Output:**
1 2 3

---

Use while when you don't know how many times to repeat in advance.

---

 Short example using `while True` in Python:

# Infinite loop until user types 'exit'
while True:
    user_input = input("Type something (or 'exit' to quit): ")
    if user_input.lower() == 'exit':
        print("Exiting the loop. Goodbye!")
        break
    else:
        print("You typed:", user_input)

## Explanation:

* while True: creates an infinite loop.
* The break statement is used to exit the loop when the user types "exit".

This format is beginner-friendly and commonly used for input-based loops.

---

 **short example** of the break statement in Python 

# Example: Break statement in a loop

while True:
    user_input = input("Type 'exit' to stop: ")
    if user_input == "exit":
        break
    print("You typed:", user_input)

print("Loop ended.")

### 🔹 What it does:

* Keeps asking for input.
* Breaks the loop if the user types "exit".

---

 A **short example** of the `continue` statement in Python

# Example: Continue statement in a loop

for num in range(1, 6):
    if num == 3:
        continue  # Skip number 3
    print("Number:", num)

## What it does:

* Loops from 1 to 5.
* Skips printing number 3 using continue.

  ---

  A **short example** of the `pass` statement in Python 

# Example: Pass statement in a loop

for num in range(5):
    if num == 2:
        pass  # Placeholder for future code
    print("Number:", num)

## What it does:

* Loops through 0 to 4.
* When num is 2, it does nothing and continues — pass acts as a placeholder.

---

## `for` Loop in Python — *Short Explanation*

A **for loop** is used to **repeat a block of code** a certain number of times, usually when working with **sequences** like lists, strings, or ranges.

## Basic Syntax:

for variable in sequence:
    # code to repeat

## Example 1: Loop through a list

fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

## Example 2: Loop using `range()`

for i in range(5):
    print(i)

This prints: 0 1 2 3 4

## Key Points:

* The loop **automatically moves** to the next item.
* Stops when all items are covered.
* Use range() to repeat something **fixed number of times**.

---

Example of the range() function with **one parameter** in a `for` loop:

for i in range(5):
    print(i)

### Output:

0
1
2
3
4

 **Explanation**:
range(5) generates numbers from `0` to `4` (not including 5).

---

Example of `range()` with **two parameters**:

for i in range(2, 6):
    print(i)

## Output 

2
3
4
5

**Explanation**:
range(2, 6) starts from 2 and goes up to 5 (6 is not included).

---

An example of `range()` with **three parameters**:

for i in range(1, 10, 2):
    print(i)

### Output:

1
3
5
7
9

 **Explanation**:
range(start, stop, step)
This means: start at 1, go up to (but not include) 10, increment by 2.

---

 A simple **quiz question** for the `while` loop:

---

## **Quiz: What will be the output of the following code?**

x = 0
while x < 3:
    print(x)
    x += 1

**A.** 0 1 2 3
**B.** 0 1 2
**C.** 1 2 3
**D.** Infinite loop

**Correct Answer:** **B. 0 1 2**

---

A short quiz on the **`break` statement** in Python:

---

** Quiz: What will be the output of the following code?**

for i in range(5):
    if i == 3:
        break
    print(i)

**A.** 0 1 2 3
**B.** 0 1 2
**C.** 1 2 3
**D.** 0 1 2 3 4

---

** Correct Answer: B. 0 1 2**

> The loop **breaks when `i` is 3**, so it doesn’t print 3. Only 0, 1, and 2 are printed.

---

A short quiz on the **`continue` statement** in Python:

---

** Quiz: What will be the output of the following code?**

for i in range(5):
    if i == 2:
        continue
    print(i)

**A.** 0 1 2 3 4
**B.** 0 1 3 4
**C.** 1 2 3 4
**D.** 0 1 2 4

---

** Correct Answer: B. 0 1 3 4**

> The continue skips the iteration when i == 2, so **2 is not printed**.

---

A short quiz on the **`pass` statement** in Python:

---

** Quiz: What will be the output of the following code?**

for i in range(3):
    if i == 1:
        pass
    print(i)

**A.** 0 1 2
**B.** 0 2
**C.** 1
**D.** 0 1

---

** Correct Answer: A. 0 1 2**

> The `pass` statement **does nothing** — it's just a placeholder. So the loop runs normally and prints all values.

---

A quiz on the **`for` loop with `range()` using one parameter**:

---

** Quiz: What will be the output of the following code?**

for i in range(4):
    print(i)

**A.** 1 2 3 4
**B.** 0 1 2 3
**C.** 0 1 2 3 4
**D.** 1 2 3

---

** Correct Answer: B. 0 1 2 3**

> `range(4)` generates numbers starting from **0 up to 3** (but **not including 4**).

---

A quiz on the **`for` loop with `range()` using two parameters**:

---

** Quiz: What will be the output of the following code?**

for i in range(2, 6):
    print(i)

**A.** 2 3 4 5 6
**B.** 2 3 4 5
**C.** 3 4 5 6
**D.** 1 2 3 4 5

---

** Correct Answer: B. 2 3 4 5**

> range(2, 6) starts from **2** and goes **up to but not including 6**.

Need one for range() with **three parameters** next?

---

A quiz on the **`for` loop with `range()` using three parameters**:

---

** Quiz: What will be the output of the following code?**

for i in range(1, 10, 3):
    print(i)

**A.** 1 4 7 10
**B.** 1 3 6 9
**C.** 1 4 7
**D.** 1 4 7 9

---

** Correct Answer: D. 1 4 7 9**

> range(1, 10, 3) starts at **1**, ends **before 10**, and increases by **3** each step → 1, 4, 7, 10 (but 10 is not included), so result is **1, 4, 7, 9**.

---

A ** explanation of **lists in Python**:

---

## Python Lists – Quick Overview

A **list** in Python is a **collection of items** that is **ordered**, **changeable (mutable)**, and **allows duplicates**.

## Creating a List

fruits = ["apple", "banana", "cherry"]

## Accessing Items

print(fruits[0])  # Output: apple
print(fruits[-1]) # Output: cherry (last item)


## Modifying Items

fruits[1] = "orange"
print(fruits)  # ['apple', 'orange', 'cherry']

## List Operations

fruits.append("mango")       # Add to end
fruits.insert(1, "grape")    # Insert at position
fruits.remove("apple")       # Remove item

## Looping Through List

for fruit in fruits:
    print(fruit)

## Length of List

print(len(fruits))  # Number of items

## List with Mixed Data

my_list = [1, "hello", 3.14, True]

---

** Tip:** Lists are defined using square brackets `[]` and are one of the most flexible data structures in Python.

---

A **short example** of declaring and displaying a list in Python:

# Declaring a list
numbers = [10, 20, 30, 40]

# Displaying the list
print(numbers)

**Output:**

[10, 20, 30, 40]

---

A  **simple example** of displaying a specific element from a list:

# List of fruits
fruits = ["apple", "banana", "cherry"]

# Display the second element
print(fruits[1])

**Output:**

banana

>  Remember: List indexing starts at **0**, so `fruits[1]` gives the **second** item.

---

A **simple example** to display **all elements** in a list using a loop:

# List of fruits
fruits = ["apple", "banana", "cherry"]

# Display all elements
for fruit in fruits:
    print(fruit)

**Output:**

apple
banana
cherry

>  This is the most common way to loop through and print all items in a list.

---

A **short explanation** on **list modification** in Python:

---

## List Modification in Python

You can **change** list items because lists are **mutable**.

## Modify an Item

fruits = ["apple", "banana", "cherry"]
fruits[1] = "orange"
print(fruits)  # ['apple', 'orange', 'cherry']

## Add Items

fruits.append("mango")       # Add to end
fruits.insert(1, "grape")    # Add at position

## Remove Items

fruits.remove("apple")       # Remove by value
fruits.pop()                 # Remove last item

>  Lists can grow, shrink, and change — great for dynamic data!

---

 A **short explanation** on **adding elements to a list** in Python:

---

## Adding Elements to a List

## 1. `append()` – Add to the end

fruits = ["apple", "banana"]
fruits.append("cherry")
print(fruits)  # ['apple', 'banana', 'cherry']

## 2. `insert()` – Add at a specific position

fruits.insert(1, "orange")
print(fruits)  # ['apple', 'orange', 'banana', 'cherry']

## 3. `extend()` – Add multiple items from another list

fruits.extend(["mango", "grape"])
print(fruits)  # ['apple', 'orange', 'banana', 'cherry', 'mango', 'grape']

>  Use `append()` for single items, `extend()` for adding multiple, and `insert()` to control position.

---

A **short explanation** on **removing elements** from a list in Python:

---

## Removing Elements from a List

## 1. `remove(value)` – Removes the first matching item

fruits = ["apple", "banana", "cherry"]
fruits.remove("banana")
print(fruits)  # ['apple', 'cherry']

## 2. `pop(index)` – Removes by position (default: last item)

fruits.pop()        # Removes 'cherry'
fruits.pop(0)       # Removes 'apple'

## 3. `del` – Deletes by index or entire list

fruits = ["apple", "banana"]
del fruits[1]       # Deletes 'banana'
# del fruits         # Deletes the whole list

## 4. `clear()` – Empties the list

fruits.clear()
print(fruits)       # []


>  Use `remove()` by value, `pop()` or `del` by index, and `clear()` to wipe everything.

---

A explanation of **other common list functions** in Python:

---

## Other Useful List Functions in Python

## `len()` – Get number of items

fruits = ["apple", "banana", "cherry"]
print(len(fruits))  # Output: 3

---

## `sort()` – Sorts list in ascending order (modifies original)

numbers = [5, 2, 9, 1]
numbers.sort()
print(numbers)  # [1, 2, 5, 9]

---

## `sorted()` – Returns a sorted copy of the list

nums = [3, 1, 4]
print(sorted(nums))  # [1, 3, 4]
print(nums)          # [3, 1, 4] (original unchanged)

---

## `reverse()` – Reverses the list in place

fruits.reverse()
print(fruits)  # ['cherry', 'banana', 'apple']

---

## `index(value)` – Finds the index of a value

fruits = ["apple", "banana", "cherry"]
print(fruits.index("banana"))  # Output: 1

---

## `count(value)` – Counts how many times a value appears

nums = [1, 2, 2, 3]
print(nums.count(2))  # Output: 2

---

>  These functions help manage, search, and manipulate lists efficiently.

---

A **short and clear explanation** on **adding elements to a list** in Python:

---

## Adding Elements to a List in Python

You can add items to a list using **three main methods**:

---

## 1. `append()` – Add a single item to the **end** of the list

fruits = ["apple", "banana"]
fruits.append("cherry")
print(fruits)  # ['apple', 'banana', 'cherry']

---

## 2. `insert(index, item)` – Add item at a **specific position**

fruits.insert(1, "orange")
print(fruits)  # ['apple', 'orange', 'banana', 'cherry']

---

## 3. `extend()` – Add **multiple items** from another list

fruits.extend(["mango", "grape"])
print(fruits)  # ['apple', 'orange', 'banana', 'cherry', 'mango', 'grape']

---

>  Use `append()` for one item, `insert()` to control position, and `extend()` to add many at once.

---

A **simple example** of adding an element to the **end** of a list using `append()`:

# Original list
fruits = ["apple", "banana"]

# Add an element to the end
fruits.append("cherry")

# Display the updated list
print(fruits)

**Output:**

['apple', 'banana', 'cherry']

>  `append()` always adds the item to the **end** of the list.

---

A **simple example** of adding an element to a **specific position** in a list using `insert()`:

# Original list
fruits = ["apple", "banana", "cherry"]

# Insert 'orange' at index 1
fruits.insert(1, "orange")

# Display the updated list
print(fruits)

**Output:**

['apple', 'orange', 'banana', 'cherry']

>  `insert(index, item)` places the item **before** the given index.

---

A simple example of **adding multiple elements (a list) to another list** using `extend()`:

---

## Example: Add a list to another list

# Original list
fruits = ["apple", "banana"]

# New list to add
more_fruits = ["cherry", "mango"]

# Add all elements from more_fruits to fruits
fruits.extend(more_fruits)

# Display the updated list
print(fruits)

**Output:**

['apple', 'banana', 'cherry', 'mango']


>  `extend()` adds each item from the second list to the first one — not as a sublist.

---

## Bonus Tip: What if you use `append()` with a list?

fruits = ["apple", "banana"]
fruits.append(["cherry", "mango"])
print(fruits)

**Output:**

['apple', 'banana', ['cherry', 'mango']]

>  `append()` adds the **whole list as a single item**, not individual elements.

---

A **short and clear explanation** on **removing elements from a list** in Python:

---

## Removing Elements from a List in Python

Python provides **multiple ways** to remove items from a list:

---

## 1. `remove(value)` – Removes the **first occurrence** of the given value

fruits = ["apple", "banana", "cherry"]
fruits.remove("banana")
print(fruits)  # ['apple', 'cherry']

---

## 2. `pop(index)` – Removes the item at a **specific index**

(If index is not given, removes the **last** item)

fruits = ["apple", "banana", "cherry"]
fruits.pop(1)
print(fruits)  # ['apple', 'cherry']

fruits.pop()
print(fruits)  # ['apple']

---

## 3. `del` – Deletes item by index or the entire list

fruits = ["apple", "banana", "cherry"]
del fruits[0]
print(fruits)  # ['banana', 'cherry']

# del fruits  # Deletes the entire list

---

## 4. `clear()` – Removes **all items** from the list

fruits = ["apple", "banana"]
fruits.clear()
print(fruits)  # []

---

>  Use:

* `remove()` when you know the **value**
* `pop()` or `del` when you know the **index**
* `clear()` to **empty the list**

---

A **simple example** of removing elements from a list using different methods:

---

## Example 1: Using `remove()`

fruits = ["apple", "banana", "cherry"]
fruits.remove("banana")
print(fruits)  # ['apple', 'cherry']

---

## Example 2: Using `pop()`

fruits = ["apple", "banana", "cherry"]
fruits.pop(1)          # Removes item at index 1
print(fruits)          # ['apple', 'cherry']

---

## Example 3: Using `clear()`

fruits = ["apple", "banana"]
fruits.clear()         # Removes all elements
print(fruits)          # []

>  `remove()` = by value
>  `pop()` = by index
>  `clear()` = remove all

---

 **removing an element by its position** using the `pop()` method:

# List of fruits
fruits = ["apple", "banana", "cherry", "date"]

# Remove the element at index 2 (which is "cherry")
removed_item = fruits.pop(2)

print("Removed:", removed_item)
print("Updated list:", fruits)

## Output:

Removed: cherry  
Updated list: ['apple', 'banana', 'date']

 pop(index) removes the item at the given position and returns it.
 If the index doesn't exist, it will raise an IndexError.

---

 **removing all elements from a list** using the `.clear()` method:

# Example: Removing all elements from a list

# Initial list
numbers = [10, 20, 30, 40, 50]

# Clear all elements from the list
numbers.clear()

# Output the result
print("List after clearing:", numbers)

## Output:

List after clearing: []

## Notes:

* .clear() removes **all elements** from the list.
* The list still exists but becomes **empty**.

---

 the **number of elements** in a list 

# Example: Find the number of elements in a list

numbers = [10, 20, 30, 40, 50]

# Use len() to find the number of elements
count = len(numbers)

print("Number of elements in the list:", count)

## Output:

Number of elements in the list: 5

---

**sort a list of strings alphabetically** 

# Example: Sort a list of strings alphabetically

fruits = ["banana", "apple", "cherry", "date"]

# Sort the list in alphabetical order
fruits.sort()

print("Sorted list:", fruits)

## Output:

Sorted list: ['apple', 'banana', 'cherry', 'date']

If you want to sort without changing the original list, use `sorted()` instead:

sorted_fruits = sorted(fruits)

---

**copy a list** (GitHub-friendly):

# Example: Copy a list

original_list = [1, 2, 3, 4, 5]

# Method 1: Using copy()
copied_list = original_list.copy()

print("Original List:", original_list)
print("Copied List:", copied_list)

## Output:

Original List: [1, 2, 3, 4, 5]
Copied List: [1, 2, 3, 4, 5]

## Other ways to copy a list:

# Method 2: Using slicing
copied_list = original_list[:]

# Method 3: Using list()
copied_list = list(original_list)

---

 The **number of times a specific element** appears in a list 

# Example: Count the number of times a specific element appears in a list

colors = ["red", "blue", "green", "red", "yellow", "red"]

# Count how many times "red" appears
red_count = colors.count("red")

print("Number of times 'red' appears:", red_count)

### Output:

 To find the **position (index) of an element** in a list 
 
# Example: Find the position of an element in a list

fruits = ["apple", "banana", "cherry", "date"]

# Find the index of "cherry"
position = fruits.index("cherry")

print("Position of 'cherry':", position)

## Output:

Position of 'cherry': 2

> ⚠ Note: Indexing starts from **0**, and `.index()` gives the position of the **first occurrence**.

---

 focused on displaying a list of freelancers (suitable for beginners):

---

## **Quiz: Display Freelancers**

You are given a list of freelancer names. Write a Python program to **display each freelancer name one by one** using a loop.

# Given list
freelancers = ["Alice", "Bob", "Charlie", "Diana"]

# TODO: Write code to display each freelancer's name

## Expected Output:

Alice
Bob
Charlie
Diana

---

Great! Here's a **Python quiz** for **modifying a list of freelancers**:

---

## **Quiz: Modify Freelancers List**

You are given a list of freelancers.
**Task:** Add a new freelancer "Eve" to the end of the list and remove "Charlie" from the list.

# Given list
freelancers = ["Alice", "Bob", "Charlie", "Diana"]

# TODO: Add "Eve" and remove "Charlie"

## Expected Output (after printing the list):

['Alice', 'Bob', 'Diana', 'Eve']

--- 

 To test copying a list of freelancers:

---

## **Quiz: Copy Freelancers List**

You are given a list of freelancers.
**Task:** Make a copy of the list and store it in a new variable called copied_freelancers. Then, print the copied list.

# Given list
freelancers = ["Alice", "Bob", "Charlie", "Diana"]

# TODO: Copy the list to 'copied_freelancers' and print it

## Expected Output:

['Alice', 'Bob', 'Charlie', 'Diana']

---

To **declare a dictionary in Python**, with examples.

---

## What is a Dictionary in Python?

A **dictionary** is a collection of **key-value pairs**.
It allows you to store and access data using **keys** instead of numeric indexes (like lists).

---

## **How to Declare a Dictionary**

# Syntax: dictionary = { key1: value1, key2: value2, ... }

# Example: A dictionary of freelancers and their skills
freelancer = {
    "name": "Alice",
    "skill": "Web Development",
    "experience": 3
    
}

---

## Accessing Value

print(freelancer["name"])        # Output: Alice
print(freelancer["experience"])  # Output: 3

---

## Common Dictionary Methods:

freelancer["location"] = "Chennai"   # Add new key-value
freelancer["experience"] = 4         # Update value
del freelancer["skill"]              # Remove a key

---

 To find values by keys in a dictionary :

# Example: Find values by keys in a dictionary

freelancer = {
    "name": "Alice",
    "skill": "Graphic Design",
    "experience": 5
}

# Access values using keys
print("Name:", freelancer["name"])
print("Skill:", freelancer["skill"])
print("Experience:", freelancer["experience"])

## Output:

Name: Alice
Skill: Graphic Design
Experience: 5

## Tip:

You can also use .get() to avoid errors if the key doesn’t exist:

print(freelancer.get("location", "Not available"))

---

 **print the price of a product** using a dictionary 

# Example: Print the price of a product

product = {
    "name": "Laptop",
    "brand": "Dell",
    "price": 55000
}

# Print the price of the product
print("Price of the product:", product["price"])

## Output:

Price of the product: 55000

---

To **display both keys and values** from a dictionary 

# Example: Display keys and values in a dictionary

product = {
    "name": "Smartphone",
    "brand": "Samsung",
    "price": 20000
}

# Display all keys and values
for key, value in product.items():
    print(key, ":", value)

## Output:

name : Smartphone
brand : Samsung
price : 20000

---

To **add elements to a dictionary** 

# Example: Adding elements to a dictionary

product = {
    "name": "Headphones",
    "brand": "Sony"
}

# Add a new key-value pair
product["price"] = 1500
product["warranty"] = "1 year"

# Display the updated dictionary
print(product)

## Output:

{'name': 'Headphones', 'brand': 'Sony', 'price': 1500, 'warranty': '1 year'}

---

Example of removing elements from a dictionary in Python:

## Example: Remove an element from a dictionary by key

# Sample dictionary
product_prices = {
    "apple": 30,
    "banana": 10,
    "orange": 25
}

# Remove the item with key 'banana'
removed_price = product_prices.pop("banana")

# Print the removed value and updated dictionary
print("Removed price:", removed_price)
print("Updated dictionary:", product_prices)

## Output:

Removed price: 10
Updated dictionary: {'apple': 30, 'orange': 25}

---

## Other Methods to Remove Elements:

1. **Using `del` keyword:**

del product_prices["apple"]

2. **Using `clear()` to remove all items:**

product_prices.clear()

---

A quiz on finding the number of elements in a dictionary:

---

## **Python Dictionary Quiz – Number of Elements**

## Question:

students = {
    "Alice": 85,
    "Bob": 90,
    "Charlie": 78,
    "David": 92
}

print(len(students))

## What will be the output?

A) 3
B) 4
C) 5
D) Error

---

## Answer:

**B) 4**

>  len() returns the number of **key-value pairs** in the dictionary.

---

A **short quiz** on printing dictionary elements:

---

## Quiz:

person = {"name": "John", "age": 25}

for k, v in person.items():
    print(k, ":", v)

What is the output?

A) name age
B) John 25
C)

name : John  
age : 25

D) Error

---

## Answer:

C

---

Explanation of how to **declare a function** in Python:

---

## Declaring a Function in Python

def greet():
    print("Hello, world!")

## Explanation:

* def → keyword to define a function
* greet() → function name (can be any valid name)
* : → colon to start the function block
* print(...) → code that runs when the function is called

## Call the function:

greet()

---

A example of a function that stores and displays **contact data**:

---

## Example: Contact Data Function

def contact_info():
    contact = {
        "name": "Arun Kumar",
        "phone": "+91-9876543210",
        "email": "arun@example.com",
        "city": "Chennai"
    }

    for key, value in contact.items():
        print(key.title() + ":", value)

# Call the function
contact_info()

---

## Output:

Name: Arun Kumar  
Phone: +91-9876543210  
Email: arun@example.com  
City: Chennai

---

 A explanation of a **function without arguments** in Python 

---

## Function Without Arguments

A function **without arguments** means it doesn't take any input when called.

## Example:

def say_hello():
    print("Hello, welcome!")

# Call the function
say_hello()

## Explanation:

* def say_hello(): → defines a function with **no parameters**.
* print(...) → code that runs when you call the function.
* say_hello() → calling the function to execute it.

---

A **simple example** of a **function with one argument** 

---

A simple example of a function with one argument

---

## Function with One Argument

def greet(name):
    print("Hello,", name)

# Call the function with an argument
greet("Arun")

## Output:

Hello, Arun

---

A **function with two arguments** in Python:

---

## Example: Function with Two Arguments

def add_numbers(a, b):
    result = a + b
    print("Sum:", result)

# Call the function
add_numbers(5, 3)

---

## Explanation:

* a and b are **parameters** (inputs).
* add_numbers(5, 3) passes **two arguments**.
* It prints: Sum: 8

---

A **function that returns a value** in Python:

---

## Function That Returns a Value

A function can **return a result** using the return keyword.

## Example:

def square(num):
    return num * num

# Store the result
result = square(4)
print("Square is:", result)

---

## Explanation:

* return num * num → sends the result back to where the function was called.
* result = square(4) → stores the returned value.
* Output: Square is: 16

---

A quiz based on a simple **function calculator** in Python:

---

## **Python Function Quiz – Calculator**

## Question:

def calculator(a, b, op):
    if op == "+":
        return a + b
    elif op == "-":
        return a - b
    else:
        return "Invalid operation"

print(calculator(10, 5, "-"))

## What is the output?

A) 5
B) 15
C) -5
D) Invalid operation

---

## Answer:

**A) 5**

>  The function returns 10 - 5 which is 5.

---

Sure! Here's a **short and clear explanation** of **exceptions** in Python:

---

## What are Exceptions?

**Exceptions** are errors that happen during program execution.
Python stops the program unless the error is **handled**.

---

## Example:

try:
    num = int(input("Enter a number: "))
    print(10 / num)
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Please enter a valid number.")

---

## Keywords:

* try: Code that might cause an error
* except: Handles the error
* ZeroDivisionError, ValueError: Common exception types

---

A explanation **syntax errors** in Python 

---

## What is a Syntax Error?

A **syntax error** happens when the Python code is **not written correctly** — it breaks the rules of the language.

---

## Example of Syntax Error:

# Missing colon (:) after if statement
if 5 > 3
    print("Hello")

## Output:

SyntaxError: expected ':'

---

## Fix:

if 5 > 3:
    print("Hello")

---

## Tip:

Syntax errors happen **before** the code runs. Python won’t run the program until the syntax is correct.

---

A explanation of **runtime errors** in Python 

---

## What is a Runtime Error?

A **runtime error** happens **while the program is running** — the syntax is correct, but something goes wrong during execution.

---

## Example of Runtime Error:

num = int(input("Enter a number: "))
print(10 / num)

## If user enters `0`:

ZeroDivisionError: division by zero

---

## Common Runtime Errors:

* ZeroDivisionError` → Dividing by 0
* ValueError → Wrong data type
* IndexError → List index out of range
* TypeError → Invalid operation on wrong types

---

## Fix with Try-Except:

try:
    print(10 / int(input("Enter a number: ")))
except ZeroDivisionError:
    print("Can't divide by zero!")

---

A explanation** of **logical errors** in Python 

---

## What is a Logical Error?

A **logical error** happens when the program **runs without crashing**, but the **output is wrong** due to a mistake in logic.

---

## Example of Logical Error:

def calculate_area(length, width):
    return length + width  # ❌ wrong logic (should be *)

# Expected: 20, but gives 9
print("Area:", calculate_area(4, 5))

## Output:

Area: 9

---

## Correct Logic:

def calculate_area(length, width):
    return length * width  # ✔️ correct logic

---

## Tip:

Logical errors are the **hardest to find** because there’s **no error message** — you must **test and debug** your code carefully.

---

A explanation of a **logical error**

---

## Logical Error

A **logical error** occurs when code runs without crashing but produces incorrect results. It means the **logic of the code is flawed**, not the syntax.

 **Example (Python):**

# Should calculate area of a rectangle
def area(length, width):
    return length + width  # Logical error: should be length * width

 **Note:** Logical errors are hard to spot because the program runs normally — you must test outputs carefully!

---

 **division by zero** to demonstrate **error handling** with `try` / `except` 

---

## Example: Handling Division by Zero in Python

def safe_divide(a, b):
    try:
        result = a / b
        print(f"Result: {result}")
    except ZeroDivisionError:
        print("Error: Cannot divide by zero.")

# Test cases
safe_divide(10, 2)   # Output: Result: 5.0
safe_divide(5, 0)    #  Output: Error: Cannot divide by zero.

## What’s Happening:

* `try`: runs code that might raise an error.
* `except ZeroDivisionError`: catches the specific error and handles it gracefully.

---

 Example of a **TypeError** in Python — along with how to handle it:

---

## Example: TypeError in Python

def add_numbers(a, b):
    return a + b

# This will cause a TypeError
result = add_numbers(5, "3")  #  Can't add int and str

## Output:

TypeError: unsupported operand type(s) for +: 'int' and 'str'

---

## Handling the TypeError

def add_numbers(a, b):
    try:
        return a + b
    except TypeError:
        print("Error: Both inputs must be numbers of the same type.")

# Test cases
print(add_numbers(5, 3))    #  Output: 8
print(add_numbers(5, "3"))  #  Output: Error message

---

 Example of an **IndexError**, and how to handle it:

---

## Example: IndexError in Python

fruits = ["apple", "banana", "cherry"]

# This will raise an IndexError
print(fruits[5])  #  Index 5 is out of range

## Output:

IndexError: list index out of range

---

## Handling the IndexError

def get_fruit(index):
    fruits = ["apple", "banana", "cherry"]
    try:
        return fruits[index]
    except IndexError:
        return "Error: Index out of range."

# Test cases
print(get_fruit(1))  #  Output: banana
print(get_fruit(5))  #  Output: Error message

---

## Example: Handling Multiple Exceptions

try:
    # This will raise a ZeroDivisionError
    result = 10 / 0
    
    # This will raise a NameError
    print(unknown_variable)

except ZeroDivisionError:
    print("You can't divide by zero!")

except NameError:
    print("A variable used was not defined.")

except Exception as e:
    print(f"An unexpected error occurred: {e}")

else:
    print("Everything worked fine!")

finally:
    print("This will always run.")

## What’s Happening:

* The code in the `try` block can raise different types of exceptions.
* We handle specific exceptions (`ZeroDivisionError`, `NameError`) separately.
* The `Exception` block is a generic catch-all for anything unexpected.
* `finally` runs no matter what — useful for cleanup (e.g., closing files or DB connections).

---

## Example: Using `finally` with File Handling

try:
    file = open("example.txt", "r")
    content = file.read()
    print("File content:")
    print(content)

except FileNotFoundError:
    print("The file was not found.")

finally:
    # This will run whether an exception occurred or not
    print("Closing the file (if it was opened).")
    try:
        file.close()
    except NameError:
        pass  # file was never opened

## Explanation:

* The `try` block attempts to open and read from a file.
* If the file doesn't exist, a `FileNotFoundError` is raised and handled.
* The `finally` block always executes — even if an exception was raised — ensuring resources are cleaned up (like closing the file).

---
##  Quiz: Zero Division Exception

**Question:**
What will be the output of the following code?

try:
    result = 10 / 0
    print("Result is:", result)
except ZeroDivisionError:
    print("You can't divide by zero!")

**A.** `Result is: 0`
**B.** `ZeroDivisionError`
**C.** `You can't divide by zero!`
**D.** `Program crashes`

---

**Correct Answer:**  **C.** `You can't divide by zero!`

---

## Quiz: IndexError Exception

**Question:**
What will be the output of the following code?

my_list = [10, 20, 30]
try:
    print(my_list[5])
except IndexError:
    print("Index out of range!")

**A.** `30`
**B.** `None`
**C.** `Index out of range!`
**D.** `Error in list`

---

**Correct Answer:  **C.** `Index out of range!`

---

## Quiz: General Exception Handling

**Question:**
What will be the output of the following code?

try:
    number = int("abc")
except:
    print("Something went wrong!")

**A.** `abc`
**B.** `Something went wrong!`
**C.** `ValueError`
**D.** `Program crashes`

---

**Correct Answer:  **B.** `Something went wrong!`

This is because the `int("abc")` raises a `ValueError`, and the `except` block catches it without specifying the error type.

---

## `import random` – Explanation

The `random` module in Python is used to **generate random numbers** or make **random selections**.

When you write:

import random

You are telling Python to **load the built-in `random` module**, so you can use its functions like:

---

## Common Uses:

| Function               | Description                                                  |
| ---------------------- | ------------------------------------------------------------ |
| `random.random()`      | Returns a random float between 0.0 and 1.0                   |
| `random.randint(a, b)` | Returns a random **integer** between `a` and `b` (inclusive) |
| `random.choice(list)`  | Randomly picks an element from a list                        |
| `random.shuffle(list)` | Randomly rearranges the items in a list                      |
| `random.uniform(a, b)` | Returns a random **float** between `a` and `b`               |

---

## Example:

import random

num = random.randint(1, 10)
print("Random number:", num)

This will print a **random number between 1 and 10**.

---

## `random.randrange()` – Explanation

The `random.randrange()` function is used to **generate a random number from a specific range**.
It works **like the `range()` function**, but picks one **randomly**.

---

## Syntax:

random.randrange(start, stop, step)

* `start` – (optional) the beginning of the range (default is 0)
* `stop` – (required) the end of the range (not included)
* `step` – (optional) the difference between numbers (default is 1)

---

## Example:

import random

num = random.randrange(1, 10)
print(num)

This will print a random number from **1 to 9** (10 is **not included**).

---

## Example with Step:

random.randrange(0, 20, 2)

This returns a random **even number** between 0 and 18.

---

A short example using `import random`:

import random

num = random.randint(1, 5)
print("Random number:", num)

🎲 **This prints a random number between 1 and 5.**

---

A example of  **dice roll simulator** using `random`:

import random

dice = random.randint(1, 6)
print("🎲 You rolled:", dice)

 **This simulates rolling a 6-sided dice.** Each run gives a number between **1 and 6**.

---

A example for rolling **two dice**:

import random

dice1 = random.randint(1, 6)
dice2 = random.randint(1, 6)

print("🎲 Dice 1:", dice1)
print("🎲 Dice 2:", dice2)

 This simulates rolling **two 6-sided dice**.

 ---

Explanation of **date and time**

---

## What is the `datetime` module?

It helps you:

* Get the current date and time
* Format date and time
* Do date/time calculations (like yesterday/tomorrow)
* Convert between strings and dates

---

## Importing the module:

import datetime

---

## Getting current date and time:

import datetime

now = datetime.datetime.now()
print("Current date and time:", now)

Output:

Current date and time: 2025-07-30 18:15:23.456789

---

## Get only date or time:

today = datetime.date.today()
print("Today's date:", today)

time_now = datetime.datetime.now().time()
print("Current time:", time_now)

---

## Creating a specific date or time:

d = datetime.date(2025, 7, 30)
print("Specific date:", d)

t = datetime.time(14, 30, 0)
print("Specific time:", t)

---

## Formatting date and time:

now = datetime.datetime.now()

formatted = now.strftime("%d-%m-%Y %H:%M:%S")
print("Formatted:", formatted)

**Common format codes:**

* `%d` = Day
* `%m` = Month
* `%Y` = Year
* `%H` = Hour
* `%M` = Minute
* `%S` = Second

---

## Doing date calculations:

from datetime import timedelta, date

today = date.today()
tomorrow = today + timedelta(days=1)
yesterday = today - timedelta(days=1)

print("Tomorrow:", tomorrow)
print("Yesterday:", yesterday)

---

## Converting string to date:

from datetime import datetime

date_str = "30-07-2025"
date_obj = datetime.strptime(date_str, "%d-%m-%Y")

print("Converted date:", date_obj)

---

 example for printing the **current date** in Python:

import datetime

# Get today's date
today = datetime.date.today()

# Print the current date
print("Today's date is:", today)

**Output:**

Today's date is: 2025-07-30

---

A example to print a **selected date**:

import datetime

# Create a selected date (Year, Month, Day)
selected_date = datetime.date(2025, 12, 25)

print("Selected date is:", selected_date)

**Output:**

Selected date is: 2025-12-25

You can change the values to any date you need.

---

A example of **updating a selected date** by **adding or subtracting days** using `timedelta`:

import datetime

# Original selected date
selected_date = datetime.date(2025, 12, 25)
print("Original date:", selected_date)

# Add 5 days
updated_date = selected_date + datetime.timedelta(days=5)
print("Updated date (after 5 days):", updated_date)

# Subtract 7 days
earlier_date = selected_date - datetime.timedelta(days=7)
print("Updated date (before 7 days):", earlier_date)

**Output:**

Original date: 2025-12-25
Updated date (after 5 days): 2025-12-30
Updated date (before 7 days): 2025-12-18

This is useful for calculating deadlines, future events, or past dates. Let me know if you want to update months or years too (that needs a different approach).

---

A example of **formatting a date** using `strftime`:

import datetime

# Get today's date
today = datetime.date.today()

# Format the date as DD-MM-YYYY
formatted_date = today.strftime("%d-%m-%Y")
print("Formatted date:", formatted_date)

**Output:**

Formatted date: 30-07-2025

---

## Common format codes:

* `%d` – Day (01 to 31)
* `%m` – Month (01 to 12)
* `%Y` – Year (4 digits)
* `%B` – Full month name (e.g., July)
* `%A` – Full weekday name (e.g., Wednesday)

## Example using full names:

formatted = today.strftime("%A, %d %B %Y")
print("Formatted date:", formatted)

**Output:**

Wednesday, 30 July 2025

---

A example for formatting the current date** in Python:

import datetime

# Get the current date
today = datetime.date.today()

# Format as DD/MM/YYYY
formatted_date = today.strftime("%d/%m/%Y")

print("Current date (formatted):", formatted_date)

**Output:**

Current date (formatted): 30/07/2025

---

## Other examples of formats:

# Format as Month Day, Year
print(today.strftime("%B %d, %Y"))  # July 30, 2025

# Format as YYYY-MM-DD
print(today.strftime("%Y-%m-%d"))  # 2025-07-30

---

A example for formatting the current time in Python:

import datetime

# Get current time
now = datetime.datetime.now()

# Format time as HH:MM:SS
formatted_time = now.strftime("%H:%M:%S")

print("Current time (formatted):", formatted_time)

**Output:**

Current time (formatted): 18:45:10

---

## Common time format codes:

* `%H` – Hour (00–23)
* `%I` – Hour (01–12)
* `%M` – Minute (00–59)
* `%S` – Second (00–59)
* `%p` – AM/PM

---

## Example with AM/PM format:

formatted_time_am_pm = now.strftime("%I:%M %p")
print("Time with AM/PM:", formatted_time_am_pm)

**Output:**

Time with AM/PM: 06:45 PM

---

A example to **format both current date and time** using `datetime` and `strftime`:

import datetime

# Get current date and time
now = datetime.datetime.now()

# Format date and time as: DD-MM-YYYY HH:MM:SS
formatted = now.strftime("%d-%m-%Y %H:%M:%S")

print("Formatted date and time:", formatted)

**Output:**

Formatted date and time: 30-07-2025 18:45:30

---

## Format codes used:

* `%d` – Day
* `%m` – Month
* `%Y` – Year
* `%H` – Hour (24-hour)
* `%M` – Minute
* `%S` – Second

---

 **Python quiz on date**:

---

## **Quiz:**

What will be the output of the following code?

import datetime

d = datetime.date(2023, 1, 15)
new_date = d + datetime.timedelta(days=10)
print("Updated date:", new_date)

## Options:

A) 2023-01-25
B) 2023-01-05
C) 2023-01-10
D) Error

---

A explanation of **files, directories, and the `os` module** in Python:

---

## **Files in Python**

Files are used to **store data** permanently (like `.txt`, `.csv`, etc.).

##  Basic file operations:

# Open a file
f = open("data.txt", "r")  # "r" = read, "w" = write, "a" = append

# Read from file
content = f.read()

# Close the file
f.close()

---

## **Directories (Folders)**

A directory is a **container** for files or other folders.

Example: `C:/Users/John/Documents/` is a directory path.

---

## **The `os` Module**

Python's `os` module lets you **interact with the file system**.

## Common `os` functions:

import os

# Get current directory
print(os.getcwd())

# List files and folders
print(os.listdir())

# Create a new folder
os.mkdir("new_folder")

# Check if a file or folder exists
print(os.path.exists("data.txt"))

---

To **create directories** (folders) in Python, you can use the `os` module.

---

## Basic Example – Create one directory

import os

# Create a single directory
os.mkdir("my_folder")

This will create a folder named `my_folder` in the current directory.

---

## Create nested directories (multiple levels)

import os

# Create nested folders like parent/child/grandchild
os.makedirs("parent/child/grandchild")

`os.makedirs()` creates all intermediate folders if they don't exist.

---

## Check before creating

import os

folder_name = "my_folder"

if not os.path.exists(folder_name):
    os.mkdir(folder_name)
    print("Folder created!")
else:
    print("Folder already exists.")

---

A example for creating a directory in Python using the `os` module:

import os

# Directory name
directory_name = "MyFolder"

# Create the directory
os.mkdir(directory_name)

print(f"Directory '{directory_name}' created successfully!")

**Note:**

* This will create the folder in the current working directory.
* If the folder already exists, Python will throw a `FileExistsError`.
* To create **nested directories**, use `os.makedirs()` instead.

---

A example for creating a **subdirectory** in Python:

import os

# Parent directory
parent_dir = "MainFolder"

# Subdirectory name
sub_dir = "SubFolder"

# Create the subdirectory path
path = os.path.join(parent_dir, sub_dir)

# Create subdirectory
os.makedirs(path)

print(f"Subdirectory '{sub_dir}' created inside '{parent_dir}' successfully!")

**Notes:**

* `os.makedirs()` will create both the parent folder and the subfolder if they don’t exist.
* If the folders already exist, it will raise an error unless you pass `exist_ok=True` like:

  os.makedirs(path, exist_ok=True)

---

A example to **check if a directory exists** in Python:

import os

# Directory name
directory_name = "MyFolder"

# Check existence
if os.path.exists(directory_name):
    print(f"Directory '{directory_name}' exists.")
else:
    print(f"Directory '{directory_name}' does not exist.")

**Tip:**
You can also check specifically if it’s a **directory** (not a file) using:

os.path.isdir(directory_name)

---

 Removing directories depends on **whether the directory is empty or contains files**.

---

##  **Removing an Empty Directory**

You can use `os.rmdir()` for an empty directory:

import os

os.rmdir("MyFolder")  # Deletes only if empty
print("Empty directory removed.")

 If the directory has files/subfolders, `os.rmdir()` will throw an error.

---

##  **Removing a Directory (with all contents)**

You can use `shutil.rmtree()` to delete a directory and everything inside it:

import shutil

shutil.rmtree("MyFolder")  # Deletes folder even if it has files/subfolders
print("Directory and its contents removed.")

 **Be careful!** `shutil.rmtree()` is permanent and cannot be undone.

---

##  **Safe Deletion (Check before Removing)**

It’s a good practice to check if the directory exists before removing:

import os
import shutil

folder = "MyFolder"

if os.path.exists(folder):
    shutil.rmtree(folder)
    print(f"Directory '{folder}' removed.")
else:
    print(f"Directory '{folder}' does not exist.")

---

A example for **removing an empty directory** in Python:

import os

# Directory name
directory_name = "MyFolder"

# Remove directory
os.rmdir(directory_name)

print(f"Directory '{directory_name}' removed successfully!")

**Note:**

* `os.rmdir()` works only if the directory is **empty**.
* If it has files or subdirectories, you need to use `shutil.rmtree()` instead.

Example for **removing a directory with files**:

import shutil

shutil.rmtree("MyFolder")
print("Directory and its contents removed successfully!")

---

let’s go step-by-step through **creating and working with files** in Python.

---

##  **Opening / Creating a File**

We use Python’s built-in `open()` function:

# open(filename, mode)
file = open("example.txt", "w")  # 'w' creates a new file or overwrites if exists
file.write("Hello, this is my first file!\n")
file.close()

 **Modes** in `open()`:

| Mode  | Meaning                                 |
| ----- | --------------------------------------- |
| "w" | Write (create new / overwrite)            |
| "a" | Append (create if not exists, add to end) |
| "r" | Read (must exist)                         |
| "x" | Create new file (error if exists)         |
| "b" | Binary mode (e.g., `"wb"`)                |
| "t" | Text mode (default, e.g., `"wt"`)         |

---

##  **Writing to a File**

with open("example.txt", "w") as file:
    file.write("Line 1\n")
    file.write("Line 2\n")

 Using `with` automatically closes the file.

---

##  **Reading from a File**

with open("example.txt", "r") as file:
    content = file.read()
    print(content)

Other ways to read:

file.readline()   # Read one line
file.readlines()  # Read all lines into a list

---

##  **Appending to a File**

with open("example.txt", "a") as file:
    file.write("This is an extra line.\n")

---

##  **Checking if a File Exists**

import os

if os.path.exists("example.txt"):
    print("File exists!")
else:
    print("File not found!")

---

##  **Deleting a File**

import os

if os.path.exists("example.txt"):
    os.remove("example.txt")
    print("File deleted.")

---

A example to **create a file** in Python:

# Create a new file (or overwrite if it exists)
file = open("myfile.txt", "w")
file.write("Hello! This is my new file.\n")
file.close()

print("File created successfully!")

**Tip:**
If you want to create a file only if it does **not** already exist, use the `"x"` mode:

# Create file, error if it already exists
file = open("myfile.txt", "x")
file.write("This file is created only once!\n")
file.close()

---

let’s break down **writing to an existing file** in Python.

---

##  **What “Writing” Means**

When you **write** to a file in Python using "w" mode:

* If the file exists → its contents are **erased** before writing new data.
* If the file does not exist → it will be created automatically.

---

##  **Example – Overwriting an Existing File**

# Writing to an existing file (overwrites old content)
with open("myfile.txt", "w") as file:
    file.write("This is new content.\n")
    file.write("The old content is gone.\n")

print("File updated successfully!")

✅ `with` automatically closes the file after writing.

---

##  **If You Don’t Want to Erase Existing Content**

Use "a" mode (**append**) instead:

# Append new content without erasing
with open("myfile.txt", "a") as file:
    file.write("This is an extra line.\n")

---

##  **Key Modes Recap**

| Mode  | Action                            |
| ----- | --------------------------------- |
| "w" | Overwrite (or create if not exists) |
| "a" | Append to the end                   |
| "x" | Create new file, error if exists    |

---

If you want, I can give you a **short table comparing "w" and "a" mode** so you can quickly remember which to use.

---

A simple example for **writing to a file** in Python:

# Open the file in write mode
with open("myfile.txt", "w") as file:
    file.write("Hello, world!\n")
    file.write("This is my first line in the file.\n")

print("Data written to file successfully!")

**Notes:**

* "w" mode will create the file if it doesn’t exist.
* If the file exists, `"w"` will **overwrite** its content.
* Always use `with` to ensure the file closes automatically.

---

The breakdown for **reading an existing file** in Python.

---

##  Opening a File for Reading

We use the open() function with "r" mode (**read mode**):

with open("myfile.txt", "r") as file:
    content = file.read()
    print(content)

* "r" means **read only** (file must already exist).
* If the file does **not** exist, Python raises a `FileNotFoundError`.

---

##  Reading Methods

| Method        | Description                                   |
| ------------- | --------------------------------------------- |
| read()      | Reads the **entire file** as one string.        |
| readline()  | Reads **one line** at a time.                   |
| readlines() | Reads all lines and returns them as a **list**. |

Example:

with open("myfile.txt", "r") as file:
    print(file.readline())   # First line
    print(file.readline())   # Second line

---

##  Reading Line-by-Line in a Loop

with open("myfile.txt", "r") as file:
    for line in file:
        print(line.strip())  # strip() removes extra spaces/newlines

---

##  Checking if a File Exists Before Reading

import os
if os.path.exists("myfile.txt"):
    with open("myfile.txt", "r") as file:
        print(file.read())
else:
    print("File not found!")

---

A example for **reading a file** in Python:

# Open the file in read mode
with open("myfile.txt", "r") as file:
    content = file.read()
    print(content)

**Notes:**

* "r" means **read mode** — the file must already exist.
* file.read() reads the **entire file** as one string.
* Using with ensures the file closes automatically after reading.

---

A example of reading a file **line by line** using a loop with readline():

# Open the file in read mode
with open("myfile.txt", "r") as file:
    line = file.readline()
    while line:
        print(line.strip())  # strip() removes extra spaces/newlines
        line = file.readline()

**How it works:**

1. readline() reads **one line at a time**.
2. The while line: loop keeps going until no more lines exist.
3. strip() cleans up newline characters at the end of each line.

---

A example for **listing all files and directories** in Python:

import os

# Path to list (current directory)
path = "."

# List all files and directories
items = os.listdir(path)

print("Files and Directories in", path, ":")
for item in items:
    print(item)

**Notes:**

* os.listdir(path) returns a **list** of names (files + directories) in the given path.
* "." means the **current directory**.
* To check whether an item is a file or directory, you can use `os.path.isfile()` and `os.path.isdir()`.

Example with filtering:

for item in items:
    if os.path.isfile(os.path.join(path, item)):
        print(f"File: {item}")
    else:
        print(f"Directory: {item}")

---

A example to check the **current operating system** in Python:

import os

# Get the name of the operating system
os_name = os.name
print("OS Name:", os_name)

# More detailed system info
import platform
print("System:", platform.system())
print("Release:", platform.release())

**Output example (Windows):**

OS Name: nt
System: Windows
Release: 10

**Notes:**

* os.name returns short codes like `"nt"` (Windows), `"posix"` (Linux/Mac).
* platform.system()` gives a readable OS name (`Windows`, `Linux`, `Darwin`).
* `platform.release()` shows the OS version/release.

---

A **quiz question** for creating a map (dictionary) in Python:

---

**Quiz:**
Which of the following is the correct way to create a dictionary (map) in Python that stores **country → capital** pairs?

A)
countries = ["India": "New Delhi", "France": "Paris"]

B)
countries = {"India": "New Delhi", "France": "Paris"}

C)
countries = ("India": "New Delhi", "France": "Paris")

D)
countries = {"India", "New Delhi", "France", "Paris"}

---

 **Correct Answer:** **B**
Because in Python, a dictionary is created using **curly braces `{}`** with **key: value** pairs.

---

A **quiz question** for creating and writing into a file in Python:

---

**Quiz:**
Which of the following correctly **creates** a file named `notes.txt` and **writes** `"Hello World"` into it?

A)
with open("notes.txt", "r") as file:
    file.write("Hello World")

B)
with open("notes.txt", "w") as file:
    file.write("Hello World")

C)
with open("notes.txt", "a") as file:
    file.read("Hello World")

D)
open("notes.txt", "x")
file.write("Hello World")

---

**Correct Answer:** **B**

* "w" mode creates the file if it doesn’t exist and writes data (overwrites if it exists).
* "r" mode cannot write, and `"a"` mode appends instead of overwriting.

---
