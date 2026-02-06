Experiment–5

Title
Implementation of Set and Dictionary in Python

Aim

To learn and work with sets and dictionaries in Python and perform various operations on them.
Objectives

Understand what sets are
Create sets and perform basic operations
Use mathematical set operations
Understand dictionary structure
Insert, delete, and access data in dictionaries
Apply dictionary methods

Theory on Sets

What is a Set?
A set is a collection of unique elements with no particular order. Sets use curly braces {} or the set() constructor.
Characteristics of Sets

Unordered
No duplicate elements
Mutable (can be changed)
Doesn't support indexing

Sets are useful for removing duplicates, checking membership, and mathematical operations.
Set Operations

Union (combine all elements)
Intersection (common elements)
Difference (elements in one but not the other)
Symmetric Difference (elements in either but not both)

Applications of Sets

Removing duplicate records
Membership testing
Mathematical computations

Programs on Sets
Program 1: Creating a Set and Displaying Elements
pythonfruits = {"apple", "banana", "cherry"}
print("Fruits:", fruits)
Program 2: Removing Duplicate Values
pythonnumbers = {1, 2, 3, 2, 4, 1}
print("Unique numbers:", numbers)
Program 3: Set Operations
pythonA = {1, 2, 3, 4}
B = {3, 4, 5, 6}
 
print("Union:", A | B)
print("Intersection:", A & B)
print("Difference:", A - B)
print("Symmetric Difference:", A ^ B)
Program 4: Set Methods
pythons = {10, 20, 30}
s.add(40)
s.remove(20)
 
print("Updated Set:", s)
Theory on Dictionary
What is a Dictionary?
A dictionary stores data as key-value pairs. Each key must be unique, but values can repeat.
Syntax:
pythondictionary = {key: value}
Dictionaries are great for student records, phone books, and configuration data.
Characteristics of Dictionary

Key-value based
Mutable
Keys are unique
Values can be modified

Applications of Dictionary

Student information systems
Phone directories
Database records
Configuration files

Program 1: Creating and Accessing Dictionary

student = {
    "roll": 101,
    "name": "Amit",
    "branch": "CSE"
}

print("Name:", student["name"])
________________________________________
Program 2: Adding and Updating Elements
student["year"] = "Second"
student["name"] = "Rahul"

print(student)
________________________________________
Program 3: Removing Elements
student.pop("branch")
print("After removal:", student)
________________________________________
Program 4: Dictionary Methods
print("Keys:", student.keys())
print("Values:", student.values())
print("Items:", student.items())
________________________________________
Program 5: Iterating Through Dictionary
for key, value in student.items():
    print(key, ":", value)
________________________________________
Applications of Dictionary
•	Student information systems
•	Phone directories
•	Database records
•	Configuration files
________________________________________

Summary of Results

OperationStatusSet creation✓Duplicate removal✓Union, Intersection, Difference✓Set methods (add, remove)✓Dictionary creation✓Dictionary access✓Adding/Updating elements✓Removing elements✓Dictionary methods✓Dictionary iteration✓
Conclusion
Sets:

Efficiently handle unique data
Support mathematical operations (union, intersection, difference)
Great for removing duplicates and membership testing
All set operations worked successfully

Dictionaries:

Provide efficient key-value storage
Allow quick data retrieval using keys
Support adding, updating, and removing elements
Essential for real-world applications like databases and configuration files
All dictionary methods worked perfectly

Conclusion
Sets efficiently handle unique data and support mathematical operations, making them useful for data processing tasks.
Dictionaries provide efficient storage and retrieval of data using keys, making them essential for real-world applications.
