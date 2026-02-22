#Parth Dahiwade

#ENTC - A3 | PRN - 25070123177

#Experiment 7: Mastering Loops and Control Statements in Python

##Aim

To explore, understand, and practically implement the concepts of for loops, while loops, and loop control statements (break, continue, pass) in Python programming.

Theory: The Power of Iteration

In programming, repetition is one of the most common operations. Many real-world problems require performing the same task multiple times — such as processing items in a list, validating user input repeatedly, or analyzing large datasets. Writing repetitive code manually is inefficient and error-prone. To solve this problem, programming languages provide iteration structures, commonly known as loops.

A loop is a control structure that repeatedly executes a block of code either for a fixed number of times, or until a certain condition becomes false.

In Python, loops are simple yet powerful. They improve code efficiency, readability, and scalability.
Python provides two main types of loops:

For Loop (Definite Iteration)

While Loop (Indefinite Iteration)

In addition to loops, Python provides loop control statements that allow programmers to alter the normal flow of execution when required.

1. The For Loop (Definite Loop)
The for loop is used when the number of iterations is known in advance. It iterates over a sequence such as a list, tuple, string, range of numbers, or any iterable object. It automatically moves from one element of the sequence to the next until the sequence ends.
Why is it called a Definite Loop? Because the number of iterations is predetermined by the size of the sequence.

Algorithm – For Loop

Algorithm: FOR_LOOP_EXECUTION

Input  : A sequence S of n elements, a code block B

Output : Execute B for each element in S

BEGIN
  Step 1: Start

  Step 2: Initialize iterator i = first element of S
  
  Step 3: If S is exhausted, GOTO Step 6
  
  Step 4: Execute block B with current element i
  
  Step 5: Advance i to next element in S; GOTO Step 3
  
  Step 6: Exit loop
  
  Step 7: Stop

END

Syntax

pythonfor variable in sequence:
    # Code to execute
Practical Example
python# Printing numbers from 1 to 5
for i in range(1, 6):
    print(i)
```

Output: 1  2  3  4  5

### Advantages of For Loop

- Simple and readable
- Low risk of infinite loop
- Automatic iteration handling
- Best for traversing collections

---

## 2. The While Loop (Indefinite Loop)

The while loop executes a block of code as long as a specified condition remains True. It is used when the number of iterations is unknown, execution depends on user input, or a condition controls repetition.

*Why is it called an Indefinite Loop? Because the number of iterations is not fixed in advance — it depends entirely on the condition.*

### Algorithm – While Loop
```
Algorithm: WHILE_LOOP_EXECUTION

Input  : A condition C, a code block B

Output : Execute B repeatedly while C is True

BEGIN
  Step 1: Start
  Step 2: Initialize loop variable (e.g., i = 1)
  Step 3: Evaluate condition C
  Step 4: If C is False, GOTO Step 7
  Step 5: Execute block B
  Step 6: Update loop variable; GOTO Step 3
  Step 7: Exit loop
  Step 8: Stop
END

WARNING: If loop variable is not updated in Step 6,
         C may never become False → Infinite Loop
Syntax
pythonwhile condition:
    # Code to execute
Practical Example
pythoni = 1
while i <= 5:
    print(i)
    i += 1
```

Output: 1  2  3  4  5

### Comparison Between For and While Loops

| Feature | For Loop | While Loop |
|---|---|---|
| Type | Definite iteration | Indefinite iteration |
| Best Used When | Number of iterations is known | Iterations depend on condition |
| Variable Handling | Automatic | Manual |
| Infinite Loop Risk | Very Low | High if condition not updated |
| Common Use | Traversing sequences | Condition-based repetition |

---

## 3. Loop Control Statements

Sometimes, normal loop execution is not sufficient. We may need to stop the loop early, skip certain values, or leave space for future code. Python provides three important control statements: break, continue, and pass.

### 3.1 break – Loop Terminator

Immediately exits the loop. Control transfers to the statement after the loop. Commonly used in searching operations.

#### Algorithm – break
```
Algorithm: BREAK_STATEMENT
Input  : A loop with condition C, termination trigger T
Output : Exit loop immediately when T is encountered

BEGIN
  Step 1: Start loop
  Step 2: Fetch next element / evaluate condition C
  Step 3: If C is False (or sequence exhausted), GOTO Step 7
  Step 4: If current element == T (trigger condition):
              GOTO Step 7   [break – exit loop]
  Step 5: Execute loop body
  Step 6: GOTO Step 2
  Step 7: Exit loop
  Step 8: Continue with statements after loop
  Step 9: Stop
