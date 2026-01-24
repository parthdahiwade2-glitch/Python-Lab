Experiment–4

Title

Tuples in Python: Creation, Access, and Operations
________________________________________
Aim

To understand Python tuples and perform operations such as creation, indexing, slicing, and use of built-in functions.
________________________________________
Objectives

•	To understand the concept of tuples in Python

•	To study characteristics and advantages of tuples

•	To perform indexing and slicing on tuples

•	To apply built-in tuple functions

•	To understand immutability of tuples
________________________________________
Theory

1. Introduction to Tuples

A tuple is an ordered collection of elements in Python, similar to a list, but immutable in nature. Tuples are written using parentheses ( ) and elements are separated by commas.

Example:
(10, 20, 30)
________________________________________
2. Characteristics of Tuples

•	Ordered

•	Indexed

•	Immutable (cannot be changed after creation)

•	Allows duplicate values

•	Can store heterogeneous data types
________________________________________
3. Why Tuples are Used

•	Faster than lists

•	Data integrity (values cannot be modified)

•	Used for fixed data such as coordinates, days of week, database records
________________________________________
4. Creating Tuples

Tuples can be created:

•	With parentheses

•	Without parentheses (tuple packing)

•	Using the tuple() constructor

Special cases:

•	Single element tuple must have a trailing comma
(10,)
________________________________________
5. Indexing in Tuples

Tuple elements are accessed using index numbers, starting from 0.

Both:

•	Positive indexing

•	Negative indexing

are supported.
________________________________________
6. Slicing in Tuples

Slicing is used to extract a portion of a tuple.
General Syntax:

tuple_name[start : end : step]

Meaning of each part:

•	start → index to begin slicing (included)

•	end → index to stop slicing (excluded)

•	step → gap between elements (optional)

7. Immutability of Tuples

Once a tuple is created:

•	Elements cannot be added

•	Elements cannot be removed

•	Elements cannot be updated

Any attempt to modify results in an error.
________________________________________
8. Built-in Functions for Tuples

Function	Description

len()	Number of elements

max()	Maximum value

min()	Minimum value

sum()	Sum of elements

count()	Count occurrences

index()	Find index of element
________________________________________

9. Difference Between List and Tuple

List	Tuple

Mutable	Immutable

Uses [ ]	Uses ( )

Slower	Faster

Dynamic	Fixed

Conclusion
Thus, Python tuples were studied and operations such as creation, indexing, slicing, packing, unpacking, and built-in functions were successfully implemented.


Problem Statements:
1. A student’s exam result is stored in a tuple containing three fixed fields:
Subject name, marks obtained, and grade.

Write a Python program to:

•	Store the exam result using a tuple.

•	Unpack the tuple elements into separate variables.

•	Display the subject, marks, and grade.

•	Check whether the student has scored 75 or more marks and print “Distinction” if the condition is satisfied.

2. An organization records an employee’s daily attendance for a week using a tuple, where:
"P" represents Present, "A" represents Absent 

Write a Python program to:

•	Store the attendance record in a tuple.

•	Count and display the total number of present days.

•	Count and display the total number of absent days.

•	Check whether the employee was absent at least once

•	during the recorded period and display an appropriate message.

Results

1. Tuple Operations

Creation (parentheses, packing, constructor, single element) 
Positive/negative indexing 
Slicing tuple[start:end:step] 
Immutability verified (add/remove/update blocked) 

2. Built-in Functions
len(), max(), min(), sum(), count(), index() - all successful 
3. Problem Statements

Student Result: Unpacking and distinction check 
Attendance: Count present (5), absent (2) days 

4. List vs Tuple
Tuple: Immutable, ( ), faster | List: Mutable, [ ], slower 
