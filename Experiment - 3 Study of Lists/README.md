Experiment–3

Title

Lists in Python: Indexing, Slicing, and List Methods

Aim

To learn about Python lists and how to use indexing, slicing, and built-in list methods.
Objectives

Create and access lists
Use indexing and slicing operations
Apply common list methods
Understand that lists can be changed
Work with list traversal and modification

Theory

Introduction to Lists
A list stores multiple values in one variable. Lists use square brackets [ ] with elements separated by commas.
Lists are super popular in Python because they're flexible and easy to work with.
Characteristics of Python Lists


Ordered: Elements stay in the order you put them

Indexed: Each element has a position starting from 0

Mutable: You can change elements after creating the list

Heterogeneous: Can mix different data types in one list

Allows Duplicates: Same value can appear multiple times


List Creation

You can create lists in different ways:

Using square brackets
Using the list() constructor


Lists can even contain other lists (nested lists).

Indexing in Lists

Indexing lets you access individual elements.

Types of Indexing:


Positive Indexing: Starts from 0 (left to right)

Negative Indexing: Starts from -1 (right to left)

ElementABCDIndex0123Negative Index-4-3-2-1

Slicing in Lists
Slicing extracts a part of the list.

Syntax:

list_name[start : end : step]

start → where to begin (included)

end → where to stop (excluded)

step → gap between elements (optional)


Slicing doesn't change the original list.
Mutability of Lists
Lists are mutable – you can change them after creating them.

What you can do:

Update elements

Add new elements

Remove elements

This makes lists great for data that changes.

List Traversal

Traversal means going through each element one by one.

You can use:

for loop

while loop

Useful for processing data.

List Methods

Python has built-in methods to work with lists:
MethodWhat it doesappend()Adds element at the endinsert()Inserts element at specific positionremove()Removes specified elementpop()Removes element by indexsort()Sorts the listreverse()Reverses the listclear()Removes all elementscount()Counts how many times element appearsindex()Finds position of element
Built-in Functions for Lists
FunctionPurposelen()Number of elementsmax()Maximum valuemin()Minimum valuesum()Sum of all elements

Problem Statements

Student Marks Management System

A teacher stores student marks in a list.
Tasks:

Create a list of marks
Show highest and lowest marks
Calculate average marks
Sort marks in ascending order

Uses: List creation, max(), min(), sum(), len(), sort()
Grocery Shopping List
Managing a monthly shopping list.
Tasks:

Create a grocery list
Add new items
Remove purchased items
Display final list

Uses: append(), remove(), indexing
Attendance Register
Recording daily attendance.
Tasks:

Store present students' roll numbers
Check if a student is present
Count total students present

Uses: in operator, count(), len()

Mobile Contact List

Storing phone contacts.
Tasks:

Create contact list

Add new contact

Delete existing contact

Show contacts alphabetically

Uses: append(), remove(), sort()

Temperature Analysis

Analyzing daily city temperatures.

Tasks:

Show temperatures for first and last 5 days

Find highest and lowest temperature

Calculate average temperature

Uses: Slicing, max(), min(), sum()

Results

List Creation & Properties

Created lists using [] and list() constructor
Confirmed: ordered, indexed, mutable, heterogeneous, allows duplicates

Indexing

Positive indexing (0, 1, 2...) - left to right ✓

Negative indexing (-1, -2, -3...) - right to left ✓

Slicing

Syntax list[start:end:step] worked correctly

Beginning, ending, and full slices successful

Original list stayed unchanged

List Methods Performance
MethodResultMethodResultappend()✓sort()✓insert()✓reverse()✓remove()✓count()✓pop()✓index()✓

Built-in Functions

len(), max(), min(), sum() - all worked perfectly

List Traversal

for loop and while loop both accessed elements correctly



1. Students marks management system

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

Conclusion
Everything worked great! Lists are:

Flexible: Store different data types and change easily
Easy to Access: Positive and negative indexing make it simple
Feature-Rich: Built-in methods handle common tasks (add, remove, sort, search)
Changeable: Perfect for data that needs updating
Practical: Useful for real-world problems in data management and analysis

