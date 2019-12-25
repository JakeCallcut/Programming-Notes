#include<iostream>
#include<string> 
#include<vector>
#include<fstream>

using namespace std;

int main()

{

//this is how to comment [comments will only show in scripts]


/*
this is 
a multi-line comment
*/




EXTREME BASICS

// C++ knows when a statement has ended with a semi colon

// return 0; will ensure the action has ben carried out properly

// if you go beyond variable boundaries the variable will become negetive

// B I D M A S occurs








OUTPUT

	cout<< “this is how to print a message on screen”;

	cout<< x;                // this will print the value of x on screen

	cout<< "i am" << age << "years old";             //this will say " i am [value of age] years old

	cout<< "to insert a break\n";
	cout<< "just put slash n in the speech marks";

	cout<< "alternatively" << endl;
	cout<< " you can use endl" 

return 0;





VARIABLES

// if you want a variable to never be changed use "const" [constant] ie

const double "PI" = 3.14

/*
double [numbers to 15 decimal places]
char [single character][1 byte]
bool [true,1][false,0]
int [whole numbers]
float [numbers to 6 decimal places]
string [multiple words][size depends]
*/


// variables can be different sizes[in bytes]

// the lagest int possible is 2147483647

// if you want to find the size of a variable use the following command

cout<< sizeof(name of variable); 

return 0;





OPERATORS

/*
arithmetic operaters [maths signs]
*, multiply 
/, division
+, plus
-, minus
*/



/*
relational operators 
==, equal to
!=, not equal to
<, less than
>, greater than
<=,less than or equal to
>=,greater than or equal to
*/



/*
logical operators
&&, and
||, not
!, not
*/



/*
||, if the left-hand side expression is true, 
the combined result is true 
[the right-hand side expression is never evaluated].
*/



/*
&&, if the left-hand side expression is false, 
the combined result is false 
[the right-hand side expression is never evaluated].
*/




MATHS

// C++ will round to the nearest integer 

// to stop this use the desired variable in the sum ie 

	cout<< "4/5="<<(double) 4/5<<




	
	
	
STRINGS

// a string is a way of asigning multiple words to a variable

	string mystr;
	cout<< "whats your name?\n"

	getline (cin,mystr)
	cout<< "hello"<< mystr << "\n"
	
	return 0;

	
	
	
	
	
	
	
	
	
	
	
IF/ELSE


//lets say ie

int age = 37

bool isintoxicated = true



if((age>=1) && (age<17){  	// these are nested brackets and you must close them

	cout<< "you cant drive";


} else if (! isintoxicated)

	cout<< "you cant drive";

return 0;



	int x = 100
	
if (x==100)
	cout<< "x is 100";
else
	cout<< "x is not 100"





WHILE LOOPS


	int n = 100
	
while (n = 100)	 {
	
	cout<< "this is a way to make a forever loop"
	
	
}
	




















SWITCH STATEMENT
 
int greeting=2;

switch(greeting){

case 1:				// you can have as many cases as you want
	cout<<"bonjour";
break;

case 2:
	cout<<"hola";
break;

default:			// you can only have one default
	cout<<"hello";}




INPUT


int age
	cin>> age;		//they input age

	return 0;
	
	
int name 
	cout<< "whats your name";
	cin>> name;						// they input thier name
	cout<< name << "thats a nice name"
	
	

// to input strings 
	
	getline (cin,[your string])
	
	return 0;
	
	

	
	
	
	ARRAYS

// arrays are a way of storing mulitiple of the same data type

	int favnums[3] = {5,25,64} 		//25 would be given the value favnums[1]
	
	cout<< "favourite number 1:"<< favnums[0]

}
	

	