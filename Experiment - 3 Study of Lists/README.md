Experiment–3

Title

Lists in Python: Indexing, Slicing, and List Methods

Aim

To understand Python lists and perform operations such as indexing, slicing, and using built-in list methods.
________________________________________
Objectives

•	To create and access lists

•	To perform indexing and slicing operations

•	To apply commonly used list methods

•	To understand mutable nature of lists

•	To perform list traversal and modification
________________________________________
Theory

1. Introduction to Lists

A list is a built-in data structure in Python used to store multiple values in a single variable. Lists are written using square brackets [ ] and elements are separated by commas.

Lists are one of the most widely used data structures in Python because they are flexible and dynamic.
________________________________________
2. Characteristics of Python Lists

•	Ordered: Elements maintain insertion order

•	Indexed: Each element has a unique index starting from 0

•	Mutable: Elements can be modified after creation

•	Heterogeneous: Can store different data types in one list

•	Allows Duplicates: Same value can appear multiple times

List Creation

Lists can be created in multiple ways:


•	Using square brackets

•	Using the list() constructor

Lists can also be nested, meaning a list can contain another list.
________________________________________
4. Indexing in Lists

Indexing allows access to individual elements of a list.
Types of Indexing

•	Positive Indexing: Starts from 0 (left to right)

•	Negative Indexing: Starts from -1 (right to left)

Element	A	B	C	D

Index	0	1	2	3

Negative Index	-4	-3	-2	-1
________________________________________
5. Slicing in Lists

Slicing is used to extract a portion (sublist) from a list.

General Syntax:

list_name[start : end : step]

Meaning of each part:

•	start → index to begin slicing (included)

•	end → index to stop slicing (excluded)

•	step → gap between elements (optional)


Types of slicing:

•	Beginning slice

•	Ending slice

•	Full slice

Slicing does not modify the original list.
________________________________________
6. Mutability of Lists

Lists are mutable, meaning their elements can be changed after creation.

Operations possible due to mutability:

•	Updating elements

•	Adding new elements

•	Removing elements

This feature makes lists suitable for dynamic data storage.
________________________________________
7. List Traversal

Traversal means accessing each element of the list one by one.

Traversal can be done using:

•	for loop

•	while loop

Traversal is commonly used for data processing and analysis.
________________________________________
8. List Methods

Python provides several built-in methods to manipulate lists.

Method	Description

append()	Adds element at the end

insert()	Inserts element at given index

remove()	Removes specified element

pop()	Removes element by index

sort()	Sorts list

reverse()	Reverses list

clear()	Removes all elements

count()	Counts occurrences

index()	Returns index of element
________________________________________
9. Built-in Functions for Lists

Python provides built-in functions to work with lists:

Function	Purpose

len()	Number of elements

max()	Maximum value

min()	Minimum value

sum()	Sum of elements

Problem statements

1. Student Marks Management System

A teacher wants to store marks of students in a list.

Tasks:

•	Create a list of student marks

•	Display highest and lowest marks

•	Calculate average marks

•	Sort the marks in ascending order

Concepts Used: List creation, max(), min(), sum(), len(), sort()
________________________________________
2. Grocery Shopping List

A user maintains a grocery list for monthly shopping.

Tasks:

•	Create a grocery list

•	Add new items to the list

•	Remove purchased items

•	Display the final shopping list

Concepts Used: append(), remove(), indexing

________________________________________
3. Attendance Register

A class teacher records daily attendance.

Tasks:

•	Store present student roll numbers in a list

•	Check whether a particular student is present

•	Count total students present

Concepts Used: in operator, count(), len()
________________________________________
4. Mobile Contact List

A person stores phone contacts in a list.

Tasks:

•	Create a list of contacts

•	Add a new contact

•	Delete an existing contact

•	Display contacts alphabetically

Concepts Used: append(), remove(), sort()
________________________________________
5. Temperature Analysis

Daily temperature readings of a city are stored in a list.

Tasks:

•	Display temperatures of first and last 5 days

•	Find highest and lowest temperature

•	Calculate average temperature

Concepts Used: Slicing, max(), min(), sum()

Results

1. List Creation & Properties

Successfully created lists using [] and list() constructor

Verified: ordered, indexed, mutable, heterogeneous, allows duplicates

2. Indexing

Positive indexing (0, 1, 2...) - left to right ✓

Negative indexing (-1, -2, -3...) - right to left ✓

3. Slicing


Syntax list[start:end:step] worked correctly

Beginning, ending, and full slices successful

Original list unchanged (non-destructive)

4. List Methods Performance

MethodResultMethodResultappend()✓sort()✓insert()✓reverse()✓remove()✓count()✓pop()✓index()✓

5. Built-in Functions

len(), max(), min(), sum() - all executed successfully

6. List Traversal

for loop and while loop both accessed elements sequentially

7. Practical Applications
All five real-world scenarios completed:


Student marks management

Grocery shopping list

Attendance register

Contact list management

Temperature analysis

Conclusion
All objectives achieved successfully. The experiment demonstrated:

Flexibility: Lists store multiple data types and support dynamic modifications

Dual Access: Positive and negative indexing provide versatile element access

Rich Functionality: Built-in methods simplify common operations (add, remove, sort, search)

Mutability: Elements can be modified, making lists ideal for changing datasets

Real-world Utility: Lists effectively solve practical problems in data management and analysis