END
pythonfor i in range(1, 10):
    if i == 5:
        break
    print(i)
```

Output: 1  2  3  4

---

### 3.2 continue – Skip Current Iteration

Skips the remaining statements in the current iteration and moves control back to the top of the loop. Used to ignore unwanted values.

#### Algorithm – continue
```
Algorithm: CONTINUE_STATEMENT
Input  : A loop, a skip condition K
Output : Skip iteration when K is True, otherwise execute body

BEGIN

  Step 1: Start loop
  
  Step 2: Fetch next element / evaluate loop condition
  
  Step 3: If loop ends, GOTO Step 8
  
  Step 4: If current element satisfies K (skip condition):
              GOTO Step 2   [continue – skip rest of body]
  
  Step 5: Execute remaining loop body
  
  Step 6: Update loop variable (if while loop)
  
  Step 7: GOTO Step 2
  
  Step 8: Exit loop
  
  Step 9: Stop

END

pythonfor i in range(1, 6):
    if i == 3:
        continue
    print(i)
```

Output: 1  2  4  5

---

### 3.3 pass – Null Statement

Does nothing. Acts as a placeholder. Used when syntax requires a block but no action is needed yet.

#### Algorithm – pass
```
Algorithm: PASS_STATEMENT

Input  : A loop body requiring syntactic completeness

Output : No operation; execution continues normally

BEGIN

  Step 1: Start loop
  
  Step 2: Fetch next element / evaluate loop condition
  
  Step 3: If loop ends, GOTO Step 6
  
  Step 4: Execute pass  [NOP – no operation performed]
  
  Step 5: GOTO Step 2
  
  Step 6: Exit loop
  
  Step 7: Stop

END

NOTE: pass is syntactically valid but semantically empty.
      It serves as a placeholder for future implementation.
pythonfor i in range(5):
    pass
```

---

## 4. Implementation of Control Statements

### Example A: Inside a While Loop

#### Algorithm – Combined While Loop with break, continue, pass
```
Algorithm: WHILE_WITH_CONTROLS

Input  : i = 1

Output : Print selected numbers from 1 to 10

BEGIN

  Step 1:  Start; set i = 1
  
  Step 2:  If i > 10, GOTO Step 10
  
  Step 3:  If i == 3: execute pass (no effect); proceed
  
  Step 4:  If i == 5: increment i by 1; GOTO Step 2  [continue]
  
  Step 5:  If i == 8: GOTO Step 10                   [break]
  
  Step 6:  Print i
  
  Step 7:  Increment i by 1
  
  Step 8:  GOTO Step 2
  
  Step 9:  (unreachable after break)
  
  Step 10: Exit loop
  
  Step 11: Stop

END

Expected Output: 1, 2, 3, 4, 6, 7

pythoni = 1

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
```

Output: 1  2  3  4  6  7

---

### Example B: Inside a For Loop

#### Algorithm – Combined For Loop with break, continue, pass
```
Algorithm: FOR_WITH_CONTROLS

Input  : range(1, 11)

Output : Print selected numbers from 1 to 10

BEGIN
  
  Step 1:  Start; initialize range(1, 11)
  
  Step 2:  Fetch next i from range; if exhausted GOTO Step 9

  Step 3:  If i == 3: execute pass (no effect); proceed
  
  Step 4:  If i == 5: GOTO Step 2               [continue]
  
  Step 5:  If i == 8: GOTO Step 9               [break]
  
  Step 6:  Print i
  
  Step 7:  GOTO Step 2
  
  Step 8:  (unreachable after break)
  
  Step 9:  Exit loop
  
  Step 10: Stop

END

Expected Output: 1, 2, 3, 4, 6, 7
pythonfor i in range(1, 11):
    if i == 3:
        pass
    if i == 5:
        continue
    if i == 8:
        break
    print(i)
Output: 1  2  3  4  6  7

5. Real-World Applications of Loops

Searching for an element in a dataset

Validating passwords

Processing student marks

Generating reports

Game development logic

Automation scripts

Data analysis

Loops are foundational in almost every Python program.

Conclusion

In this experiment, we studied and implemented Python's primary iteration mechanisms: the for loop and the while loop. We also designed step-by-step algorithms for each construct and its associated control statements.
We explored the importance of control statements:

break — for early termination of a loop

continue — for skipping unwanted iterations

pass — as a structural placeholder for future code

The algorithms developed for each control statement help in understanding the precise flow of execution and serve as a blueprint before actual implementation. Understanding loops and control statements is essential for writing efficient, readable, and scalable programs. Mastery of these constructs forms the backbone of Python programming.
