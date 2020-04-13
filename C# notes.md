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

## Working with Numbers
### Decimal Numbers

> when using a decimal, there are *decimals*, *floats* and *doubles*.

a *double* is usually the best to use for general application, as it is more precise than a *float* but is faster to proccess than a *decimal*, for financial applications one should use a *decimal*, as it is the most precise.

    decimal return = 43800.56m;

you have to use an m after the number so that C# knows we are defining a *decimal*.

### Incrementing and Decrementing

> Incrementing and decrementing a number means adding a certain amount to a number.

there are some shortcuts to increment and decrement in C#:

If you want to increment or decrement by one you can use -- or ++, like so:

    MyNumber++;
    MyNumber--;

if you want to incrememt or decrement by a number other than one like so:

    Increment by three
    MyNumber+=3;

    Decrement by three
    MyNumber-=3;

### Advanced Mathmatical Operations

Some more complex operations such as square root are not represented in C# by characters, so we must use function dot notation.

these are a few,

    Math.Abs(Number) - returns the distance from 0
    Math.Sqrt(Number) - returns the square root of a number
    Math.Floor(Number) - truncates the number to an integer
    Math.Min(Number) - returns the smaller of the two numbers
    Math.Max(Number) - returns the greater of the two numbers    
    Math.Pow(Number) - 

Math.Min() has some different syntax like so:

    Math.Min(15,8);
    This will return 8

> N.B Math.Sqrt() cannot take a negative number as input, this can be circumvented by using Math.Abs() inside Math.Sqrt() like so:

    Math.Sqrt(Math.Abs(-1337));
    this will return the positive solution for the square root of -1337

#### Math.Pow( ):

>Math.Pow( ) is a built-in method which you can use for raising a number to an exponent, the method has two parameters.

the first is the number which you want to raise to the power of the exponent, which is the second parameter. e.g

    Math.Pow(2, 3);
    this will return 8, (2^3)

#### Math.Ceiling( ):

>Math.Ceiling( ) rounds the decimal number UP to the nearest whole number no matter the decimal value. e.g

    Math.Ceiling(7.13);
    will return 8

## Working With Text

### Escape Character

Lets say you want to put speech marks within a string, doing this wont work:

    Console.WriteLine("this is a speech mark " ")

Because the second speech mark will end the string, then you have an open speech mark and everything gets confusing.

so we must uses an escape character, in C# this is backslash "\" e.g:

    String sentence = "Perhaps the most famous latin phrase: \"Veni, Vidi, Vici\"";

    Console.WriteLine(sentence);

this will return:

Perhaps the most famous latin phrase: "Veni, Vidi, Vici"

### Line Break

Lets say that you want to output two statements to the Console, but on different lines:

    Like

    This

to do this we simply use the line of code:

    Console.WriteLine("\n")

this will create a line break.

### Concatenation and interpolation
****
#### concatenation
concatenation is the joining of two strings, in C# this can be done with a "+" like so:

    String firstWord = "veni "
    String secondWord = "vidi "
    String thirdWord = "vici "

    string phrase = firstWord + secondWord + thirdWord
    Console.WriteLine(phrase)

this will return "veni vidi vici"

#### Interpolation
An alternative to concatenation is interpolation, this is where one can insert variables seamlessly into a string e.g

    string phrase = "veni, vidi, vici"

    Console.WriteLine($"Perhaps the most famous latin phrase: {phrase});

in this code, the dollar sign ($) tells C# that we are going to be using interpolation in this string.

then, any variable that you want to insert you must put in {braces}.











