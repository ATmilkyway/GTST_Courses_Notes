# Core of Python Programming

<u><b>Topics</b></u>
+ indexing and slicing{start,stop,step}
+ input handling{2 methods}
+ Operations
+ indentation
+ if else
+ Errors (Exceptions)
+ Error handling
+ loops

## Indexing
+ Calling texts by indexes also works for strings & tuples

## Slicing
+ In Python it is possible to access a section of items from the list using the slicing operator 👉‘ : ‘ 

        Mylist[ start : stop : step ]

+ Slicing is indexing syntax that extracts a portion from a list. If a is a list, then a[m:n] returns the portion of a:
    + Starting with postion m
    + Up to but not including n
    + Negative indexing can also be used

## User Input handling
+ On python there are 2 types of inputs
  + By input function
  + By Arguments
1) By input functions,
    + var = input(“Text you like to display: ”)
 2) Arguments
    + Shell: python gtst.py arg1 arg2 arg3

            import sys
            name = sys.argv[1]
            print(f"Hello{name}")

👉 starts from index 1 rember

There are lots of operators type on python:
<ol>
    <li>Arithmetic operators</li>
    <li>Assignment Operators</li>
    <li>Comparison Operators</li>
    <li>Logical Operators</li>
    <li>Bitwise Operators</li>
    <li>Special Operators</li>
</ol>

## Indentations
+ Are Just a WhiteSpace which python uses for some of its function. If
there is no proper indentation error then you are doomed.

## If-else conditions
In Python, there are three forms of the if...else statement.
1. if statement
2. if...else statement
3. if...elif...else statement

## Nested if statements
We can also use an if statement inside of an if statement. This is known as a nested if statement

## Logical Errors ( Exceptions)
Errors that occur at runtime (after passing the syntax test) are called
exceptions or logical errors.

## Error handling
For handling errors we use try…except blocks

## Python Loops
There are 2 types of loops in Python:
  + For Loop
  + While Loop

## Range keyword
A range is series of values between two numeric intervals. 
range(size)

## len keyword
A len is used to show the length of a sequence
may be list,tuple or staffing. len(list)

 


##  :fire:Difference between <b>for</b> and <b>while</b>:fire:
for loop :
  + is usually used when the number of iterations is known.

while :
  + loop is usually used when the number of iterations are unknown. When we have condition.

##  break
Break used to exit from an infinite loop