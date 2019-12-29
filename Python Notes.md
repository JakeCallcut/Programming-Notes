# **PYTHON NOTES**
***

## Fundamentals

>Python is a very high level, useful programming language for making simple programs developing applications, and solving problems.

>everything in Python occurs inside the terminal, he terminal is at the heart of all of the proccesses in Python even with a graphical user interface all proccesses are run in the terminal.

## Comments

	''' 
	multi 
	line 
	comment
	'''

	#single line comment

## Basic Syntax
### Output

	print("this is how to output on screen")

If you are outputting a variable you do not need to use quotes:

	print(variable)

### Input

you can take input to a variable with the following syntax:

	name = input("what is your name? ")

### IF statements
an if statement can be created using the following syntax:

	if age < 17:
		print("you may not drive")
	else:
		print("you may drive with a licence")


## Variables
>Python is what we call a "dynamic type" language, this means that we do not have to declare the data type when we create a variable.

	car = "ford"

### Concatenation
>to combine or concatenate strings and variables use this syntax:

	print("I have a " + car)
	
## Functions

>functions are a huge part of Python and allow us to do a lot more things with our code.

here are some of the most basic and useful ones:

	len(variable)

this will return the length of the variable in the brackets

	str(variable)

this will turn the variable into a string for example:
the integer 67000 will become the string "67000"

	variable.upper()

this will turn the entire string uppercase for example:
"Hello There" will become "HELLO THERE"

	Variable.lower()

this does the exact opposite, turning everything in the string to lower case.

### Dot notation
some functions use dot notation (variable.upper() for example)
rather than putting the variable in the parentheses

this is because dot notation can only be used on string variables

## Date and Time

	from datetime import datetime

this line imports the function of date and time into the program. 

the current date and time can be printed using the following syntax:
	
	print(datetime.now())	

>this will print the date and time in the form "YYYY-MM-DD HH:MM:SS"

	now.month
	now.year 
	now.day

these functions will output the current month, year and day respectively

	from datetime import datetime
	now = datetime.now()
	print '%02d/%02d/%04d %02d:%02d:%02d' % (now.month, now.day, now.year, now.hour, now.minute, now.second)

this slice of code will output the date and time in a niceer format

## Substrings

>a substring is a part of a string which can be extracted using a functions

you can extract the substring using the following syntax:

	string = "hello this is a string"
	substring = string[0:4]

	print(substring)

this will print "hello"

the two parameters in the square brackets are the start and the end of the substring,

if you leave the end of last parameter blank, the subtring will carry on until the end of the string

## Arrays

>in Python arrays are called Python lists, they are essentially the same thing.

>arrays are a one dimensional set of separate variables.

arrays can be created by using the following syntax:

	Cars = ["volvo", "ford", "peugeot"]
	FavNumbers = [24, 64, 2]

arrays can be made with any data type

different items of the array can be addressed using square brackets, using the following syntax

	Cars[3] = "nissan"
	FirstCar = Cars[0]

you can manipulate this by using variables in its place, for example, you can cycle through an array like this:

	while (counter < len(array))
	
NumberOfCars = len(Cars)