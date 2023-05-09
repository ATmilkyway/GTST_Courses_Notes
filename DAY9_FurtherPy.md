# Further on Python

<u><b>Topics</b></u>
  + Functions,recursion
  + lambda → Map/filter
  + OOP & POP
  + Class & objects
  + user-built Module

## Functions
+ A function is a block of code that performs a specific
task.
+ Dividing a complex problem into smaller chunks makes our program easy to understand and reuse.

## Types of function
1. <b>Standard library functions</b> - These are built-in functions in Python that are available to use.
      + Almost all keywords are functions
2. <b>User-defined functions</b> - We can create our own functions based on our requirements.

## Creating FUnctions

    def function_name(argument)
 
## Return statement
If we want our function to return some value to a function call, we use the return statement.

## Recursion
+ Recursion is process of defining something in terms of itself.
+ In Python, we know that a function can call other functions. It is even possible for the
function to call itself. These types of construct are termed as recursive functions

## Anonymous / lambda Function
+ If function doesn't have name it is called lambda function / Anonymous
+ If you have 1 line code to return you dont need to def a function,
+ a lambda function is a special type of function without the function name.

      lambda arguments : expression

👉 We use lambda keyword instead of def

## Function takers function
The filter() function returns an iterator where the items are filtered through a function to test if the item is accepted or not.

    filter(function, iterable)
● Filter, map & reduce takes a function as an argument.

    ages = [5, 12, 17, 18, 24, 32]

    def myFunc(x):
      if x < 18:
        return False
      else:
        return True

    adults = filter(myFunc, ages)

    for x in adults:
      print(x)
  #

     # 18
     # 24
     # 32

👉 OR

    adults = filter(lambda a:a>=18, ages)

    for x in adults:
      print(x)
  #
    num=[1,2,3,4,5,6,7,8,9]
    evens=list(filter(lambda a:a%2==0,num))
    [2, 4, 6, 8]  # as list
    i.e The list() function creates a list object.
    # 2
    # 4
    # 6
    # 8  

## Map function
Used to do some operations on Sequences, mostly used for opeerations

    def myfunc(a):
      return len(a)

    x = map(myfunc, ('apple', 'banana', 'cherry'))

    print(x)

    #convert the map into a list, for readability:
    print(list(x))

+ The map() function executes a specified function for each item in an iterable. The item is sent to the function as a parameter.

## Append
+ Append used to add some value to a list.
  mylist.append(new_value)


## Object-Oriented Programming / OOP
+ Python is an object oriented programming. This means mores things on python are objects.
  + Objects are anythings which can have action and name.
  + Objects have attributes(properties) and methods(action or functions)

 + Example : My Computer
    + Attribute: name,size,cpu,ram…
    + Behaviour: Running games, playing music, displaying texts…

## Python class and object
+ Class is simply a place where we create our Object’s attribute and behaviour in blueprint
+ a class is a blueprint for that object.
    
        class Class_Name
## Creating Objects
    Var = classname()
    Var.attribute = “value”

## Python Constructors
    __init__() 
+ is the constructor function that is called whenever a new object of that class is instantiated.

## Python Inheritance
+ Is a way of creating new class with some properties of existing class.

      class newclass(oldclass): 


## Python Encapsulation
+ Encapsulation is Feature of OOP, That refers to bundling of attributes and methods inside a single class.


