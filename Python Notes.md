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

now.month			#this will only output the current month
now.year 			#this will only output the current year
now.day				#this will only output the current day


from datetime import datetime
now = datetime.now()
print '%02d/%02d/%04d %02d:%02d:%02d' % (now.month, now.day, now.year, now.hour, now.minute, now.second)

						#this slice of code will print the date and time in a nicer format


SUBSTRINGS

example = "this is how to make a substring"
substring = example[0:10]							#the first number is the start of the substring and the last is the last
Print(substring)									#this will print "this is how"

#also, if you leave the character last character blank, the subtring will continue until the end of the string
substring = example[21:]
Print(substring)							#this will print "substring"


ARRAYS #("Python Lists" in Python)

Cars = ["volvo", "ford", "peugeot"]
FavNumbers = [24, 64, 2]

Cars[3] = "nissan"
FirstCar = Cars[0]

NumberOfCars = len(Cars)