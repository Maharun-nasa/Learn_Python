# Python Learning Guide

**Date:** 12/01/26  
**Author:** Maharun Nasa

---

## 📚 Overview

This repository contains a comprehensive guide to **Python Basics** covering fundamental concepts, data types, operators, control flow, functions, object-oriented programming, and more. This is perfect for beginners starting their Python programming journey.

---

## 📋 Table of Contents

- [Python Learning Guide](#python-learning-guide)
  - [📚 Overview](#-overview)
  - [📋 Table of Contents](#-table-of-contents)
  - [🎯 Key Topics](#-key-topics)
    - [Python Variables](#python-variables)
    - [Data Types](#data-types)
    - [Type Conversion](#type-conversion)
    - [Print Function](#print-function)
    - [Python Booleans](#python-booleans)
    - [Python Operators](#python-operators)
      - [Arithmetic Operators](#arithmetic-operators)
      - [Comparison Operators](#comparison-operators)
      - [Logical Operators](#logical-operators)
    - [Comments in Python](#comments-in-python)
    - [User Input Method](#user-input-method)
    - [Python Collections](#python-collections)
      - [List](#list)
      - [Tuple](#tuple)
      - [Set](#set)
      - [Dictionary](#dictionary)
    - [Python If...Else](#python-ifelse)
    - [Python Loops](#python-loops)
      - [While Loop](#while-loop)
      - [For Loop](#for-loop)
      - [Loop Control Statements](#loop-control-statements)
    - [Define Your Own Function in Python](#define-your-own-function-in-python)
      - [Parameters and Arguments](#parameters-and-arguments)
      - [\*args (Arbitrary Arguments)](#args-arbitrary-arguments)
      - [\*\*kwargs (Arbitrary Keyword Arguments)](#kwargs-arbitrary-keyword-arguments)
      - [Return Values](#return-values)
    - [Python Lambda Function](#python-lambda-function)
    - [Array in Python](#array-in-python)
    - [Python Math](#python-math)
      - [Built-in Math Functions](#built-in-math-functions)
      - [Math Module](#math-module)
    - [Python Classes/Objects](#python-classesobjects)
    - [Python Inheritance](#python-inheritance)
    - [Python Iterators](#python-iterators)
    - [Exception / Try Except](#exception--try-except)
  - [🚀 Getting Started](#-getting-started)
    - [Requirements](#requirements)
  - [� Tips for Learning](#-tips-for-learning)
  - [📝 Topics Covered Summary](#-topics-covered-summary)

---

## 🎯 Key Topics

### Python Variables

A Python variable is a _reserved memory location_  (Just Like a box or container) to store values. Variables give data to the computer for processing.

Think of a variable like a **labeled box** where you can store information (like numbers or text). You can change what's inside the box anytime, that's why it's called 'variable'.

**Example:**
```python
a = 10
b = 15
c = 'Maharun'
print(a, b, c)
```

### Data Types

Python supports multiple data types:

| Category | Types |
|----------|-------|
| **Text** | `str` |
| **Numeric** | `int`, `float`, `complex` |
| **Sequence** | `list`, `tuple`, `range` |
| **Mapping** | `dict` |
| **Set** | `set`, `frozenset` |
| **Boolean** | `bool` |
| **Binary** | `bytes`, `bytearray`, `memoryview` |

### Type Conversion

Type casting converts a value from one data type to another:

```python
# int conversion
a = int(5)
b = int(3.8)
c = int("6")

# float conversion
x = float(5)
y = float("45.7")

# str conversion
d = str(5)
e = str(3.8)
```

### Print Function

Used to output data to the console:

```python
num1 = 567
num2 = 345
total = num1 + num2
print("Summation of num1 and num2 is :", total)
```

### Python Booleans

Returns `True` or `False` based on conditions:

```python
print(10 > 8)      # True
print(34 < 67)     # True
print(54 <= 78)    # True
```

### Python Operators

#### Arithmetic Operators
```python
a = 10
b = 30
print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
print("Modulus:", a % b)
print("Floor Division:", a // b)
print("Exponentiation:", a ** b)
```

#### Comparison Operators
- `==` (Equal)
- `!=` (Not Equal)
- `>` (Greater than)
- `<` (Less than)
- `>=` (Greater or equal)
- `<=` (Less or equal)

#### Logical Operators
- `and` - Both conditions must be true
- `or` - At least one condition must be true
- `not` - Negates the condition

### Comments in Python

- **Single-line comment:** Starts with `#`
- **Multi-line comment:** Uses triple quotes `'''` or `"""`

```python
# This is a single-line comment
''' This is a
    multi-line comment '''
```

### User Input Method

Take values from user using `input()`:

```python
number = int(input("Enter your number: "))
print(number)
print(type(number))
```

### Python Collections

#### List
Ordered, changeable, allows duplicates:
```python
l1 = ["red", "blue", "green"]
l1.append("yellow")
l1.remove("red")
```

#### Tuple
Ordered, unchangeable, allows duplicates:
```python
t1 = ('apple', 'mango', 'jackfruit')
print(t1[1])      # Access by index
print(t1[-1])     # Negative indexing
```

#### Set
Unordered, unindexed, no duplicates:
```python
s1 = {'apple', 'mango', 'jackfruit'}
s1.add('banana')
s1.remove('mango')
```

#### Dictionary
Unordered, changeable, indexed with keys:
```python
d1 = {
    'name': 'maharun',
    'roll': 1,
    'class': 12
}
print(d1['name'])
```

### Python If...Else

Conditional statements to execute code based on conditions:

```python
a = 23
b = 19

if a > b:
    print("a is greater than b")
elif a == b:
    print("a and b are equal")
else:
    print("b is greater than a")
```

**Logical conditions:**
- `and` - Both conditions true
- `or` - At least one condition true
- `not` - Reverses the result

### Python Loops

#### While Loop
```python
i = 1
while i < 5:
    print(i)
    i += 1
else:
    print('i is no longer less than 5')
```

#### For Loop
```python
fruits = ['apple', 'mango', 'jackfruit']
for x in fruits:
    print(x)

for a in range(2, 7):
    print(a)
```

#### Loop Control Statements

- **`pass`** - Placeholder, does nothing
- **`continue`** - Skip current iteration
- **`break`** - Exit the loop

```python
for x in fruits:
    if x == 'jackfruit':
        continue
    print(x)
```

### Define Your Own Function in Python

```python
def my_function():
    print("Hello World")

my_function()  # Calling the function
```

#### Parameters and Arguments
```python
def my_function(fname):  # fname = parameter
    print("Hello " + fname)

my_function("Maharun")  # "Maharun" = Argument
```

#### *args (Arbitrary Arguments)
```python
def my_function(*city):
    print("I live in " + city[1])

my_function('rajshahi', 'dinajpur', 'dhaka')
```

#### **kwargs (Arbitrary Keyword Arguments)
```python
def my_function(**lname):
    print("Last name is " + lname['lastname'])

my_function(firstname='maharun', lastname='nishi')
```

#### Return Values
```python
def my_function(x):
    return 5 * x

print(my_function(3))   # 15
```

### Python Lambda Function

Anonymous function using `lambda` keyword :

```python
add = lambda x: x + 5
print(add(10))  # 15

a = lambda x, y: x ** y
print(a(5, 3))  # 125
```

Lambda with user-defined functions:
```python
def my_function(n):
    return lambda x: x * n

my_doubler = my_function(2)
print(my_doubler(11))  # 22
```

### Array in Python

Arrays hold multiple values of the **same data type** :

```python
fruits = ['apple', 'banana', 'cherry', 'kiwi', 'mango']
print(fruits[1])           # Access element
fruits[0] = 'blackcurrant' # Modify
fruits.append('orange')    # Add item
fruits.pop(1)              # Remove by index
fruits.remove('kiwi')      # Remove by value
```

### Python Math

#### Built-in Math Functions

```python
x = max(10, 16, 25)        # Maximum value
y = min(10, 16, 25)        # Minimum value
z = abs(-7.25)             # Absolute value
p = pow(4, 3)              # Power function
```

#### Math Module

```python
import math

s = math.sqrt(64)          # Square root
x = math.ceil(2.6)         # Round up
y = math.floor(2.6)        # Round down
pi = math.pi               # Value of PI
```

### Python Classes/Objects

Object-oriented programming with classes:

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def myfunc(self):
        print("Hello my name is " + self.name)

p1 = Person("Maharun", 22)
p1.myfunc()
```

**Key concepts:**
- `__init__()` - Constructor, runs automatically
- `self` - Refers to the current instance
- Object properties can be modified or deleted

### Python Inheritance

Child class inherits from parent class:

```python
class Person:
    def __init__(self, fname, lname):
        self.firstname = fname
        self.lastname = lname
    
    def printname(self):
        print(self.firstname, self.lastname)

class Student(Person):
    pass

student = Student("Maharun", "Nishi")
student.printname()
```

### Python Iterators

Iterators traverse through values using `iter()` and `next()`:

```python
my_tuple = ("apple", "banana", "cherry")
myit = iter(my_tuple)
print(next(myit))  # apple
print(next(myit))  # banana

# Or use in loop
for x in my_tuple:
    print(x)
```

### Exception / Try Except

Handle errors gracefully:

```python
try:
    print(x)
except NameError:
    print("Variable x is not defined")
except:
    print("Something else went wrong")
else:
    print("Nothing went wrong")
finally:
    print("The try except is finished")
```

**Blocks:**
- `try` -  Test code for errors
- `except` - Handle the error
- `else` - Execute if no error
- `finally` - Execute regardless

---

## 🚀 Getting Started

1. **Clone or download** this repository
2. **Open the notebook** `python_basic_level.ipynb` in Jupyter Notebook or VS Code
3. **Execute cells** to see examples and output
4. **Modify and experiment** with the code to learn

### Requirements

- Python 3.x installed
- Jupyter Notebook or VS Code with Python extension

---

## 💡 Tips for Learning

- Read through each topic carefully
- Run all code examples to see output
- Modify examples and experiment
- Try solving simple problems using concepts learned
- Practice regularly for better retention

---

## 📝 Topics Covered Summary

✅ Variables and Data Types  
✅ Type Conversion  
✅ Operators (Arithmetic, Comparison, Logical)  
✅ Control Flow (if/elif/else)  
✅ Loops (while, for, with control statements)  
✅ Functions and Lambda  
✅ Collections (List, Tuple, Set, Dictionary)  
✅ Arrays and Methods  
✅ Math Operations and Module  
✅ Object-Oriented Programming (Classes, Inheritance)  
✅ Iterators  
✅ Exception Handling  

---

**Happy Learning!** 🎉
