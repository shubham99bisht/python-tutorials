
# Python Print function, String and Variables
NOTE: '__#__' is used in python for single line comments and triple quotes (''' or """) are used to mutli-line comments

## print function

>print( )

The print function in Python is a function that outputs to your console window whatever you say you want to print out. It is actually one of the most widely used functions in all of python. The reason for this is that it makes for a great debugging tool.

"Debugging" is the term given to the act of finding, removing, and fixing errors and mistakes within code.

If something isn't acting right, you can use the print function to print out what is happening in the program. Many times, you expect a certain variable to be one thing, but you cannot see what the program sees. If you print out the variable, you might see that what you thought was, was not.



There are a number of ways in which a print function can be used. Syntax is always the same but little bit changes depending upon what we are trying to print.

> print("hello")
>
> print("hello" + "there")
>
> print("hello","world")
>
> print(5)
>
> print(5+9)
>
> print(9/2)
>
> print(172.782)

* ### printing a statement: anything inside quotes are directly printed


```python
#prints everything inside quotes
print("Hello world, this function prints anything written inside quotes")
print('Even single quotes work fine!')
```

    Hello world, this function prints anything written inside quotes
    Even single quotes work fine!


>You can print two strings inside a single print. Strings can be concatenated using '__,__'(comma) or '__+__'(plus)
Difference between the two is, using '__+__' won't add a space between two strings and just stick them together while '__,__' would add a space between the two strings.

>It's not limited to just two strings, any number of strings can be concatenated. As we see later we can even concatenate variable values to strings for printing results.


```python
print("hello"+"world")     #No space added while attaching strings
print("hello","world")     #Space is added while printing
```

    helloworld
    hello world


* ### printing numbers, numbers with strings, performing operations


```python
#prints any integer or floating decimal
print(5)            #same for both integer and float
print(19.768)

#Can even perform calulations inside print
print(16+5)  #note: doesn't print 165
print(5*6)
print(9/2)
print(9//2)

#NOTE: Dividing using single '/' gives results as a float value whereas using '//' gives floored integer value
```

    5
    19.768
    21
    30
    4.5
    4



```python
#prints string and integer in one line

print("Hi",5)

#But, you can't add a string and a integer, therefore '+' wont work
#print("hi"+5)   WRONG SYNTAX

#RIGHT SYNTAX FOR PRINTING NUMBER + STRING

print("hi"+str(5))   # str() converts any interger to string, which can be concatenated with other strings

```

    Hi 5
    hi5


* ### printing from variables

A variable can be defined as 'variable_name = 5(value)'.
More on variables later, right now we just focusing on print function


```python
#prints value of a variable

var_name = 10
print(var_name)

# Note: using quotes will result in printing the 'var_name' as a string

print("var_name",var_name)
# OR
print('var_name = ' + str(var_name))
```

    10
    var_name 10
    var_name = 10


* ### printing multiple times


```python
#prints string 5 times

print("hello "*5)
#Note this will not work for integers as it will multiply and print the product
```

    hello hello hello hello hello 


## Variables

> var_name1 = "Hello"
>
> var_name2 = 5
>
> var_name3 = 1123.12312

In almost every single Python program you write, you will have variables. Variables act as placeholders for data. They can aid in short hand, as well as with logic, as variables can change, hence their name.

Variables help programs become much more dynamic, and allow a program to always reference a value in one spot, rather than the programmer needing to repeatedly type it out, and, worse, change it if they decide to use a different definition for it.

Variables can be called just about whatever you want. You wouldn't want them to conflict with function names, and they also cannot start with a number.

You want to be careful what you name variables, classes (discussed later), and functions (discussed later), so that they do not have the same names as eachother.

For example, you have leared about the print function. What if you go and define a variable named print?

Say, for example, you do:

> print = print("Uh oh!")

Now you have a variable and a function named print, which can cause trouble down the road!


> var_name4 = 7/4

We can even store a variable to our variable, or an operation with our variables to a variable. Something like **var3 = (var2/var1)** would work. You can store other things, like functions, as well to variables. More on that later!

Try playing with variables in the console provided by Python installation. 

## Input Function : taking user input
***

> input()
>
> input(" Enter data: ")

* ### Taking user input


```python
name = input()  #takes input from user and stores data into 'name' variable
print(name)     #print contents of name(variable)
```

    John
    John


> We can add a small message to be prompted for making user know that console is waiting for input

> Similar to print(), we can print the prompt by passing the message inside braces.


```python
name = input("Enter your name here: ")
print(name)
```

    Enter your name here: shubham
    shubham


> The most important thing to note about print function is it takes input data and converts it into string. Even if an integer or a float is passed, it is converted into a string and then stored into the variable.
>
> For handling integers or taking input in other datatypes like float, complex etc then we have to explicitly convert the input() into that data type.


```python
var_int = int(input("Enter a integer value: "))
var_float = float(input("Enter a float value: "))
var_complex = complex(input("Enter a complex value: "))

print(var_int)
print(var_float)
print(var_complex)
```

    Enter a integer value: 67
    Enter a float value: 12.45
    Enter a complex value: 2+5j
    67
    12.45
    (2+5j)

***
### That's all about strings, variables and print and input function. Play around with these code and try to make your own programs. For executing python code from terminal or cmd prompt, go to the directory where the python file is stored and type:

> python filename.py

### Thank you for reading. Once you feel comfortable with them, proceed to the next tutorial.

>If you have any queries or suggestions to improve this tutorial please contact me [here](https://skillconnect.wixsite.com/home) or you can connect me on [linkedin](https://www.linkedin.com/in/shubham99bisht/)
