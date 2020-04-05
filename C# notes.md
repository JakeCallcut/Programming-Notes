# Programming in C#
***

# Fundamentals

> C# is a fairly high level, object-oriented programming language which is part of the C programming languages, these were developed by microsoft.

> C# was based on C++ and Java

## Running a program
> C# runs from a terminal which can be typed into, and outputted from. to run a program you must input the following command,

    dotnet run

## Basic Syntax

>In C#, every line must end with a semi-colon (;)

>Comments in C# are done as follows,

    //this is a single line comment
    
    /* 
    this is a 
    multi-line comment 
    */

## Input and Output
 in C# output is done using the code: 
    
    Console.WriteLine("text to output");

to output a variable use:

    Console.WriteLine(variable);

***

to get input from the user, you must use the following code

    string name = Console.ReadLine();

in this case "name" is the name of the variable, and the variable type is string.

If you need to have a question before the input, simply put a output statement before.

    Console.WriteLine("Please enter your name")
    Console.ReadLine()

***

## Variables
### Data Types

>C# has the same data types as most other mainstream programming languages.

here is a list of the basic ones and briefly what they store:

    int - whole numbers
    double - decimal numbers
    char - single characters 
    string - a string of characters
    bool - stores true or false

 to declare a variable, you must use the following code:

    int age = 25;

the syntax here is using, the data type followed by the variable name and assigning it a value.

when declaring a string or a char, you must use quotation marks or speech marks e.g:

    char FaveLetter = 'X';
    string Name = "James";

>N.B Though not essential, it is common practice to use quotation marks for characters and speach marks for a string, as above.

you can create a variable, without assigning it a value or with assigning it a value:

    int age;
    string name = "James";

### Converting Data Types

In programming there are two types of variable conversion, implicit and explicit:

> Implicit conversion is when no data is lost in the conversion, this means you can convert an integer to a double but not the other way around.

    e.g
    int MyInt = MyDouble   //this code will not work

    double MyDouble = MyInt   //this code will work

> Explicit conversion is where data is lost in the conversion. for example, converting a double to an integer. this has to be done using an operator.

    e.g
    int MyInt = Convert.ToInt(MyDouble)

We must convert variables very often because:
    
    Console.Readline()

Will always return a string. so if we want an integer input we have to do the following:

    int Input = Convert.ToInt32(Console.ReadLine());


