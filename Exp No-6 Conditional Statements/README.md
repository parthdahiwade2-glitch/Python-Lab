Experiment – 6

Title

Decision Making Using if-else Statement in Python

Aim

To understand and implement decision-making techniques in Python programs using conditional statements such as if, if-else, if-elif-else, and nested if.

Objectives

• To understand how conditional execution works in Python

• To learn the syntax and structure of if-else statements

• To practice writing programs based on decision logic

• To apply conditional statements to solve real-life problems

Theory

Programming is not only about performing calculations — it is also about making decisions based on different situations. In real life, we constantly evaluate conditions before taking actions, such as deciding whether to carry an umbrella based on the weather or checking eligibility before applying for something. Similarly, in Python, decision making is implemented using conditional statements that allow the program to choose different execution paths depending on whether a condition is true or false.

The if-else statement is one of the most fundamental decision-making tools in Python. It allows a program to evaluate a condition and execute a specific block of code when the condition is satisfied (True) and another block when it is not (False). This structure helps create dynamic and intelligent programs rather than programs that simply execute instructions sequentially.

Python differs from many other programming languages because it uses indentation to define blocks of code instead of curly braces. Proper indentation improves readability and ensures the interpreter correctly understands the structure of the program. Incorrect indentation can lead to execution errors or unintended program behavior.

Conditional statements are essential for building logical applications such as grading systems, login verification, eligibility checking, menu selection systems, and many more real-world scenarios. Python provides multiple variations of conditional control structures including simple if statements, if-else statements, multi-branch if-elif-else statements, and nested conditions that allow checking multiple levels of criteria.

By using these decision-making constructs, programmers can design flexible and responsive programs capable of adapting to user input and environmental conditions.

Boolean Conditions

The expression used in an if statement must evaluate to a Boolean value (True or False). Conditions are usually formed using:

• Relational operators (<, >, <=, >=, ==, !=)

• Logical operators (and, or, not)

Example conditions:

• marks >= 40

• age >= 18 and citizen == True

These expressions determine which block of code will be executed.

Importance of Indentation in Python

Unlike many programming languages that rely on braces { } to define blocks of code, Python uses indentation. All statements belonging to an if or else block must be aligned at the same indentation level.

Improper indentation may cause:

• Logical mistakes in program flow

• IndentationError during execution

Therefore, indentation is not only a stylistic requirement but a fundamental part of Python syntax and readability.

Control Flow in if-else

The if-else structure directs how a program executes instructions:

• Only one block (either if or else) runs based on the condition

• After execution of the selected block, the program continues normally

• This ensures efficient and structured decision-based execution

Types of Conditions Used

• Simple condition: A single comparison

• Compound condition: Combination of multiple conditions using logical operators

These enable handling of complex real-life scenarios such as authentication systems, eligibility verification, and grading evaluation.

Flow of Execution

Start
↓
Check Condition
↓
True → Execute if-block
False → Execute else-block
↓
End

Programs

Program 1: Check Whether a Number is Even or Odd

Program 3: Voting Eligibility

Program 4: Login Authentication

Decision Making Using if-elif-else Statement in Python
Syntax
if condition1:
    statement(s)
elif condition2:
    statement(s)
elif condition3:
    statement(s)
else:
    statement(s)

Program 1: Grade Calculation
marks = int(input("Enter marks: "))



Program 2: Menu-Driven Choice

Using Nested if Statement in Python

Syntax

if condition1:

    if condition2:
    
        statement(s)
    
    else:
       
        statement(s)

else:
    
    statement(s)

Program 1: Voting Eligibility with Citizenship

Problem statements

1. Find out wether a given year is leap or not.

2. Write a python program to check if a date is valid and print the incremented date if it is valid.

3. Write a python program to calculate the gross salary of an employee based on basic salary.

If basic <= 10000: HRA = 20%, DA = 80%

If basic <= 20000: HRA = 25 %, DA = 90%

Otherwise : HRA = 30%, DA = 95%

4. Write a python program to calculate Income tax based on annual income:

Up ti Rs.2,50,000: No tax


Rs.2,50,001-Rs.5,00,000 : 5%
Rs.5,00,001 - Rs.10,00,000: 20%

Above Rs.10,00,000 :30%

Conclusion

Through this experiment, various decision-making constructs in Python — including if, if-else, if-elif-else, and nested if statements — were studied and implemented. These structures play a crucial role in developing logical and interactive programs by allowing them to evaluate conditions and respond accordingly. Understanding these concepts forms a strong foundation for solving real-world problems and building more advanced applications in Python.
