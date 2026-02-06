Experiment–4

Title
Tuples in Python: Creation, Access, and Operations

Aim
To learn about Python tuples and how to create, access, and perform operations on them.

Objectives

Understand what tuples are in Python
Learn characteristics and benefits of tuples
Use indexing and slicing on tuples
Apply built-in tuple functions
Understand that tuples can't be changed

Theory

1. Introduction to Tuples
A tuple is like a list but you can't change it after creating it. Tuples use parentheses ( ) with elements separated by commas.
Example:

(10, 20, 30)

2. Characteristics of Tuples

Ordered

Indexed

Immutable (can't be changed)

Allows duplicate values

Can store different data types

3. Why Use Tuples

Faster than lists

Data stays safe (can't be accidentally modified)

Good for fixed data like coordinates, days of the week, database records

4. Creating Tuples

You can create tuples:


With parentheses

Without parentheses (tuple packing)

Using the tuple() constructor

Special case:

Single element tuple needs a comma:

(10,)

5. Indexing in Tuples

Access elements using index numbers starting from 0.
Supports:

Positive indexing

Negative indexing

6. Slicing in Tuples

Extract part of a tuple.

Syntax:
tuple_name[start : end : step]

start → where to begin (included)

end → where to stop (excluded)

step → gap between elements (optional)

7. Immutability of Tuples
Once created:

Can't add elements

Can't remove elements

Can't update elements

Trying to modify gives an error.

8. Built-in Functions for Tuples
FunctionDescriptionlen()Number of elementsmax()Maximum valuemin()Minimum valuesum()Sum of elementscount()Count occurrencesindex()Find index of element

9. Difference Between List and Tuple
ListTupleMutableImmutableUses [ ]Uses ( )SlowerFasterDynamicFixed

Problem Statements

1. Student Exam Result

A student's exam result is stored in a tuple containing three fixed fields:
Subject name, marks obtained, and grade.
Write a Python program to:

Store the exam result using a tuple.
Unpack the tuple elements into separate variables.
Display the subject, marks, and grade.
Check whether the student has scored 75 or more marks and print "Distinction" if the condition is satisfied.

2. Employee Attendance Tracker

An organization records an employee's daily attendance for a week using a tuple, where:
"P" represents Present, "A" represents Absent
Write a Python program to:

Store the attendance record in a tuple.
Count and display the total number of present days.
Count and display the total number of absent days.
Check whether the employee was absent at least once during the recorded period and display an appropriate message.

Conclusion

All objectives achieved! Tuples are:

Immutable: Can't be changed after creation, keeping data safe

Fast: Perform better than lists for fixed data

Reliable: Perfect for data that shouldn't be modified

Versatile: Support indexing, slicing, and built-in functions

Python tuples were successfully studied and all operations including creation, indexing, slicing, unpacking, and built-in functions worked perfectly!
