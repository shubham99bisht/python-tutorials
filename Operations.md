
# Operations and Built-in functions

We have looked over variables in that last tutorial, now we're trying to use these variables and perform some operations on them. Most basic operations include just arithmetic operations like: add, substract, multiply, devide and exponent. We can even perform some built-in operations on variables to manipulate over data.

## Simple math

Math is a pretty popular topic, so we should probably learn how to do it in Python 3. Luckily for us, math is so very popular that it works extremely simply.


> 7+6                adds two numbers (or subtract using -)
> 
> 13*3               multiply operands
>
> 56/2               division (results in float value)
>
> 9//2               floored division (results in int datatype)
>
> 5**2               exponential function (another approach exp(5,2))

That's it for basic math. It really is quite simple. Math is quite integral to a lot of programs, so it is very nice that it is kept simple enough.


```python
print(7+6)
print(13*3)
print(56/2)
print(9//2)
print(5**2)
```

    13
    39
    28.0
    4
    25


You can even perform these operations directly on the variables, refering them by variable names


```python
var1 = 4
var2 = 3

var3 = var1 ** var2
print("Example for exponential operation: 4**3 = ",var3)

print("Example of inline addtion: 4+3 = ", var1 + var2)
```

    Example for exponential operation: 4**3 =  64
    Example of inline addtion: 4+3 =  7


## Built-in operations

> abs( )
>
> help( )
>
> max( ) min( )
>
> int( ), str( ), float( )


```python
#Absolute Values: Return the absolute value of the argument

exNum1 = -5
exNum1 = abs(exNum1)
print(exNum1)
```

    5


>**The Help function:**

>This is probably one of the most under-utilized commands in Python, many people do not even know that it exists. With help(), you can type it with empty parameters to engage in a search, or you can put a specific function in question in the paramete


```python
import time
# will work in a typical installation of Python, but not in the embedded editor
help(abs)
```

    Help on built-in function abs in module builtins:
    
    abs(x, /)
        Return the absolute value of the argument.
    


> **Max and Min:**

>How to find the maximum or highest number in a list or how to find the lowest or minimum number in a list.

> List will be described later, it is a just data-type to store more than one values.


```python
exList = [5,2,1,6,7]

largest = max(exList)
print(largest)

smallest = min(exList)
print(smallest)
```

    7
    1


>**Converting data types:**

>Many times, like reading data in from a file, you might find the datatype is incorrect, like when we mean to have integers, but they are currently in string form, or visa versa.

**Converting a string to an integer**


```python
intMe = '55'
intMe = int(intMe)
print(intMe)
```

    55


**Converting and integer to a string:**


```python
stringMe = 55
stringMe = str(stringMe)
print(stringMe, type(stringMe))
```

    55 <class 'str'>


**Converting an integer to a float:**


```python
floatMe = 55
floatMe = float(floatMe)
print(floatMe, type(floatMe))
```

    55.0 <class 'float'>


> **You can also convert floats to strings, strings to floats, and more. Just make sure you do a valid operation. You still cannot convert the letter h to a float.**

In this tutorial, we cover a handful of the built-in functions with Python 3. For a full list, see: https://docs.python.org/3/library/functions.html

### That's all about Operations. Play around with these code and try to make your own programs.


### Thank you for reading. Once you feel comfortable with them, proceed to the next tutorial.

>If you have any queries or suggestions to improve this tutorial please contact me [here](https://www.skillconnect.wixsite.com/home) or you can connect me on [linkedin](https//:www.linkedin.com/shubham99bisht)
