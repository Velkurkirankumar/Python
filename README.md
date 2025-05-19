# April 15

### Programming
##### Approach
- Programs dont respond to make tea rather they expect instructions
- These instructions or the way we represent these instructions is referred as programming logic or algo etc.
- Note:
    - Never Write Program with out instructions
    - Programs fail
- Principle: Programming is 80% debugging and 20% writing
- Lets instruct chaitra

![image](https://github.com/user-attachments/assets/26a724ff-229d-4bf7-96ae-36685319799b)

- Chaitra knows + -
- Sample instruction
```
Hi chaitra
say 5 + 6
```

- Sample Response

11

- Sample Instruction

```
Hi Chaitra
remember 90 as maths
remember 80 as science
say maths + science
```

- Sample Response

170

- Write instructions for chaitra to calculate 3 * any number. Chaitra knows + -
```
Hello Chaitra
Remember 2 as number
say number + number + number
```
- Chaitra now knows + - * / // % ==
- Write instructions for chaitra to say if the number is even
```
Hello Chaitra
Remember 6 as number
calculate number %2 and remember as result
say even if result == 0
```
- Moral of story sofar
    - Learn to write instructions
    - Examine Instructions (debugging)
### How Programs are Executed on a System
- Typically we run our program on Operating Systems.
- Operating System allows us to
    - run custom applications
    - allows application to interacts with hardware with an abstracted interface
- Operating Systems creates a Process with a unique id, some ram & cpu allocated to it
- CPU w.r.t your program executes instructions and RAM stores values

#### Memory in RAM
- Data Types: The basic idea of data type is to allocate memory in a way convinient to developers.
    - Size
    - nature:
        - static size (mutable types)
        - dynamic size (immutable types)


## April 16

# Programming foundations
#### Chaitra knows how to + - * / // % == < >

![image](https://github.com/user-attachments/assets/1665bb39-5690-4f3d-99e6-6ba3079f68e6)

- Chaitra can rememeber values as long as you are referring with names

### Problem: Let solve the problem of area of circle

- Formulae: A=πr2

```
Hi chaitra
pi = 3.14
radius = 1
result = pi * radius * radius
say result
```

### Problem: Lets solve the problem of simple intrest

- inputs
    - principal
    - time (in years)
    - rate of intrest
- forumla: p * t * r / 100

```
Hi Chaitra
p = 10000000
t = 5
r = 24
si = p * t * r / 100
say si
```

### Problem: Lets solve the problem of Converting degrees into farnhiet

- Input: celcius
- Formuala: (C Ã— 9/5) + 32
- Chaitra evaluates operators according to python operator precedence
- Solution:

```
Hi Chaitra
c = 50
f = (c * (9 / 5)) + 32
```

## Operator Precedence

- This defines the priority

![image](https://github.com/user-attachments/assets/8a212e0c-e1ee-48e2-9b33-a76a4270b380)

### Problem

- Ask chaitra to say number 5 times

number = 5
repeat 5 times and rememeber count in index
    say number

- other

```
number = 5
index = 0
until index < 5 
    say number
    index += 1
```

- I want Chaitra to calculate gst on popcorn

```
popcorn = caramel
price = 1000
if popcorn == normal 
    tax = price * 5 / 100
if popcorn == salted
    tax = price * 12 / 100
if popcorn == caramel
    tax = price * 18 / 100

total = price + tax
say total
```

### Factorial of a number

- input = number
- solution

```
Hi Chaitra
number = 5
index = 1
factorial = 1
until index <= number
    factorial = factorial * index
    index = index + 1
say factorial
```

### Project euler 1
- Project euler
- Problem 1
- Solution

```
Hi chaitra
index = 1
result = 0
number = 10
until index < number
  is_multiple = (index % 3 == 0) or (index % 5 == 0)
  if is_multiple == True
    result = result + index
  index = index + 1
say result
```

### Project euler 2

- Lets solve fibonnaci sequence

```
a = 1
b = 2
say a
say b
max = 30
until (a + b) <= max
    c = a + b
    say c
    a = b
    b = c
```

## April 17

### Project euler 2

- Overview
- Lets solve fibonnaci sequence

```
a = 1
b = 2
say a
say b
max = 30
until (a + b) <= max
    c = a + b
    say c
    a = b
    b = c
```

- Now we need to find sum of even numbers

```
Hi Chaitra
a = 1
b = 2
sum = 2
max = 30
until (a + b) <= max
    c = a + b
    if c % 2 == 0
        sum = sum + c
    a = b
    b = c
```

### Leap Year
- Lets make chaitra to tell if the year is leap or not
- Leap Year Rules
    - A year is a leap year if it is divisible by 4.
    - However, if the year is also divisible by 100, it is NOT a leap year, unless…
    - The year is divisible by 400, then it IS a leap year.
- Summary:

```
If year % 400 == 0 â†’ Leap year

Else if year % 100 == 0 â†’ Not a leap year

Else if year % 4 == 0 â†’ Leap year

Else â†’ Not a leap year
```

- inputs: year
- Solution

```
Hi Chaitra
year = 1904
leap_year = false
if year % 4 == 0
    if year % 100 == 0 and year % 400 == 0:
        leap_year = true
    if year % 100 != 0
        leap_year = true

say leap_year
```

### Sum of digits
- Lets look at this problem

```
1530  => 1 + 5 + 3 = 9
7776  => 7 + 7 + 7 + 6 = 27 => 2 + 7 = 9
1827 => 1 + 8 + 2+ 7 = 18 => 1 + 8 => 9
7775 => 8
1234 = > 1
```

- Chaitra knows + - * / // % == != < > <= >=
- This problem involves two sub problems
    - pulling out individual digits
    - add all digits till the result is single digit
- pulling out individual digits

```
Hi Chaitra
number = 7776
result = 0
until number > 0
   digit = number % 10
   result = result + digit
   number = number // 10
   if number == 0 and result > 9:
      number = result
      result = 0
say result
```

### System Setup
- Level 1 Softwares:
    - Git
    - Python 3.11
    - Visual Studio Code
- Level 2 Softwares: After creating cloud accounts
- aws cli
- azure cli
- azure data studio


# April 19

### Debugging using visual studio code

- Breakpoint: This is where the code execution stops and we get control
- Step Over: This instructs the debugger to execute the current line
- Continue: We give control back to debugger
- Sections:
    - Variables
    - Watch
    - Call Stack

### References
- Gist link for individual code debugging practice
- To debug
    - copy the python code in a file (with .py extension) and preferably in a new folder debugging-practice
    - Start Debugging
- Findout the logical mistake in fibbonci problem

```
a = 1
b = 2
sum = 2
while a + b < 100:
    c = a + b
    if c % 2 == 0:
        sum = sum + c
    a = b
    b = c
print(sum)
```

# April 22

### Programming languages

- The idea of programming language was to make systems/computers perform custom tasks especially w.r.t applications
- Python is a language popular as it can be used in
    - Programming
    - Scripting
    - AI
    - Data
- Python has Zen of Python

![image](https://github.com/user-attachments/assets/b7896ad4-4506-4463-8e64-023f0b335413)

- Python is an Open Source Project, And any new feature into python comes as PEP (Python enhancement Proposal)
- Two import PEP’s
    - PEP-20: Zen of python
    - PEP-8: Style Guide
- References

### First steps into python
- Data types
    - int
    - float
    - str
    - bool
    - list
    - tuple
    - set
    - dict
- Python is dynamically typed language

### REPL (Read evaluate Print loop)

- Launch terminal
- Type python (python3 for mac/linux) & enter

![image](https://github.com/user-attachments/assets/7dced8a5-569f-4805-8656-9e86d8816421)

#### Built in functions
- print
- type
- id

### Python Hello world program
- Python code

```
print("Hello")

print("Welcome to python")
```

- Exercise:
    - Create a folder and python file
    - Execute
    - Debug

### Approach
- Data types
- Operators
- Instructions
- Syntax
- Code organization
- builtins
- types
- functions
- Standard Library
- Using external libraries or Packages
- Exceptions and Error Handling


### General References
- Websites
    - Real Python
    - Geek for Geeks
    - Programiz
    - W3Schools
- Books
    - Learning Python
    - Python in a Nutshell
    - Automating Boring Stuff with Python
    - Fluent Python
- AI Based Learning
    - Perplexity
    - Gemini
    - Chatgpt

### Data types
[Refer Here](https://www.programiz.com/python-programming/variables-datatypes)  for python data types

### Operators
- Operators
- Types:
    - Arthimetic
    - Assignment
    - Comparision
    - Logical
    - BitWise
    - Special Operators

### Playing with numeric data
[Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/datatypes-intro.ipynb)  for jupyter notebook


# April 23

## Naming conventions
- Pascal Casing: In this case every word starts with capital case
```
Value
MyValue
MyNewValue
```
- Camel Casing
```
value = "hello"
myValue = "hello"
myNewValue = "hello"
```

- Snake Casing
```
value = "hello"
my_value = "hello"
my_new_value = "hello"
```

- Capital Snake Casing
```
VALUE = "hello"
MY_VALUE = "hello"
MY_NEW_VALUE = "hello"
```

- In python for
    - variables we use snake casing
    - function names we use snake casing
    - class names we use Pascal Casing
    - constant values we use Capital Snake casing

### Spacing in python
- Consider the following
`10**3`

- It recommeneded to use
`10 ** 3`

### Indentation in python
- Python follows strict [indentation](https://www.geeksforgeeks.org/indentation-in-python/)

### Operators and Numeric Data types
- [Refer Here](https://www.programiz.com/python-programming/operators) for operators


### Doc Strings
- [Refer Here](https://www.programiz.com/python-programming/docstrings) for doc strings
### First Program
- Average of marks
- Topics
    - doc string
    - input
    - typecasting
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/average.py)

```
"""This program is to learn numeric types and its 
operators

Topics:
  input
  typecast
"""

maths = float(input("Enter maths marks: "))
science = float(input("Enter science marks: "))
social = float(input("Enter social marks: "))
average = (maths + science + social) / 3
print(average)
```

- Write a program to calculate compound intrest

### Conditional expressions
- comparision operators
- logical operators

### Conditionals
- if statement  
```
if <conditional-expression>:
   ....
   ....
```

- if else

```
if <conditional-expression>:
   ....
   ....
else:
   ....
   ....
```

- if elif else

```
if <conditional-expression>:
   ....
   ....
elif <conditional-expression>:
   ....
   ....
elif <conditional-expression>:
   ....
   ....
else:
   ....
   ....
```

- Program to print different id cards according to age in india


| Minimum Age    | Identity Cards                                                        |
|----------------|----------------------------------------------------------------------|
| Birth          | Birth Certificate, Aadhaar Card (can be obtained for newborns)       |
| Any Age        | Passport, PAN Card, Bank/Post Office Passbook                        |
| Enrolled       | School/College ID Card (for currently enrolled students)             |
| No specific age| Ration Card                                                          |
| 18 years       | Voter ID Card (EPIC), Driving License                                |
| 60 years       | Senior Citizen Card (eligibility criteria might vary slightly by state) |

```
age = int(input("Enter your age: "))
print("You are eligbile for ")
print("Birth Certificate \nAadhaar Card \nPassport \nPAN Card \nBank/Post Office Passbook")
if age >= 18:
    print("Voter ID Card (EPIC) \nDriving License")
if age >= 60:
    print("Senior Citizen Card")
```

### looping
- In python we have two approaches
    - while
    - for

- while
    - [while](https://www.programiz.com/python-programming/while-loop)
- Syntax

```
while <conditional-expression>:
   ...
   ...
   ...
```

- To exit out of while loop we have two options
    - conditonal expression becoming false
    - break keyword


# April 24

### Looping constructs while contd

#### Project euler 3
- [Refer](https://projecteuler.net/problem=3) Here for problem
- Largest prime factor of a number
    - it has to be a factor
    - it has to be a prime
    - it has to be a largest possible
- Example
```
70 =>
   factors: 2,5,7,10,14,35
   prime: 2,5,7
   largest: 7

27 =>
   factors: 3,9
   prime: 3
   largest: 3
```

- Solution for prime number
```
Hi Chaitra,
number = 7
is_prime = True
index = 2
while index < number
   if number%index == 0
      is_prime = False
      break
   index = index + 1
```

- Python
```
number = 13195
factor = number // 2
while factor > 1:
    # check if it is factor
    if number % factor == 0:
        # if factor also check if index it is prime
        is_prime = True
        index = 2
        while index <= factor//2 :
            if factor % index == 0:
                is_prime = False
                break
            index = index + 1
        if is_prime:
            print(factor)
            break
    factor = factor - 1
```

- Project euler 5
- [Refer Here](https://projecteuler.net/problem=5)

- Python
```
# Smallest multiple
number = 20

# boundary
index = 1
factorial = 1
while index <= number:
    factorial = factorial * index
    index += 1

max = factorial
index = number
while index <= factorial:
    # check if is divisible by all numbers from 2 to number
    divisible = True
    number_index = 2
    while number_index <= number:
        if index % number_index != 0:
            divisible = False
            break
        number_index += 1
    if divisible:
        print(index)
        break
    index += number
```


### Project euler 6: Sum square difference
- [Refer Here](https://projecteuler.net/problem=6)

```
# Project euler problem 6

number = 100

sum = (number * (number + 1)) // 2

square_sum = sum ** 2

square_number = 0
index = 1
while index <= number:
    square_number += index ** 2
    index += 1
print(square_sum - square_number)
```


# April 26

## Sequence Types
- All the sequence types can hold multiple values in it
- Sequence types supports indexes where we have positive and negative indexes

![image](https://github.com/user-attachments/assets/6b219153-7b30-43f6-92ee-175aa32473c5)

![image](https://github.com/user-attachments/assets/a494eb74-7736-4f9c-a0f5-05803b312798)

- All sequence types support len function
- Sequence types support slicing start-index:stop-index:step
    - start-index: default value is 0
    - stop-index: default value is length
    - step: it has default value of 1
- [Refer Here](https://www.programiz.com/python-programming/variables-datatypes) for data types
- Sequence types:
    - list
    - tuple
    - range: it is used to create sequences
- list:
    - can hold multiple types
    - is mutable
    - syntax: []
- tuple:
    - can hold multiple types
    - are immutable
    - syntax: ()
- We can convert between list and tuple
- We can loop through lists, tuple using while
- For loop in python [Refer Here](https://www.programiz.com/python-programming/for-loop)

```
for item in items:
    print(item)
```

- [Range](https://www.programiz.com/python-programming/methods/built-in/range): This is used to generate number sequences
- Python set: [Refer Here](https://www.programiz.com/python-programming/set)
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/sequences.ipynb) for jupyter notebook

## Modules and Functions

- One of the major principle in programming in Reusability which revolves around DRY principle (Dont Repeat yourself)
- Module is a python file
- Function is a reusable code which exists in a module
- modules can be reused or functions, classes or variables in module can be reused
- To document modules and functions lets use docstrings, Lets use [Google’s style guide](https://google.github.io/styleguide/pyguide.html) for this
- [Docstring for a module](https://google.github.io/styleguide/pyguide.html#382-modules)
- [Docstring for function and methods](https://google.github.io/styleguide/pyguide.html#383-functions-and-methods)
- [Functions](https://www.programiz.com/python-programming/function)
- To name a function we use snake casing
- Module can be used in two ways
    - executor:
        - we are executing the module python <module-name>.py
    - library:
        - other module imports and calls the reusable functions (or classes or variable)
- Module import options
- option 1: import
```
import utils

if utils.is_even(10):
    print("even")
```
- option 2: from import
```
from utils import is_even

if is_even(10):
    print("even")
```

- Whenever you see anything in python with double underscores (dunder) around it, it has special purpose and is defined by python.
- Lets discuss about a special dunder variable __name__ which will have two possible values
    - __main__ when the module is executed directly
    - module-name when module is imported

# April 27

### Functions contd
- Refer Here for functions
- Refer Here for jupyter notebook

### Exercise:
- Write a function to find the sum of numbers in number plate for numerology
```
9999 => 9 + 9 + 9 + 9 => 36 => 3 + 6 => 9
8273 => 8 + 2 + 7 + 3 => 20 => 2 + 0 => 2
```

- solution
```
def sum_digits(number):
    sum = 0
    while number > 0:
        digit = number % 10 
        sum = sum + digit
        number = number // 10
        if number == 0 and sum > 9:
            number = sum
            sum = 0
    return sum
```

### Modules and packages
- Refer Here for the package
- Refer Here for the sample package and using the package in the module main.py

### Finding methods for a type
- List methods
- Tuple methods
- set methods
- str methods

#### Problem
- Take a string as an input and return bool if the string is numeric
```
def is_numeric(value):
    return value.isnumeric()
```

- Type Hinting in Python
- expert usage of python functions
- object oriented programming
- str methods
- list methods


# April 28

- List, Tuple, set methods
- Refer Here for the list methods
- Refer Here for tuple methods
- Refer Here for set methods
- Membership operators:
    - in
    - not in
- Refer Here for the jupyter notebook created in the class

### Dictionary
- Python dictionaries contain key value pairs.
- Keys must be unique
- Keys must be immutable
- Refer Here for python dictionary
- Refer Here for dictionary methods
- Refer Here for the jupyter notebook created in the class

### Python strings
- Refer Here for strings
- Refer Here for sample notebook written

# April 29

## Procedural Programming
- Procedural Programming is like a recipe
    - inputs
    - steps (sequence)
    - output

### Object Oriented Programming
- Object:
    - contains
    - capabilities

#### Examples
- Bank Account
```
BankAccount
  contains:
     account number
     account type
     balance
  characteristics:
    transfer
    withdraw
    deposit
```        

- Laptop
```
contains:
  configuration
     cpu
     ram
     storgae
  os
  features
characteristics:
  start
  shutdown
  browser
  ...
  ...
```

- Library
```
book
shelf
newspaper
transaction
librarian
user
```

- Object oriented programming has two important concepts
    - Class: Here we are building a cookie cutter/ design (Blueprint)
        - In programming world we write class to specify structure
    - Object: This is what we operate on (cookie/home/ac).
        - We create object from class and object has memory/cpu/resources attached to it.

#### Writing a class
- Class is a blueprint
    - members are contents (variables)
    - methods are capabilities (functions)
- Classes or objects can have relationships
- To classify these relationship all we have to figure out is
    - is-a relationship
    - has-a relationship
- Technically in OOD we have 4 types of relationships that can exist
    - Association: uses
    - Aggregation: Weak has-a
    - Composition: Strong has-a
    - Inheritence: is-a

#### Exercise
- Identify classes for Restaurant, we are supposed to build a Billing system
    - Restaurant
    - Menu
    - MenuItem
    - Tables list<Table>
    - Order
    - OrderItem
    - Bill
    - Payment

- Menu
```
contents:
        menu items
```

- Menu Item
```
contents:
  id
  category
  price
  name
```

- Table
```
content:
   number
   capacity
```

- Order
```
content:
  id
  list<orderItem>
  status
capability:
  generate_bill()
  cancel
```

- OrderItem
```
content:
  id
  menuitem_id
  quanity
```

- Bill
```
contents:
  id
  Order
  amount
  tax
  total
capabilites:
  pay()
```

### UML Diagrams
- [Refer Here](https://online.visual-paradigm.com/) for visual paradigm

### Principles
- Abstraction
- Encapsulation
- Polymorphism
- SOLID
- DuckTyping (Python special)
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/oop_intro.ipynb) for the notebook created in the class


# April 30

## Object oriented Programming
- Lets try to build an application which does calcuations i.e. we will be builing a calculator.
    - Investment Calculator
    - Loan Calculator
    - Tax Caclulator

### Basics and Syntax
- Refer Here for programiz class
- How to define a class
```
class <class-name>:
    ....
    ....
    ....
Class names should be Pascal Casing
class Car:
    pass
Class can have members.
class Car:
    type = "hatchback"
    model = "Civic"
    manufacturer = "Honda"
note: we have member types, which we will be revisiting soon
Class can have methods
class Car:
    type = "hatchback"
    model = "Civic"
    manufacturer = "Honda"

    def start():
        pass

    def stop():
        pass
```

- Class has three types of methods
    - Static methods
    - class methods
    - object/instance methods
- Lets use object methods and object members for some time and revisit class methods
- Let revisit syntaxes with object/instance methods and members
- lets look into a method called __init__
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/oops.ipynb) for class methods, class members, instance methods, instance members and static methods
- Terms introduced
    - decorator @classmethod

## Inheritence in Python
- For inheritence and access modifier [refer](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/inheritence.ipynb) jupyter notebook

#### Summary of Public, Private, and Protected in Python
- Public, private, and protected are access modifiers in Python used to control the visibility and accessibility of class members (attributes and methods). Python uses naming conventions, not strict enforcement, to indicate these levels of access[5][3][1].

#### Public Members
- Definition: Accessible from anywhere-inside or outside the class.
- Syntax: No underscore prefix.
- Example: self.name
- Behavior: Default for all class variables and methods.
- Usage: Can be freely accessed and modified from any part of the code[1][2][3][5].

#### Protected Members
- Definition: Intended to be accessible within the class and its subclasses.
- Syntax: Prefix with a single underscore (_), e.g., self._age
- Behavior: This is a convention-Python does not prevent outside access, but it signals that the member is meant for internal or subclass use.
- Usage: Used when you want to allow subclass access but discourage external use[1][3][4][5][6].

#### Private Members
- Definition: Intended to be accessible only within the defining class.
- Syntax: Prefix with double underscores (__), e.g., self.__salary
- Behavior: Python applies name mangling-the interpreter changes the name of the variable to include the class name, making accidental access from outside the class more difficult.
- Usage: Accessing from outside the class raises an AttributeError, but it can still be accessed using the mangled name (e.g., _ClassName__salary), though this is discouraged[1][3][5][6].

#### At a Glance
| Modifier  | Prefix | Accessible From        | Enforced by Python?     | Example         |
|-----------|--------|------------------------|--------------------------|-----------------|
| Public    | (none) | Anywhere               | No                       | `self.name`     |
| Protected | `_`    | Class & subclasses     | No (convention only)     | `self._age`     |
| Private   | `__`   | Class only (name mangling) | Partial (name mangling) | `self.__salary` |


#### Key Points:
- Python’s access modifiers are conventions, not strict rules.
- Public: No underscores, accessible everywhere.
- Protected: Single underscore, intended for class and subclasses.
- Private: Double underscore, name mangling to discourage outside access[3][5][1].

- These conventions help with code organization, encapsulation, and maintainability.

Citations:

[1] https://www.tutorialspoint.com/access-modifiers-in-python-public-private-and-protected

[2] https://www.tutorialspoint.com/python/python_access_modifiers.htm

[3] https://dev.to/ankitmalikg/python-how-to-define-public-private-and-protected-variables-in-a-class-4g9

[4] https://www.tutorialsteacher.com/python/public-private-protected-modifiers

[5] https://www.scaler.com/topics/access-modifiers-in-python/

[6] https://llego.dev/posts/access-modifiers-python/

[7] https://prepinsta.com/python/access-modifiers/

[8] https://diveintopython.org/learn/classes/methods

[9] https://geekpython.in/access-modifiers-in-python

[10] https://technogeekscs.com/access-modifiers-in-python/

[11] https://www.datacamp.com/tutorial/python-private-methods-explained

[12] https://www.reddit.com/r/programming/comments/10h1n9x/public_private_and_protected_access_modifiers_in/

[13] https://www.designgurus.io/answers/detail/what-is-the-difference-between-public-private-and-protected

[14] https://www.studytonight.com/python/access-modifier-python

[15] https://pythonlobby.com/access-specifiers-or-access-modifiers-in-python-programming-public-private-and-protected-keywords/

##### Answer from Perplexity: pplx.ai/share

# May 2

## Object oriented programming
- SOLID Priniciples
- To continue building our calculator, we need to
    - unit test
    - exception handling
    - abstraction
    - standard library
    - pythonic coding

### Python abstract classes
- [Refer Here](https://docs.python.org/3/library/abc.html) for abstract classes
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/oop_cond_1.ipynb) for jupyter notebook

### Create virtual environment in python
- [Refer Here](https://docs.python.org/3/library/venv.html) for virtual environment
- Lets Create virtual environment and follow standard structure
- create a new folder
- now cd into this folder
- Create a virtual environment
```python -m venv .venv```
- Now activate virtual environment
    - Window .venv\Scripts\activate
    - mac/linux source .venv/bin/activate
    ![image](https://github.com/user-attachments/assets/04df3e7f-104d-4ebb-b142-27b08c74197b)

- To download additional packages
```pip install <package>```

- To list all the installed packages
```
pip freeze
pip freeze > requirements.txt
```

- To install dependencies from requirements.txt
```pip install -r requirements.txt```

#### Exercise:
- create a new folder
- activate the virtual environment
- install the package called pytest

# May 3

## Python Exceptions
- [Refer Here](https://www.programiz.com/python-programming/exceptions) for python exceptions

![image](https://github.com/user-attachments/assets/61c4acf6-bdf7-4e41-b171-16f081d2f0a6)

- Errors: represent conditions such as which cannot be handled
    - compilatioon
    - syntax
    - logical part of the code
- Exceptions: can be caught and handled by the program
- Exception Handling: For this we have try..except Block
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/exceptionsnother.ipynb) for the jupyter notebook with exception handling

### Calculator CLI
- Lets try to build an application which does calcuations i.e. we will be builing a calculator.
    - Investment Calculator
    - Loan Calculator
    - Tax Caclulator
- Create the virtual environment and activate the virtual environment from terminal
- Open the folder in visual studio code and Select the Python interpreter Ctrl+shift+p

![image](https://github.com/user-attachments/assets/d153e311-08e6-4c34-9aef-27db0d5b56c1)

- [Refer Here](https://github.com/asquarezone/Python/commit/8682b8f057f7df3420cff3ed8a2de300927db341) for the first set of changes done in the application with abstract classes
- [Refer Here](https://github.com/asquarezone/Python/tree/main/Apr25/foundations/projects/calculator-cli) for the code which we have written and [Refer Here](https://github.com/asquarezone/Python/commit/69f7b04998bdc11c2a237c2b17b848326d179ad5) for changeset

## Python Standard Library
- This is vast collection of modules & packages that are automatically installed when you install python.
- This is python’s builtin toolkit
- [Refer Here](https://docs.python.org/3/library/index.html) for official docs of python standard library

## OS & FileSystems
- When we have tasks such as
    - Path Manipulation
        - constructing files and directory paths
        - Checking existence
    - File I/O
        - Creating, moving, copying and deleting files
        - Reading & writing files
    - Temporary Workshops
    - Archiving & cleanup
- Lets look at following modules
    - [os](https://docs.python.org/3/library/os.html)
    - shutil
    - [pathlib](https://docs.python.org/3/library/pathlib.html)
    - tempfile
- We use subprocess module to launch linux or windows processes

#### Working with dates and times
- [datetime module](https://docs.python.org/3/library/datetime.html)
- [Refer Here](https://www.programiz.com/python-programming/datetime)
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/standardlibrary/os_n_files.ipynb) for samples done in the class.

### Pythonic

### list comprehensions

- Provide a concise way to create lists base on existing list by applying expressions and filtering conditions
- list comprehension syntax
```[ expression for item in iterable if condition ]```

### set comprehensions
- similar to list comprehensions but produces a set instead of list
```{ expression for item in iterable if condition }```

### dictionary comprehensions
- similar to list and set, but you define both key and value for each element
```{ key_expression: value_expression for item in iterable if condition }```
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/standardlibrary/pythonic.ipynb) for expressions

#### Exercise:
- Try to find all the files in your downloads folder which are greater than 1 MB (python)
```
path = Path(r"C:\Users\Dell\Downloads")
[ item for item in Path(r"C:\Users\Dell\Downloads").rglob("*") if  item.is_file() and item.stat().st_size > 1048576 ]
```

### Type Hinting
- Type hinting uses the typing module to specify the expected types of function arguments and return values [Refer Here](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html) for cheatsheet and [Refer Here](https://realpython.com/lessons/type-hinting/) for article
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/standardlibrary/type_hinting.ipynb) for the jupyter notebook

### Code coverage
- [Refer Here](https://www.browserstack.com/guide/generate-pytest-code-coverage-report) for how to do code coverage
- Code coverage gives us metrics on how much of development code is covered by test code
- [Refer Here](https://github.com/asquarezone/Python/commit/63fc874444ef188bb0f59ab0ea24e29016d45d09) for the changes

### Building cli applications in Python
- lets use [argparse](https://docs.python.org/3/library/argparse.html) module
- [Refer Here](https://github.com/asquarezone/Python/commit/01fee6550e898bd05b3904672d534597fefa01f9) for the cli application

# May 6

## Static Code Analysis
- Ensure the following extensions are installed
    - pylint | flake8 | mypy

    ![image](https://github.com/user-attachments/assets/cf4cb6eb-4088-44d0-b0b7-433ddb9dfe42)

    - autopep8 | black formatter

    ![image](https://github.com/user-attachments/assets/479080f1-5931-4351-ab2d-c2a7e539a7c0)

- [Refer Here](https://github.com/asquarezone/Python/commit/ebaf45904bdd24af20ca50e24ed316e2ddb6ad46) for changes done to improve code quality

### Property (oops)
- [Refer Here](https://www.programiz.com/python-programming/property)
- Example

```
class Person:
    def __init__(self, name):
        self._name = name

    @property
    def name(self):
        return self._name

    @name.setter
    def name(self, value):
        if not isinstance(value, str):
            raise TypeError('Name must be a string')
        self._name = value

p = Person("test")
p.name = "hello"
```

### Persistence
- To add persistence to our applications we have two approaches
    - unstructured:
        - data cannot be queried can only be searched
        - examples:
            - text
            - pdf
            - files
        - decision: file format
    - structured:
        - data can be queried
        - Examples:
            - databases
        - decision: database type

### Findout What is the file format & when to use
- CSV File Format

```
number, name, course
1, abc, python
2, abd, DevOps
3, abe, GenAI
```

- JSON:

```
{
    "course": "Python",
    "students": [
        "abc", "bca"
    ],
    "address": {
       "flatno": 601,
       "building": "nigiri"
    }
}
```

- YAML
```
---
course: Python
students:
  - abc
  - bca
address:
  flatno: 601
  building: nilgiri
```

### Reading and Writing files in Python
- [Refer Here](https://www.programiz.com/python-programming/file-operation) for python file handling
- Lets write a dictionary into json
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/persistence.ipynb) for the examples done in the class


# May 7

## Databases
- On a larger note we have two types of databases in terms of how they handle schema (structure)
    - Strict on Structure (Relational databases)
    - Minimal restrictions (NOSQL)
- Relational database:
    - Data is tabular in nature.
    - Each column has a field and each row is a record
    - In a database i can have multiple tables
    - Tables can have relations between them
- Relational database have a formal language which is based on standard (Strucutred Query Language)
- Each DBMS adopts the standard and create their own query language
    - orcale => pl/sql
    - SQL Server => t-sql
    - mysql
    - postgres
- SQL
    - Create:
        - create a books table
```
“`sql
</ul>
<h1>mysql</h1>
CREATE TABLE books (
id INT AUTO_INCREMENT PRIMARY KEY,
title VARCHAR(255) NOT NULL,
author VARCHAR(100) NOT NULL,
description TEXT
);
<h1>microsoft sql server</h1>
CREATE TABLE books (
id INT IDENTITY(1,1) PRIMARY KEY,
title VARCHAR(255) NOT NULL,
author VARCHAR(100) NOT NULL,
description TEXT
);
<h1>mysql</h1>
INSERT INTO books (title, author, description) VALUES
('The Great Gatsby', 'F. Scott Fitzgerald', 'A novel set in the Roaring Twenties.'),
('To Kill a Mockingbird', 'Harper Lee', 'A novel about racial injustice in the Deep South.');
<h1>microsoft sql server</h1>
INSERT INTO books (title, author, description) VALUES
('The Great Gatsby', 'F. Scott Fitzgerald', 'A novel set in the Roaring Twenties.'),
('To Kill a Mockingbird', 'Harper Lee', 'A novel about racial injustice in the Deep South.');
<code>* Retrieve</code>sql
SELECT * FROM books;
SELECT title, author FROM books;
SELECT * FROM books WHERE author = 'Harper Lee';
SELECT * FROM books ORDER BY title ASC;
</li>
</ul>
<code>* Update</code>sql
UPDATE books
SET description = 'A classic American novel set in the 1920s.'
WHERE title = 'The Great Gatsby';
<code>* Delete</code>sql
DELETE FROM books WHERE id = 1;
“`
```

- Relational Database for Library

![image](https://github.com/user-attachments/assets/de7c5810-1c21-426e-a7ef-745e8d549780)

### ORM (object relational mapping) libraries
- ORM frameworks map table to a class
- we can write the code where we deal with objects (records)
- The advantage of using orm framework is your code works with any relational database.
- Examples
    - Java: Hibernate
    - .net: EntityFramework
    - python: SQL Alchemy

### Application Types
- Commandline
- Desktop/Mobile Apps
- Web:
    - Web Apps
    - Web APIs

#### WebSite (WebApps)
- Generation 1: Readonly
    - Technologies:
        - html, css, javascript
        - server: apache, iis
- Generation 2: Interactivity
    - Technologies:
        - PHP, ASP, Servlets
        - Databases:
- Generation 3: Improvements
    - Technologies
        - Asp.net, JSP, Python Django …, bootstrap (css)
        - Databases
- Generation 4: Mobile Apps , Desktop Apps with Web
![image](https://github.com/user-attachments/assets/c29892bc-1b78-430e-988b-c48f2b6a913c)

# April 8

## HTTP(s)

- HTTP has request and response
- Request has
    - url/endpoint
    - [headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers): these are key value pairs sent along with request
    - body:
    - [Action/Verb/Method](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods):
        - GET: Select
        - PUT: Update (all)
        - PATCH: update (few)
        - POST: Create
        - DELETE: Delete
- Response
    - Status Code: [Refer Here](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status)
        - 1xx: Information
        - 2xx: Success
        - 3xx: Redirection
        - 4xx: client side errors
        - 5xx: Server side errors
    - [headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers)
    - body

#### Exercise:
- Write a python code to send sms
- Write python code to find temperature of hyderabad tomorrow [Refer Here](https://github.com/asquarezone/Python/tree/main/Apr25/foundations/clients)

### Sending HTTP Requests
- Python has a pypi library requests and [Refer Here](https://realpython.com/python-requests/) for using requests library

```
import requests
url = "https://fakestoreapi.com/products/1"
response = requests.get(url)
if response.status_code == 200:
    print(response.content)
```
- Generally all APIs are documented which give us how to use apis. The standard is OpenAPI

#### REST API
- This is an architecural pattern to build APIs
- [Refer Here](https://www.ibm.com/think/topics/rest-apis#:~:text=A%20REST%20API%20is%20an,to%20connect%20distributed%20hypermedia%20systems.) for RESTAPI docs

#### REST API Principles

| Principle                | Description |
|--------------------------|-------------|
| **Uniform Interface**     | Standardizes interactions between client and server using consistent resource identification, representations, and HTTP methods (GET, POST, PUT, DELETE)[1][4][7]. |
| **Client-Server Separation** | Separates client and server concerns, allowing each to evolve independently as long as the interface is unchanged[1][3][4][7]. |
| **Statelessness**         | Each request from client to server must contain all necessary information; no session state is stored on the server[1][3][4][7]. |
| **Cacheable**             | Responses must define whether they are cacheable to improve performance and scalability[1][3][4][7]. |
| **Layered System**        | The API architecture can include multiple layers (e.g., intermediaries, proxies) without clients knowing about them[1][3][4][7]. |
| **Code on Demand (optional)** | Servers can provide executable code (like JavaScript) to clients, extending client functionality when needed[1][4][7]. |

- Would you like examples of how these principles are applied in real-world APIs?

- Citations:

[1] https://restfulapi.net

[2] https://daily.dev/blog/restful-api-design-best-practices-guide-2024

[3] https://www.ibm.com/think/topics/rest-apis

[4] https://blog.dreamfactory.com/rest-apis-an-overview-of-basic-principles

[5] https://aws.amazon.com/what-is/restful-api/

[6] https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design

[7] https://about.gitlab.com/blog/2024/10/18/guide-to-rest-api/


[8] https://www.postman.com/api-platform/api-design/

[9] https://www.getambassador.io/blog/7-rest-api-design-best-practices

[10] https://upsun.com/blog/restful-api-design-principles/

[11] https://www.mulesoft.com/api/rest/what-is-rest-api-design

[12] https://codewithmukesh.com/blog/restful-api-best-practices-for-dotnet-developers/

[13] https://blog.postman.com/rest-api-examples/

[14] https://www.freecodecamp.org/news/rest-api-best-practices-rest-endpoint-design-examples/

[15] https://swagger.io/resources/articles/best-practices-in-api-design/

[16] https://www.youtube.com/watch?v=8XK2o5MfxkE

[17] https://stackoverflow.blog/2020/03/02/best-practices-for-rest-api-design/

### Lets Design a REST API for Job Portal
- Identify Nouns which generally become Resources
    - User
    - Employer
    - Job
    - Account
- On Each Resource (Noun) define Actions
    - Actions Account:
        - Register
        - UnRegister
    - User
    - Job
    - Employer
- URI (Uniform Resource Identifier)
    - /Users
        - Get: Get all users
        - POST: Create a user with a body (json)
    - /Users/1
        - Get user with id 1
        - PUT: update the user information for a user with id 1

### REST API Creation – Server
- We find nouns and verbs and create a API with docs
- In python, we can acheive creating this with many libraries but we will be using fastapi.
- Other options:
    - Django-restful
    - flask

### Rest API Usage – Client
- On a larger note
    - Web stores (Reactjs/angularjs)
    - Mobile/Desktop  App
    - Custom Tools:
        - from code
        - from cli
- For using a Rest API we need API Docs (Swagger/OpenAPI)

### References
- APIs
    - [Refer Here](https://github.com/whizkydee/Awesome-APIs)
    - [Refer Here](https://github.com/public-apis/public-apis)

### Getting started with fastapi
- [Refer Here](https://fastapi.tiangolo.com/) for fastapi official docs
- Create a virtual environment and install fastapi

```pip install "fastapi[standard]"```

- code which i have written

```
from fastapi import FastAPI

app = FastAPI(
    title="Hello-api",
    summary="Learning FastAPI",
    version="0.0.1")

@app.get("/")
def home():
    return { "message": "hello" }

@app.get("/square/{number}")
def square(number: int):
    return {
        "result" : number ** 2
    }
```

# May 15

### FastAPI (contd)
- Fastapi allows asynchronous calls
### Async/await
- Asynchronous programming allows to run multiple tasks concurrently without blocking the program. This is useful when dealing with IO-bound operations like
    - Waiting for network requests
    - reading/writing files
    - Interacting with databases
- [Refer Here](https://github.com/asquarezone/Python/blob/main/Apr25/foundations/async.ipynb) for basic async await example

### FastAPI Basics
- Defining first API endpoint
- Create a new folder called as books
- Activate a new virtual environment and install [fastapi](https://fastapi.tiangolo.com/#installation)
- Create requirements.txt pip freeze > requirements.txt
- Create a new file called as main.py containing the following code

```
from fastapi import FastAPI

# create app 
app = FastAPI()

# define endpoint

@app.get("/books")
async def get_all_books():
    return [{
        "book_id": 1,
        "title": "Your Brain at Work",
        "author": "David Rock"
    }]
```

- refer to classroom video for vscode debugger setup.
- [Refer Here](https://github.com/asquarezone/Python/commit/90e2c6246bfdefc5ea25176c085d461a20813a62) for the changes done

### Defining and using request and response models
- FastAPI simplifies the process of defining and validating the request and responses using [Pydantic](https://docs.pydantic.dev/latest/)
- Lets create a file called as models.py
- [Refer Here](https://github.com/asquarezone/Python/commit/07a332defef6ee103583b038ae26f9f396c557ad) for the changes done


# May 16

## Fast API contd..
### Working with Relational databases using SQLAlchemy

- Activate the virtual environment and install sqlalchemy

```pip install sqlalchemy```

- [Refer Here](https://github.com/asquarezone/Python/commit/7243695f839d2ccd58dd83460d1c015d4d81c10b) for the changes done to persist the books into sqlite database.

#### Lets build a library using fastapi
- [Refer Here](https://github.com/asquarezone/Python/commit/02dcd0d596eaee7a5d08ea5f9cf36290c5f42002) for the changes.
- Note: Transaction is failing and will be fixed in next session.

# May 17

## Microservices
- Consider an ecommerce application which is designed as shown below

![image](https://github.com/user-attachments/assets/ef786b5a-ee17-484d-a3d3-d649de04608b)

- Components
    - Web-Store:
        - This is front end application that caters to browser requests
        - This application requests to the backend Ecommerce APIs for business logic
    - Technologies:
        - ReactJs
        - Angular JS
        - VueJs

    - E-Commerce APIs:
        - This is backend application which responds to API calls that serve business logic
        - This application can be communicated from Web-Store and Mobile APPS
    - Technologies:
    - Python:
        - FastAPI
        - Flask
        - Django Restful
    - Java:
        - Spring boot
    - Dotnet:
        - Asp.net core web apis
- Mobile App:
    - This is thick client which can be installed on smartphones
    - Technologies
        - Andriod:
            - Kotlin
        - IOS:
            - Swift
- Database:
    - This can be any Relational database
- Options:
    - Postgres
    - mySQL
    - Oracle
    - SQL Server
- Deployment Options
    - Physical/Virtual Machines:
         -  Each component can be run on a different server (physical/virtual)
         ![image](https://github.com/user-attachments/assets/8a9f2d5e-6e39-4329-ab47-a6dfb80a6279)
         - We need to scaling setup for High Availability
        ![image](https://github.com/user-attachments/assets/5426fff7-9978-4cf7-976d-ff1335773d87)

    - Cloud Based PaaS Models: Cloud offers PaaS (Platform as a Service)
    ![image](https://github.com/user-attachments/assets/83a8dab0-342b-4c12-9418-174fa78f9b64)

### Microservices: Definition and Key Concepts
- Microservices is an architectural approach to software development where an application is structured as a collection of small, independent services, each responsible for a specific business function or capability[1][2][4][6].
-  Unlike traditional monolithic architectures, where all features and logic are tightly integrated into a single codebase, microservices break down the application into modular components that can be developed, deployed, and scaled independently[1][2][5][6].

### Core Characteristics
- Independence: Each microservice runs its own process and typically manages its own data, allowing for independent development, deployment, and scaling[2][4][5][6].
- Specialization: Each service is designed around a specific business capability or function, such as user authentication, payment processing, or inventory management[1][2][4][7].
- Loose Coupling: Services interact with each other through well-defined interfaces, usually via lightweight APIs (such as REST or messaging protocols), minimizing dependencies between them[2][5][6][7].
- Autonomous Teams: Microservices are often owned and managed by small, cross-functional teams, enabling faster development cycles and innovation[2][1].
- Technology Agnostic: Teams can use different programming languages, databases, or frameworks for each service, choosing the best tool for each job[2][6].

### How Microservices Work
- Each microservice is self-contained, handling a distinct task or business requirement[5][6].
- Services communicate over a network using lightweight protocols (HTTP, REST, messaging), often coordinated via an API gateway that manages requests, security, and load balancing[5].
- Microservices are commonly deployed using containers, which encapsulate the service and its dependencies, making it easier to manage and scale in cloud environments[4][5].
- The architecture supports automation and orchestration for deployment and scaling, often leveraging DevOps practices and continuous delivery pipelines[2][6].

### Advantages
- Scalability: Individual services can be scaled independently based on demand, optimizing resource usage and cost[2][4][6].
- Resilience: Failure in one service does not necessarily impact others, enhancing overall system reliability[5][6].
- Agility: Teams can update, deploy, or roll back services without affecting the entire application, accelerating time-to-market for new features[2][7].
- Flexibility: The modular nature allows for easier experimentation, adoption of new technologies, and reuse of services across different applications[2][6].

### Challenges
- Complexity: Managing a distributed system of many services introduces challenges in monitoring, debugging, and maintaining inter-service communication[6].
- Operational Overhead: Requires robust automation, orchestration, and monitoring tools to manage deployment, scaling, and fault tolerance[5][6].

### Typical Use Cases
- Microservices are widely adopted in cloud-native applications and by organizations seeking to build scalable, resilient, and rapidly evolving systems.
- Leading technology companies like Amazon, Netflix, and Uber have transitioned from monolithic architectures to microservices to support their growth and innovation needs[1][2][4].

- In summary, microservices architecture enables building modern, scalable, and flexible applications by decomposing them into loosely coupled, independently deployable services, each focused on a specific business function[1][2][4][6].

Citations:

[1] https://www.spiceworks.com/tech/devops/articles/what-are-microservices/

[2] https://aws.amazon.com/microservices/

[3] https://microservices.io

[4] https://cloud.google.com/learn/what-is-microservices-architecture

[5] https://www.techtarget.com/searchapparchitecture/definition/microservices

[6] https://en.wikipedia.org/wiki/Microservices

[7] https://www.paloaltonetworks.com/cyberpedia/what-are-microservices

[8] https://www.atlassian.com/microservices

[9] https://www.vmware.com/topics/microservices

- Microservices

![image](https://github.com/user-attachments/assets/c347ba6d-6cb0-4db8-89d8-c660a13c70a5)

![image](https://github.com/user-attachments/assets/ab13ae6a-ad0d-43b5-acc9-52ebb97140df)

![image](https://github.com/user-attachments/assets/a3b0daa0-a7bb-459f-9f57-d406b013adf7)

### Docker Container:
- [Installation](https://docs.docker.com/desktop/setup/install/windows-install/)
- Lets look into the following [application](https://github.com/fastapi/full-stack-fastapi-template)
- [Refer Here](https://github.com/asquarezone/Python/tree/main/Apr25/fastapi/hello-api) for example to create docker container based on our apis


## Lets Build a Microservice Application

Options:

- Ecommerce
- Food delivery
- Movie Booking
- Note: We will be trying to simulate Movie Booking Application with APIs

### Movie Booking Application
- Search and find out what are components in movie booking
    - identity Service
    - User Profile Service
    - Movie Service
    - ShowTime Service
    - Theatre Service
    - Booking Service
    - Payment Service
    - Notification Service
    - OffersService

- Let trim the development to three services
    - Movie Service
    - ShowTime Service
    - Theatre Service

### Movie Service
- Endpoints
    - Get /movies – List all movies
    - Get /movies/{id} – Get a Movie by id
    - POST /movies -> Create a new movie
    - PUT /movies/{id} -> Update movie
    - DELETE /movies/{id} -> Delete
- [Refer Here](https://github.com/asquarezone/Python/tree/main/Apr25/fastapi/microservices/backend/movies-svc) for movies service.

### Theatre Service
- Endpoints
    - Get /theatres – List all theatre
    - Get /theatres/{id} – Get a theatre by id
    - POST /theatres -> Create a new theatre
    - PUT /theatres/{id} -> Update theatre
    - DELETE /theatres/{id} -> Delete theatre
- Theatre
    - id
    - name
    - location
- [Refer Here](https://github.com/asquarezone/Python/tree/main/Apr25/fastapi/microservices/backend) for Theatre and movie service

# May 18

## Theatre Service
- Theatre
    - id
    - name
    - location
- [Refer Here](https://github.com/asquarezone/Python/tree/main/Apr25/fastapi/microservices/backend) for Theatre and movie service
- Lets add screens
    - Screen
        - id: int
        - theatre_id: int
        - name:
        - capacity: int
- Endpoints
    - Get /theatres – List all theatre
    - Get /theatres/{id} – Get a theatre by id
    - POST /theatres -> Create a new theatre
    - PUT /theatres/{id} -> Update theatre
    - DELETE /theatres/{id} -> Delete theatre
    - GET /theatres/{id}/screens -> Get screens for a theatre
    - POST /theatres/{id}/screens -> Creates screens for a theatre
- [Refer Here](https://github.com/asquarezone/Python/commit/a553ff2b1e6251e2922cac53ce3f5243ec4d6c31) for the changes done to include screen

### Show time Service – Exercise
- Structure
    - id: int
    - movie_id: int
    - screen_id: int
    - start_time: datetime
    - end_time: datetime
- Endpoints:
    - GET /showtimes
    - GET /showtimes/{id}
    - POST /showtimes/
    - GET /showtimes/screen/{screen_id}: call rest api of screen service to get screen id and filter showtimes by screen id
    - GET/showtimes/movie/{movie_id}: call rest api of movie service to get movie id and filter showtimes by movie id
