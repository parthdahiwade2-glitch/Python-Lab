Parth Dahiwade 

ENTC - A3

PRN - 25070123177

Experiment 7: Mastering Loops and Control Statements in Python

Aim -

To explore, understand, and practically implement the concepts of for loops, while loops, and loop control statements (break, continue, pass) in Python programming.

Theory: The Power of Iteration

In programming, repetition is one of the most common operations. Many real-world problems require performing the same task multiple times — such as processing items in a list, validating user input repeatedly, or analyzing large datasets. Writing repetitive code manually is inefficient and error-prone. To solve this problem, programming languages provide iteration structures, commonly known as loops.

A loop is a control structure that repeatedly executes a block of code either:

For a fixed number of times, or

Until a certain condition becomes false

In Python, loops are simple yet powerful. They improve code efficiency, readability, and scalability.

Python provides two main types of loops:

For Loop (Definite Iteration)

While Loop (Indefinite Iteration)

In addition to loops, Python provides loop control statements that allow programmers to alter the normal flow of execution when required.

1. The For Loop (Definite Loop)

The for loop is used when the number of iterations is known in advance. It iterates over a sequence such as:

A list

A tuple

A string

A range of numbers

Any iterable object

It automatically moves from one element of the sequence to the next until the sequence ends.

Why is it called a Definite Loop?

Because the number of iterations is predetermined by the size of the sequence.

Syntax
for variable in sequence:
    # Code to execute

Working Principle

The loop variable takes the value of each element in the sequence.

The block of code runs once for each value.

The loop automatically stops when all elements are exhausted.

Practical Example

# Printing numbers from 1 to 5
for i in range(1, 6):
    print(i)

Output
1

2

3

4

5

Advantages of For Loop

Simple and readable

Low risk of infinite loop

Automatic iteration handling

Best for traversing collections

2. The While Loop (Indefinite Loop)

The while loop executes a block of code as long as a specified condition remains True.

It is used when:

The number of iterations is unknown.

Execution depends on user input.

A condition controls repetition.

Why is it called an Indefinite Loop?

Because the number of iterations is not fixed in advance. It depends entirely on the condition.

Syntax

while condition:

    # Code to execute

Working Principle

The condition is checked.

If True → the loop body executes.

After execution, the condition is checked again.

The loop stops when the condition becomes False.

Practical Example
i = 1
while i <= 5:
    print(i)
    i += 1

Output
1

2

3

4

5

⚠ Important Note:

If the loop variable is not updated properly, the condition may never become False, resulting in an infinite loop.

Comparison Between For and While Loops

Feature	For Loop	While Loop

Type	Definite iteration	Indefinite iteration
Best Used When	Number of iterations is known	Iterations depend on condition
Variable Handling	Automatic	Manual
Infinite Loop Risk	Very Low	High if condition not updated
Common Use	Traversing sequences	Condition-based repetition
3. Loop Control Statements (Controlling Execution Flow)

Sometimes, normal loop execution is not sufficient. We may need to:

Stop the loop early

Skip certain values

Leave space for future code

Python provides three important control statements:

1. break (Loop Terminator)

Immediately exits the loop.

Control transfers to the statement after the loop.

Commonly used in searching operations.

Example:
for i in range(1, 10):
    if i == 5:
        break
    print(i)


Output:

1

2

3

4

2. continue (Skip Current Iteration)

Skips the remaining statements in the current iteration.

Moves control back to the top of the loop.

Used to ignore unwanted values.

Example:
for i in range(1, 6):
    if i == 3:
        continue
    print(i)


Output:

1

2

4

5

3. pass (Null Statement)

Does nothing.

Acts as a placeholder.

Used when syntax requires a block but no action is needed yet.

Example:

for i in range(5):
    pass

Implementation of Control Statements
Example A: Inside a While Loop
i = 1

while i <= 10:
    if i == 3:
        pass

    if i == 5:
        i += 1
        continue

    if i == 8:
        break

    print(i)
    i += 1

Output
1
2
3
4
6
7

Example B: Inside a For Loop
for i in range(1, 11):
    if i == 3:
        pass

    if i == 5:
        continue

    if i == 8:
        break

    print(i)

Output
1
2
3
4
6
7

Real-World Applications of Loops

Searching for an element in a dataset

Validating passwords

Processing student marks

Generating reports

Game development logic

Automation scripts

Data analysis

Loops are foundational in almost every Python program.

Conclusion

In this experiment, we studied and implemented Python’s primary iteration mechanisms: the for loop and the while loop.

We also explored the importance of control statements:

break for early termination

continue for skipping unwanted iterations

pass as a structural placeholder

Understanding loops and control statements is essential for writing efficient, readable, and scalable programs. Mastery of these constructs forms the backbone of problem-solving in Python programming.
