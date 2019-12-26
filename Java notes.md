# JAVA NOTES
***
	
## Fundamentals
Java programs Have at least 
one class(a real world idea) 
and one "Main()" method (this runs tasks of the program)
	
## Basic Syntax	
semi-colons are used to end a statement like so

	Systems.out.println("hello world");	

this is the syntax to print something  

### Comments	
	//this is a single line comment

	/*
	this is a multiline comment
	*/		
## Compiling
in the console, to compile a file we use the command 

	javac FileName.java

we run the executable with the command 

	java FilName

#### Example of Compiling
	
	public class Welcome {
		public static void main(String[] args) {
			System.out.print("Welcome");
		}
	}
	
if we successfully compile this program, we will have two files 

- welcome.java - our original file with java 

- welcome.class - a compiled file ready to be run by the java virtual machine			
			
			
## Variables
to declare a variable use the data type followed by the name like so:
			
	int age;
			
you can also declare a variable and assign a value in one line like so:

	int age = 25;
			
note: do no use quotation marks when ourputting a variable like so

	System.out.println(age)
			
			
### Data Types
				
- int - whole numbers between -2,147,483,648 and 2,147,483,647, inclusive.
				
- double - 1.797,693,134,862,315,7 E+308, which is approximately 17 followed by 307 zeros. The minimum value is 4.9 E-324, which is 324 decimal places!
				
- boolean - true or false
				
- char - any character, like a letter, space, or punctuation mark.
				
- String - sequences of characters. 
				
			
### Variable Checking
you can compare two variables by using certain syntax like so:

	boolean isOldEnough(age>ageNeeded);
				
					
					
## Concatenation
				
use + like so:

	 System.out.println("your username is: " + username);

you can also use other variable types like integers:

	System.out.println("Your balance is" + balance)
				
			
				
## Classes
the fundamental concept of object oriented peorgramming is in classes:

a class is like an object constructor or blueprint for creating objects, it contains the states and behaviors of all of its objects

it is created using this syntax:
	
	public class ClassName {
  		int x = 5;
	}

This means that any object with the class "ClassName" will *know* the variable 'x'

### Constructors

## Objects
Objects are things that we can control using our program some examples are dogs, doors and cars.

all of these have:
- states:
such as color, brand or breed
- behaviors
such as opening, closing and driving

creating an object is done using the following syntax:

	public class car {
	   public car(String brand) {
	   System.out.println("the cars brand is: " + brand);
	   }

	   public static void main(String []args) {
		car toyota = new car("toyota");
	   }
	}

this will output "the cars brand is toyota"
## Methods





				
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			