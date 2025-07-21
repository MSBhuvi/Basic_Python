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









