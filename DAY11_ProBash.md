# Further on Bash!

<u><b>Topics</b></u>

+ Regular expressions
+ Else if
+ loops
+ functions
+ bash and linux shell

## Regular Expressions! /regex/
+ Most filter Validation on any platform done by Regular expression/regex/.
+ Regex is PATTERN!
+ Regex are used on linux tools called grep,awk and sed 

## Metacharacters
+ Those are regex pattern symbols for filter.

        .
        ^
        $
        *
        +
        ?
        { }

### Dot ( . )
+ Used to get All the line except new lines
    + Syntax: .
+ This means give me all lines except the new lines

### Caret ( ^ ) - <b>Assertion</b>
+ Used to get line that start with pattern
    + Syntax: ^hello
+ This means lines that start with hello

### Dollar sign( $ ) - <b>Assertion</b>
+ Used to get line that ends with some pattern.
    + Syntax: hello$
+ That ends with hello

### Plus ( + ) - <b>Quantity</b>
+ Used to get line that have pattern that occurs <b>👉1 and more times.</b>
+ Syntax: hellos+
+ A text hello that have s at least 1 times and more.
### Asteriks ( * ) - <b>Quantity</b>
+ Used to get line that have pattern that occurs <b>👉0 and more times.</b>
    + Syntax: hellos*
+ A text hello that have s at least 0 times and more.

+ We need to get texts that starts with n and ends with com including all the texts between those 2 expressions
    + Start with n = ^n
    + End with com = com$
    + All Test between them = .* , .+

We can do it in 1 line

 👉^n.*com$

### Curly Bracket ( { min , max} ) - <b>Quantity</b>
+ Used to get line that have pattern that occurs min and max times.it is custom
  + Syntax: hellos{1,3}
+ A text hello that have s at least 0 times and more.

### \w
+ Used to get Alphanumeric
    + Syntax: \w
+ All texts except newlines and symbols

### \s
+ Used to get whitespace.
    + Syntax: \s

### \S
+ Used to get all except whitespace.
    + Syntax: \S

### \d
+ Used to get Digits/numbers/
    + Syntax: \d
### \D
+ Used to get all except Digits/numbers/
    + Syntax: \D
### Pipe ( | ) - OR
+ Used to search 2 different things.
    + Syntax: a|b
### Escape ( \ )
+ Used to search symbols that are metacharacters.
  + Syntax: \sign

### Square Brackets ( [ ] ) - Custom pattern
+ Used to Create your own patterns
  + Syntax: [pattern]

👉 You cant get small letters with the \w or built in patterns.

[Read More](https://www.geeksforgeeks.org/write-regular-expressions/)

    john@gmail.com
    natanhailu@yahoo.com
    micky43@geeztecg.net
    rexder@gmail.com
    Hello there this is me
    My phone number 0987654321

    ^.*@.*\.(com|net)

## BASH FOR REGEX
+ We can use =~ operator for regex check with if condition statements


        #! /bin/bash

        read -p "Enter Number : " num
        echo
        pattern="[0-9]"

        if [[ $num =~ ${pattern} ]]
        then
        echo "Good"
        else
        echo "Bad"
        fi
#
Email Validetor

    if [[ "$email" =~ ^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,4}$ ]]
    then
        echo "Email address $email is valid."
    else
        echo "Email address $email is invalid."
    fi


## Bash else if
👉 To do more than 1 comparing.
+ It is same with python is is “elif”

## Loops
+ On Bash, there are 3 types of loops

    1. For loop
    2. While loop
    3. Until loop
1. for Loop

       for num in {1..10}
       do 
       echo $num
       done

2. while

        while [expression]
        do 
            body
        done
3. Until loop
+ It is same but this one exits the loop when the expression is true.
+ The name until means እስከ

        until [expression]
        do 
            body
        done    

## Function

    function_name(){
        body
    }
#
+ When you have function and the arguments will be $1, $2 ….
  + If we use $? it will call the return value.

        print_it(){
            sum=$(($1+$2))
            echo "the sum : $sum"
        }

        print_it 5 6

## BASH and Linux
+ We can run linux commands inside our bash
+ You can run bash codesin 1 line.
+ You can access files in current directory using * sign

        #!/bin/bash

        echo *

        