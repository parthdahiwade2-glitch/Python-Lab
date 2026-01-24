Experiment-2

Title

Python Environment, Data Types, Operators, and Basic Input/Output

Aim To study the Python programming environment and interface, understand execution modes, variables, data types, operators, and basic input/output operations in Python.

Objectives

• To understand the Python programming environment and interface

• To study Python execution modes

• To understand comments in Python

• To learn variables, identifier rules, and data types

• To study different operators and expressions

• To understand basic input and output mechanisms

Theory

Python Environment and Interface The Python environment provides tools and interfaces to write, execute, and debug Python programs. Python programs can be executed using different interfaces such as:
• Python Shell

• Jupyter Notebook

• Integrated Development Environments (IDEs) like Spyder, PyCharm, and VS Code

• Cloud-based platforms like Google Colab The interface allows users to write code, execute instructions, and view results interactively.

Python Execution Modes
Python supports two main execution modes:

a) Interactive Mode

• Commands are executed one line at a time

• Immediate output is displayed

• Useful for testing small code snippets and learning

Examples: Python shell, Jupyter Notebook cells, Google Colab

b) Script Mode

• Programs are written in a file and executed as a whole

• Suitable for developing complete applications

• Files usually have .py extension

Comments in Python Comments are non-executable statements used to explain code and improve readability.
• Single-line comments: Begin with #

• Multi-line comments: Written using triple quotes (""" """)

Comments help in documentation and understanding program logic.

Variables and Identifiers
A variable is a named memory location used to store data values. Rules for Identifiers:

• Must start with a letter (A–Z, a–z) or underscore _

• Cannot start with a digit

• Case-sensitive

• Should not use Python keywords Python uses dynamic typing, meaning variables do not require explicit data type declaration.

Data Types in Python
Python provides several built-in data types to store different kinds of data.

Basic Data Types

• Integer (int): Whole numbers

• Floating-point (float): Decimal numbers

• String (str): Sequence of characters

• Boolean (bool): True or False

The data type of a variable can be identified using the type() function.

Operators and Expressions
Operators are symbols used to perform operations on variables and values.

Types of Operators

• Arithmetic Operators: Used for mathematical calculations

(+, -, *, /, %)

• Relational Operators: Used for comparison

(>, <, >=, <=, ==, !=)

• Logical Operators: Used to combine conditions

(and, or, not)

• Assignment Operators: Used to assign values

(=, +=, -=, *=, /=)

• Bitwise Operators: Perform operations at bit level

(&, |, ^, <<, >>)

An expression is a combination of operators and operands that produces a result.

Basic Input and Output Operations
Input and output operations allow interaction between the user and the program.

• Input:

input() function is used to accept input from the user.

Input is treated as a string by default and may require type conversion.

• Output:

print() function is used to display output.

Formatted output can be achieved using commas or formatted strings.

Conclusion Thus, the Python programming environment, execution modes, variables, data types, operators, and basic input/output operations were studied and understood.

Programs

Comments
This is a single-line comment
Program to demonstrate Python interface and comments
""" This is a multi-line comment (docstring). Python supports interactive and script modes. """ print("Welcome to Python Programming") print("This program demonstrates comments and execution modes")

Variable declaration
student_name = "Snehal" age = 45 height = 5.3 is_faculty = True

Display data types
print("Name:", student_name, "Type:", type(student_name)) print("Age:", age, "Type:", type(age)) print("Height:", height, "Type:", type(height)) print("Faculty Status:", is_faculty, "Type:", type(is_faculty))

Arithmetic, relational, logical, assignment, and bitwise operators a = 10 b = 5
Arithmetic Operators
print("Addition:", a + b) print("Subtraction:", a - b) print("Multiplication:", a * b) print("Division:", a / b)

Relational Operators
print("a > b:", a > b) print("a == b:", a == b)

Logical Operators
print("AND:", a > 5 and b > 2) print("OR:", a > 20 or b > 2) print("NOT:", not(a > b))

Assignment Operators
c = a c += b print("Assignment Result:", c)

Bitwise Operators
print("Bitwise AND:", a & b) print("Bitwise OR:", a | b)

Input and display formatted output using input() and print()
Input from user
name = input("Enter your name: ") marks = int(input("Enter your marks: "))

Output using formatted print
print("Student Name:", name) print("Marks Obtained:", marks)

Experiment 2: Results and Conclusion Results

Python Environment & Execution Modes

Successfully executed code in both interactive and script modes Verified functionality across Python Shell, Jupyter Notebook, and Google Colab

Comments
Single-line (#) and multi-line (""" """) comments implemented successfully Enhanced code readability and documentation

Variables and Data Types VariableValueData Typestudent_name"Snehal"strage45intheight5.3floatis_facultyTruebool

Dynamic typing demonstrated - no explicit type declaration required type() function correctly identified all data types

Operators (a=10, b=5) Arithmetic: Addition=15, Subtraction=5, Multiplication=50, Division=2.0 Relational: a>b=True, a==b=False Logical: AND=True, OR=True, NOT=False Assignment: c+=b worked correctly Bitwise: AND=0, OR=15

Input/Output

input() successfully captured user data Type conversion with int() worked correctly print() displayed formatted output effectively
