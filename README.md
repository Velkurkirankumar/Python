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
