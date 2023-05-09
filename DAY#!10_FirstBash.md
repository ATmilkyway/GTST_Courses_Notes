# Introduction to BASH scripting

<u><b>Topics</b></u>

+ what is bash
+ use of bash for hackers
+ Output,
+ variables & data type
+ Input
+ comment and indentations
+ Arithmetic operation
+ if-else

## What is Bash Script?
+ Bash = Bourne Again Shell
+ It is a shell, that used to interact with your kernel.
## What is Script?
+ Script is a file that contains shell commands.
+ The original is sh - Bourne shell

## Uses of bash
+ Script development
+ Simplifying tasks
+ Simplifying your linux ability
+ Developing hacking scripts

## Starting with Bash
+ Bash files can have “.sh” extention but you can have it with out .sh too
+ The file have to have executable Permissions.

👉 You can use any text editors u need: VIM,nano,VScode,gedit,cherrytree…


## The shebang
+ <b>#!/bin/bash</b> when used in scripts is used to instruct the operating system to use bash as a command interpreter
## Why shebang is used in shell script?
+ The shebang is the combination of the # (pound key) and ! (exclamation mark). This character combination has a special meaning when it is used in the very first line of the script. It is used to specify the interpreter with which the given script will be run by default.

+ In computing, a shebang is the character sequence consisting of the characters number sign and exclamation mark at the beginning of a script. It is also called sharp-exclamation, sha-bang, hashbang, pound-bang, or hash-pling.

## Displaying output
+ To start Every bash scripts use shebang.
    + #! /bin/bash
    + #! /bin/sh
+ To display outputs on bash you just do
  + echo “YOUR TEXT HERE”
+ To run your project you can do:
  + /bin/bash hello.sh
## Variables
👉Bash Variables are same with python variables, with some exceptions.

VARIABLE_NAME=value

👉Exceptions:
+ NO Space between the equal sign ( = )

👉USE double quotes only.

👉To use the variable we will use dollar sign($) before the Variable name

👉If you want to display the variable sticked with other text use ${VARIABLE_NAME}

👉Bash Variables are string by default.

## Set
The set command can be used to assign values to positional parameters.

+ set value1 value2 value3 value4 value5

## System Variables
+ Are variables those are declared by the system.
+ There are so many: LANG, TERM,MAIL,EDITOR,USER,SHELL….
+ USER displays Computer owner(host)

## Variables & Data Types
So to create other data types we use declare.

Arrays

Arrays are lists or tuples on python.

var=(“list1” “list2” “list3” “list4)

1. To display echo

       ${var[0]}
2. To get all the elements

       ${var[@]}
3. To get the indexes
      
       ${!var[@]}
4. To get the length

       ${#var[@]}
5. To add element to the array 

       var[4]=”list5”
6. To remove from the array

       unset var[3]

## Bash Input
+ On bash we have 2 methods to accept input
    1. Read function
    2. Arguments

1. Bash read
● Read used to accept inputs while the script is running.
 
        read -p      # “Text To Display” var
        read -sp     # “Password: ” var => used to accept hidden texts like password.
        read -a var  # for accepting arrays(lists)

2. Arguments
+ These helps to get input before the script starts
 
+ Just use $0-$9 while you want to work with the input

## Comments
multi line comment we start with
<< COMMENTS
Sfasf
Sfa
COMMENTS>> 

## Bash sleep
+ Sleep used to make a good waiting on our script.
    + sleep < number >s

## Operation
+ To do mathematical operations you have to do $(( expression ))
+ we will use let keyword for assigning variable

A) Arithmetic Operations

1. Addition $(( a + b ))
2. Subtraction $(( a - b ))
3. Multiplication $(( a * b ))
4. Division $(( a / b ))
5. Exponential $(( a ** b ))
6. Modulo $(( a % b ))

B) Assignment Operations

1. Increment “let a+= 3”
2. Decrement “ let a-= 3”
3. Multiply “ let a*= 3 “
4. Divide “ let a/=3 “


C) Comparison operation
Alphabetic comparison
1. Greater Than => -gt
2. Less Than => -lt
3. Greater than and equals to => -ge
4. Less than and equals too => -le
5. Equal => -eq
6. Not equal => -ne

Sign comparison

> , < , >= , <= , = , !=

## If else conditions

👉 On bash we don't have indentation but
if u finished writing the body you type
“fi”
