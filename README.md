C Programming
	A High Level Programming Language (which uses alphabets, digits, punctuations and some special symbols and cannot be executed directly without being converted into machine level language (the language which uses only 0 and 1))

	developed by a man named Dennis Ritchie

 


	in 1970s at Bell Telephone laboratories (now named AT & T Bell laboratories), Murray Hill, New Jersey

	to develop the UNIX operating system.

	using the two early programming languages -- Basic Combined Programming Language (BCPL) and BASIC (Beginner's All-purpose Symbolic Instruction Code) language

	Uses: used in the development of  a) operating systems like LINUX, UNIX  b) embedded systems like ATMs, printers.Most of the state-of-the-art software have been developed using C.

	Advantages: relatively simple language, reliable (able to be trusted), easy to understand, easy to use, write, modify and debug and quick to learn. 

	MYSQLDatabase, LINUX Drivers, Text Editors are written in C.

	C is called a structured programming language because it divides the problem into smaller modules called functions or procedures each of which handles a particular responsibility. Hence it is simple and easy to understand and well sited for small size implementation. However this is not restricted. A large size implementation is possible but complex design and full object oriented design cannot be implemented (because complex design concepts like Polymorphism and inheritance are not available in C).

	A Simple C program basically comprises of the following parts:
•	Preprocessor Commands
•	Functions
•	Variables
•	Statements & Expressions
•	Comments
// -------------------------------------------------------------------------------------

/* My First C Program  */   Comment

#include<stdio.h> // preprocessor command
int main() // Function where the program execution begins.
{
printf("Hello,world!"); // statement
return 0;
}

-------------------------------------------------------------------------------------  //


	Process of C Program Execution: A C program:

#include<stdio.h>
int main()
{
printf("Hello,world!");
return 0;
}

is written using Text Editor , such as [ Notepad (in case of Windows Operating System), vim or vi (in case of Linux Operating System)] and saved with [.C] Extension. 
File Saved with [.C] extension is called Source Program or Source Code. 
C Source code with [.C] Extension is sent to preprocessor first. 
The preprocessor generates an expanded source code:

// ----------------------------------------------------------------------------------------------------------

The contents of <stdio.h> would be pasted at the location of #include<stdio.h>
int main()
{
printf("Hello,world!");
return 0;
}

------------------------------------------------------------------------------------------------------  //

	Expanded source code is given as input to compiler where the expanded source program is compiled (i.e., the program is entirely read and translated to instructions the computer can understand i.e., machine understandable / readable language i.e., to machine code sequence of 0s and 1s). If the C compiler finds any error during compilation, it provides information about the error to the programmer. 

	The programmer has to review code and re-edit the program. After re-editing program, Compiler again check for any error. 

	If program is error-free then it is sent to assembler (where the code is assembled and converted into object code. Now a simple.obj file is generated). 

	The object code is sent to linker (where the object code is linked with appropriate libraries). Then it is converted into a single executable code. A simple.exe file is generated.

	The executable code is sent to loader (where the executable code is loaded into memory and then it is executed). 

	After execution, output: 
Hello,world!
is displayed on the console screen.


C is case sensitive language: only lower case letters (or small letters) must be used.  

Capital letters (or upper case letters) must be avoided to prevent the display of error on the screen 
(For example: If the statement PRINTF("Hello,world!"); is written instead of printf("Hello,world!"); 
or INT MAIN() is written instead of int main(), compilation Error will be displayed on the console screen). 

Parentheses () indicate a function and the word main indicate the name of the function.
main() implies: main function 

And if we forget to end each statement within the body of the main function with a semicolon (;), then the compilation Error will be displayed on the screen. 

There should be no space between main and the parentheses ()

i.e., int main() 

and there should be no space inside the parentheses ()

i.e., int main() 

to prevent the display of compilation error on the screen.

As we know C is Platform dependent language. So the Operating system needs to know when the program execution ends. 

So when there is value returns from the main function
the Operating System get to know that the program execution is over.
int main () implies: main() should return integer value.

	If the main function returns 0 to the operating system, then the  
program has completed execution successfully.

	If the main function returns 1 to the operating system, then the  
program has not completed execution successfully.

The statement 
#include<stdio.h>
tells the compiler to include the text from the file stdio.h (which is already present in the operating system) before it translates or compiles the program into a sequence of 0s and 1s. 

	stdio means standard input output and stdio.h means standard input output header file (printf() & scanf() are not part of the C language, because there is no input or output defined in C language itself-- stdio.h comprises standard input output functions like scanf, printf etc. 
	and allows standard input /output operations -- note: scanf is an input function and printf is an output function (note: Letter f denote formatted) and it is included into the C program by writing the statement #include <stdio.h>).
	If a program is written without the statement:
#include<stdio.h>, then the C compiler can't compile and a compilation error is displayed on the screen (because C compiler fails to recognize the functions such as printf() and scanf()).


	Note: We can also write #include "stdio.h" instead of #include <stdio.h> but some online compilers will flag error message. So the statement #include <stdio.h> is generally preferred and the statement #include "stdio.h" is generally ignored.


main() →  The program begins its execution with the function main() -- which is called the user defined function (because this function is defined by the user) - the main function -- the entry point of the program execution i.e., the point from where the execution of C program begins and the point at which the operating system passes control of  the computer over to that program.

int main() {
} → implies body of the main function within which the sequence of instructions in the form of statements 
i.e., the program  is written and executed. The left curly brace 
{ 
implies: the beginning of the main function 
and the right curly brace 
}
implies: the end of the main function.

return 0; → implies the exit status of execution of the program i.e., at this point, 
main function returns back the control of the computer to the operating system since 
the execution is terminated at this point and once a return statement 
i.e., return 0; is executed, no further instructions within the main function are executed

For example:

#include<stdio.h>
int main()
{
printf("Hello,world!");
return 0;
printf("Hello,world!");
}

Output on the screen:
Hello,world!

; → implies semicolon or statement terminator → A program is a well-defined set of instructions and each well-defined instruction (in the form of a statement) is ended by a semicolon (which is C language punctuation -- like a period in English i.e., in an English paragraph each sentence is ended by a full stop which tells that one sentence ends and another begins, semicolon implies the end of one logical entity -- that one instruction (or statement) ends and another begins).

printf()→ output function of the C language which makes provision to print the output:

Hello,world!
															
on the screen. Parentheses () indicate a function and the word printf indicate the name of the function. 

The text 
Hello,world!
should be enclosed by the double quotation marks ("") and should be written within the printf function and this 
printf function should be ended with the semicolon i.e., 
printf("Hello,world!");
otherwise the compilation error will be displayed on the screen. 


Program 1.1

C program to print the word "hello Bill Gates" on screen

#include<stdio.h>
int main()
{
printf("hello Bill Gates");
return 0;
}
The output on the screen:
hello Bill Gates

Program 1.2

C program to print 
*
*****
*****
*****
*****
on screen

#include<stdio.h>
int main()
{
printf("\n     *     ");
printf("\n  ***** ");
printf("\n  ***** ");
printf("\n  ***** ");
printf("\n  ***** ");
return 0;
}

The output on the screen:
*
*****
*****
*****
*****
If new line sequence (\n)  is not included in the above program then the output on the screen is:

*********************
In the above code, the new line character has the ASCII value of 10 which means it is a new line. The author has put the ASCII values table for different characters that can be used in the programs to solve real time problems.

	Write a program to print the following outputs:

(a)	

*
****
*******
****
*
(b)

****************
* *
* Hello World! *
* *
****************

(c)

Braces come in pairs!
Comments come in pairs!
All statements end with a semicolon!
Spaces are optional!
Must have a main function!
C is done mostly in lowercase. It's a case-sensitive language

Answers:

(a)

#include<stdio.h>
int main()
{
printf("\n           *     ");
printf("\n        ****  ");
printf("\n      ******* ");
printf("\n        ****    ");
printf("\n           *      ");
return 0;
}

(b)

#include<stdio.h>
int main()
{
printf("\n           ****************         ");
printf("\n                      * *                       ");
printf("\n           * Hello World! *           ");    
printf("\n                      * *                       ");
printf("\n           ****************         ");
return 0;
}

(c)

#include<stdio.h>
int main()
{
printf("\n Braces come in pairs!");
printf("\n Comments come in pairs!");
printf("\n  All statements end with a semicolon!");
printf("\n  Spaces are optional!");
printf("\n Must have a main function!");
printf("\n C is done mostly in lowercase. It's a case-sensitive language");
return 0;
}

Program 1.3

C program to find the area of a circle 

#include<stdio.h>
int main()
{
int r, area;
r = 2;
area = 4 * 3.14 * r * r;
printf("The area of the circle = %d", area);
return 0;
}

The output on the screen:
The area of the circle = 50

int means the data type (an attribute that tells what kind of data that value can own) is integer and the storage size of int data type is 2 or 4 or 8 byte.
Note:
•	A string, for example, is a data type that is used to categorize text and an integer is a data type used to categorize whole numbers / non fractional values.
•	We can't store decimal values using int data type.
•	If we use int data type to store decimal values, decimal values will be shortened and we will get only whole number. In this case, float data type can be used to store decimal values in a variable.

The statement 
int r, area;
imply that we are creating the integer variables r , area. 
Equal sign (" = ") implies storage operator.

The statements 
r = 2;
area = 4 * 3.14 * r * r;
imply that we are storing the values to the created variables (i.e., we are storing the value 2 for r 
and 4 * 3.14 * r * r = 4 * 3.14 * 2 * 2 = 50 for area).

Comma in the statement 
int r, area;
imply variable separator.

The statement 
printf("The area of the circle = %d", area);
make provision to print the output:
The area of the circle = 50
on the screen.

In the statement 
printf("The area of the circle = %d", area);
format string or format specifier %d indicates that the integer value to be displayed after the statement 
The area of the circle =
enclosed by double quotes needs to be taken from a variable area.

The area of the circle is 50. 24 (for r = 2) but The area of the circle = 50 is displayed on the screen 
because data type int is used instead of float and format specifier %d is used instead of %f.

If float r, area; is used instead of int r, area;
and
If the statement
printf("The area of the circle = %f", area);
is written instead of 
printf("The area of the circle = %d", area);
i.e., 

#include<stdio.h>
int main()
{
float r, area;
r = 2;
area = 4 * 3.14 * r * r;
printf("The area of the circle = %f", area);
return 0;
}

Then the output on the screen:
The area of the circle = 50.24

float means the data type is float.

The statement 
float r, area;
imply that we are creating the floating variables r, area.

(floating point variable means fractional variable or decimal number (for example: 1.5, 2.5, 3.5, 4.7 … etc.) whereas integer means non-fractional variable or whole number (for example: 1, 2, 3, 4 … etc.))

data type float is used instead of int (and format string %f is used instead of %d) because if the data type int is used instead of float then the result will not be clearly outputted i.e., instead of 50.24 the computer displays only 50.

If the statement 
printf("The area of the circle = %2f", area);
is written instead of the statement 
printf("The area of the circle = %f", area);
Then the output on the screen is:
The area of the circle =             50.24
i.e., the statement 

printf("The area of the circle = %f", area); yields the output:

The area of the circle = 50.24
whereas the statement 
printf("The area of the circle = %2f", area); yields the output:

The area of the circle =              50.24

If you want to supply the value for r through the key board, then the statement

r =2;
should be replaced by the statements
printf("Enter any number:");
scanf("%d", &r);

i.e., the program should be rewritten as: 

#include<stdio.h>
int main()
{
float r, area;
printf("Enter any number:");
scanf("%d", &r);
area = 4 * 3.14 * r * r;
printf("The area of the circle = %f", area);
return 0;
}

The output on the screen:

Enter any number:
If you enter the number 2
The area of the circle = 50.24 will be outputted on the screen.

The statement 
float r, area;
imply that we are creating the float variables r and area and these variables are stored in the computer memory and they are assigned an address to locate their position in the computer memory (like houses in a street are assigned an address to locate their position in the street). 

The statement 
printf("Enter any number:");
make provision to print the text 
Enter any number:
on the screen.

The statement 
scanf("%d", &r);
make provision to enter a number for r through the keyboard and store the number entered for r through the keyboard in the address of r in the computer memory. & symbol imply the address and &r imply the address of r in the computer memory. 

Format string %d in the statement scanf("%d", &r); tells the input function scanf to read the number entered through the keyboard (which is a integer) and since "%d" is followed by , &r  ---  %d tells the scanf function to read the integer entered through the keyboard for r  and store it in the address of r in the computer memory (i.e., store the number in &r).

	Note: 
As told earlier: when you enter an integer for r through the keyboard, this integer will be stored in the computer memory. If you want to know the storage size of the integer  in computer memory (i.e., space occupied by the entered integer in the computer memory), you need to appeal to the following program:

#include <stdio.h>
int main()
{
int r;
r=10;
printf("size of r = %d", sizeof(r));
return 0;
}

The output on the screen:
size of r = 4
													
i.e., integer entered for r i.e., 10 has occupied a space of 4 bytes in the computer memory.

	Write a program to print the circumference of the circle (given r = 2.5)

Answer:

#include<stdio.h>
int main()
{
float r, area;
r = 2.5;
circumference = 3.14 * r * r;
printf("The circumference of the circle = %f", circumference);
return 0;
}

	Write a program to print the area of the rectangle (given l = 2.5 and b = 3)

Answer:

#include<stdio.h>
int main()
{
float l, b, area;
l = 2.5;
b = 3;
area = 1*b;
printf("The area of the rectangle = %f", area);
return 0;
}


Format Specifiers in C 

Data Type	Format Specifier
int	%d
float	%f or %e
char	%c
double	%lf or %le
long int	%ld

Program 1.3
C program to find the sum of two numbers

#include<stdio.h>
int main()
{
int a, b, sum;
a=1;
b=2;
sum = a + b;
printf("the sum of a and b = %d", sum);
return 0;
}

The output on the screen:
the sum of a and b = 3

If you want to assign the floating point values i.e., fractional numbers for a & b (i.e., 1.5 for a &  2.6 for b) through the keyboard, 
then the statement 
int a, b, sum;
should be replaced by the statement 
float a, b, sum;
and the statement 
printf("the sum of a and b = %d", sum); should be replaced by the statement

printf("the sum of a and b = %f", sum);
i.e.,

#include<stdio.h>
int main()
{
float a, b, sum;
a=1.5;
b=2.6;
sum = a + b;
printf("the sum of a and b = %f", sum);
return 0;
}
The output on the screen:
the sum of a and b = 4.1
The statement 
printf("the sum of a and b = %f", sum);
make provision to print the output:
the sum of a and b = 4.1
In the statement 
printf("the sum of a and b = %f", sum);
	
format string %f tells the printf function to print a floating point value which is sum.
Since a = 1.5 and b = 2.6 therefore: 

the sum of a and b = 1.5 + 2.6 = 4.1 which is outputted on the screen.

If the statement
printf("the sum of a and b = %f", sum);
is replaced by the statement 
printf("the sum of a and b = %f, sum");
Then output on the screen is:
the sum of a and b = %f, sum

And if the statement printf("the sum of a and b = %f", sum); is omitted from the C program, 
then the program will be successfully executed but there will be no display of the output on the screen.

If you want to supply the values for a and b through the key board, then the statements

a=1.5;
b=2.6;

should be replaced by the statements

printf("Enter any two numbers:");
scanf("%f %f", &a, &b);

i.e., the program should be rewritten as:

#include<stdio.h>
int main()
{
float a, b, sum;
printf("Enter any two numbers:");
scanf("%f %f", &a, &b);
sum = a+ b;
printf("the sum of a and b = %f", sum);
return 0;
}

The output on the screen:
Enter any two numbers:
If you enter two numbers 2.9 & 3.6
the sum of a and b = 6.5 will be outputted on the screen with trailing zero’s to fill up memory.

	As Said Earlier:

ampersand ("&") imply the address and &a and &b imply the addresses of the created float variables a and b stored in the computer memory  i.e., when we enter a number for a and b through the keyboard, these numbers are read by scanf() function and they are stored in the computer memory (i.e., the number entered for a is stored in the address of a (i.e., stored in &a)  and the number entered for b is stored in the address of b (i.e., stored in &b)).

There are 2 format strings in the statement 
scanf("%f %f", &a, &b);
	one format string %f corresponds to &a i.e., %f tells the scanf() function to read the number entered through the keyboard for a and store it  in the address of a in the computer memory.
	and the other format string %f corresponds to &b i.e., %f tells the scanf() function to read the number entered through the keyboard for b and store it in the address of b in the computer memory.

If the two format strings are separated by a comma i.e.,
scanf("%f, %f", &a, &b);
Then the compilation error will be displayed on the screen.

	Note:

The statement printf("Enter any two numbers:"); make provision to print 
Enter any two numbers:
on the screen and the statement scanf("%f %f", &a, &b); read the two numbers 2.9 and 3.6 entered through the keyboard and store them in the computer memory.

If the statements 

printf("Enter any two numbers:");
scanf("%f %f", &a, &b);

are replaced by the statements:

printf("Enter any number:");
scanf("%f", &a);
printf("Enter any number:");
scanf("%f", &b);

i.e.,

#include<stdio.h>
int main()
{
float a, b, sum;
printf("Enter any number:");
scanf("%f", &a);
printf("Enter any number:");
scanf("%f", &b);
sum = a+ b;
printf("the sum of a and b = %f", sum);
return 0;
}

Then the output on the screen:

Enter any number:
If you enter a number 2.9 
Enter any number:
If you enter a number 3.6 
the sum of a and b = 6.5 will be outputted on the screen.

If the statement 
printf("the sum of a and b = %f", sum);
is replaced by the statement 
printf("the sum of %f and %f = %f", a, b, sum);
Then the output on the screen is:
the sum of 2.9 and 3.6 = 6.5

In the statement 
printf("the sum of %f and %f = %f", a, b, sum);
there are three format strings:
	The format string %f after the statement (the sum of) indicates that the value to be displayed needs to be taken from a variable a.
	The format string %f after the statement (the sum of %f and) indicates that the value to be displayed needs to be taken from a variable b.
	The format string %f after the statement (the sum of %f and %f = ) indicates that the value to be displayed needs to be taken from a variable sum.
Program 1.4
C program to convert the temperature in Celsius to Fahrenheit

#include<stdio.h>
int main()
{
float C, F;
C=38.5;
F = 9*C/5 +32;
printf("temperature in Fahrenheit= %f", F);
return 0;
}

The output on the screen:
temperature in Fahrenheit= 101.3

	Note: If x is used instead of * and F = 9C/5 +32 is used of F = 9*C/5 +32, then the compilation error will be displayed on the screen.

If you want to supply a number 16 digits after decimal point i.e., 36.5555555555555555 for C, then the statement 

double C, F; should be used instead of the statement float C, F;

and %lf should be used instead of %f

i.e.,

#include<stdio.h>
int main()
{
double C, F;
C=38.5555555555555555;
F = 9*C/5 +32;
printf("temperature in Fahrenheit= %lf", F);
return 0;
}

And if you want to supply the number 16 digits after decimal point for C through the key board, then the statement
C = 38.5;
should be replaced by the statements:

printf("Enter any number:");
scanf("%lf", &C);

i.e.,
#include<stdio.h>
int main()
{
double C, F;
printf("Enter any number:");
scanf("%lf", &C);
F = 9*C/5 +32;
printf("temperature in Fahrenheit= %lf", F);
return 0;
}
	Note:

#include <stdio.h>
int main()
{
double C, F;
C = 25.3333333333333333;
F = 9*C/5 +32;
printf("temperature in Fahrenheit= %lf", F);
}

The output on the screen:
temperature in Fahrenheit = 77.600000

If the statement double C, F; is replaced by the statements 

double C;
float F;

i.e., if the above program is rewritten as:

#include <stdio.h>
int main()
{
double C;
float F;
C = 25.3333333333333333;
F = 9*C/5 +32;
printf("temperature in Fahrenheit= %f", F); // %f is used because the data type for F is float
return 0;
}
Then there is slight change in the output on the screen:
temperature in Fahrenheit = 77.599998

												
	Write a program to print the sum of three numbers

Answer:

#include<stdio.h>
int main()
{
int a, b, c, sum;
printf("Enter any three numbers:");
scanf("%d %d%d", &a, &b, &c);
sum = a + b + c;
printf("the sum of a, b and c = %d", sum);
return 0;
}

	Write a program to print the Equivalent hexadecimal value of an integer

Answer:

#include<stdio.h>
int main()
{
int a = 45;
printf("%x", a);
return 0;
}

Output on the screen:
2d

	Write a program to print the area of a triangle, given 
area = (s (s-a) (s-b) (s-c))1/2 where s = (a + b + c) / 2 

Answer:

#include<stdio.h>
#include<math.h>
int main()
{
int a, b, c, s, area;
a = 3;
b= 4;
c=5;
s = (a + b + c) / 2;
area = sqrt ((s * (s-a) * (s-b) * (s-c));
printf("the area of the triangle = %d", area);
return 0;
}

	Note: since sqrt() is not part of C language or of standard input output file i.e., (stdio.h file), it is part of math file i.e., (math.h file which defines various mathematical functions) the statement #include<math.h> should be included in the C program otherwise the compilation error will be flagged on the screen stating that sqrt() is not declared or defined.

	Note: If the statement  area = (s (s-a) (s-b) (s-c)) 1/2   is written instead of 
area = sqrt ((s * (s-a) * (s-b) * (s-c));
Then the compilation error will be displayed on the screen because C does not support 
area = (s (s-a) (s-b) (s-c)) 1/2 .

	Stuff you need to know about:

	1 kilobyte = 1024 bytes
	1 megabyte = 1024 × 1024  bytes
	1 gigabyte = 1024 × 1024 × 1024  bytes

Program 1.5

C program to find the product of two numbers

#include<stdio.h>
int main()
{
int a, b, product;
a=1;
b=2;
product = a * b;
printf("the product of a and b = %d", product);
return 0;
}

The output on the screen:
the product of a and b = 2

If you want to insert a 10 digit number for a and b i.e.,

a=1000000000
b=3000000000, then the statement: 
int a, b, product; should be replaced by the statement long int a, b, product;
and %ld should be used instead of %d 

i.e., the program should be rewritten as:

#include<stdio.h>
int main()
{
long int a, b, product;
a=1000000000;
b=2000000000;
product = a * b;
printf("the product of a and b = %ld", product);
return 0;
}

The output on the screen:
the product of a and b = 3000000000000000000

If you want to supply the values for a and b through the key board, then the statements 
a=1;
b=2;  should be replaced by the statements
printf("Enter any two numbers:");
scanf("%d %d", &a, &b);

i.e.,

#include<stdio.h>
int main()
{
int a, b, product;
printf("Enter any two numbers:");
scanf("%d%d", &a, &b);
product = a* b;
printf("the product of a and b = %d", product);
return 0;
}

The output on the screen:
Enter any two numbers:
If you enter two numbers 1 and 3
the product of a and b = 3 will be outputted on the screen.

If you replace the statements 
printf("Enter any two numbers:");
scanf("%d%d", &a, &b);

by the statements 
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);

Then the output on the screen will be:

Enter any number:
If you enter the number 3
Enter any number:
If you enter the number 3
the product of a and b = 9
will be outputted on the screen.
If the statement 
printf("the product of a and b = %d"; product);
is written instead of the statement
printf("the product of a and b = %d", product);
i.e., instead of variable separator (i.e., comma) semicolon is used -- Then the compilation error will be displayed on the screen.

	Note: 

#include <stdio.h>
int main()
{
printf("Hello, World!");
printf("Hello, World!\b");
printf("Hello, World!\b");
printf("Hello, World!\b");
return 0;
}
i.e., if  back space \b is used then 
Hello, World!Hello, World!Hello, World!Hello, World!
will be outputted on the screen.

If carriage return \r is used instead of \b 
i.e.,

#include <stdio.h>
int main()
{
printf("Hello, World!");
printf("Hello, World!\r");
printf("Hello, World!\r");
printf("Hello, World!\r");
return 0;
}

The output on the screen is:
Hello, World!Hello, World!
Hello, World!
Hello, World!

If Horizontal tab \t is used instead of \r
i.e.,
#include <stdio.h>
int main()
{
printf("Hello, World!\t");
printf("Hello, World!\t");
printf("Hello, World!\t");
printf("Hello, World!\t");
return 0;
}

The output on the screen is:

Hello, World!	Hello, World!	Hello, World!	Hello, World!


If vertical tab \v is used instead of \t
i.e.,
#include <stdio.h>
int main()
{
printf("Hello, World!\v");
printf("Hello, World!\v");
printf("Hello, World!\v");
printf("Hello, World!\v");
return 0;
}

The output on the screen is:
Hello, World!                                                                                                              
Hello, World!                                                                                                 
Hello, World!                                                                                    
Hello, World!

Program 1.5
C program to find the square of a number

#include<stdio.h>
int main()
{
int a, b;
a=2;
b = a * a;
printf("the square of a = %d", b);
}

The output on the screen:
the square of a = 4

If the statement b = a * a; is replaced by b = pow((a), 2);
i.e., if the above program is rewritten as:
#include<stdio.h>
#include<math.h>
int main()
{
int a, b;
a=2;
b = pow((a), 2);
printf("the square of a = %d", b);
return 0;
}

Then there will be no display of compilation error on the screen or there will be no change in the output on the screen i.e.,
the square of a = 4 will be outputted on the screen.
which means:
b = pow((a), 2); is the same as b = a*a;
Since b = pow((a), 2); is used instead of  b = a*a;
#include<math.h> should be included in the C program as b = pow((a), 2); is supported by #include<math.h>
Otherwise compilation Error will be displayed on the screen.

If you want to supply the integer value for a through the key board, then the statement
a=2; is replaced by the statements
printf("Enter any number:");
scanf("%d", &a);
i.e.,
#include<stdio.h>
int main()
{
int a, b;
printf("Enter any number:");
scanf("%d", &a);
b = a * a;
printf("the square of a = %d", b);
return 0;
}

The output on the screen:

Enter any number:
If you enter a number 4
the square of a = 16 will be outputted on the screen. 

	Note: 
If scanf(%d, &a); is written instead of scanf("%d", &a);
If printf(the square of a = %d, b); is written instead of printf("the square of a = %d", b); 

If the main function is followed by a semicolon i.e.,
int main(); is written instead of int main()
Then the compilation error will be displayed on the screen.

But if the body of the main function is followed by a semicolon i.e.,
int main()
{
}; is written instead of 
int main()
{

}
There will be no display of the compilation error on the screen.
int main(); → ERROR
int main()
{
}; → NO ERROR


	Write a program to print the cube of a number 
Answer:

#include<stdio.h>
#include<math.h>
int main()
{
int a, b;
a=2;
b = pow((a), 3);
printf("the cube of a = %d", b);
return 0;
}

	Write a program to print the energy of the substance using energy = mc2

Answer:

#include<stdio.h>
#include<math.h>
int main()
{
int m;
long int c, energy;
m=2;
c = 300000000;
energy = m * pow((c), 2);
printf("the energy of the substance  = %ld joules", energy);
return 0;
}

Program 1.6

C program to find the greatest of two numbers using if - else statement

The syntax of if – else statement (Conditional Statements):

if (this condition is true)
{
print this statement;
}
else 
{
print this statement;
}


#include<stdio.h>
int main()
{
int a, b;
a = 2;
b = 3;
if(a>b)
{
printf("a is greater than b");
}
else
{
printf("b is greater than a");
}
return 0;
}

The output on the screen:
b is greater than a
													
Since the condition a>b within the parentheses is not true, the statement a is greater than b is not executed; 
instead the execution skips and pass to print the statement b is greater than a.

In simpler words,
(a>b) is the condition (i.e., logical expression that results in true or false) and
if the condition (a>b) is true, then the statement: 
{
printf("a is greater than b");
}
is executed to print the output:
a is greater than b
else the statement 
{
printf("b is greater than a");
}
is executed to print the output:
b is greater than a

If you want to supply the integer values for a and b through the key board, then the statements 

a=2;
b=3; should be replaced by the statements
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);

i.e., the program should be rewritten as:

#include<stdio.h>
int main()
{
int a, b;
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);
if(a>b)
{
printf("a is greater than b");
}
else
{
printf("b is greater than a");
}
return 0;
}

The output on the screen:

Enter any number:
If you enter the number 6
Enter any number:
If you enter the number 3
a is greater than b
will be outputted on the screen.

Program 1.7
C program to find the greatest of three numbers using if - else if - else statement

The syntax of if - else  if - else statement:

if (this condition is true)
{
print this statement;
}
else if (this condition is true)
{
print this statement;
}
else  
{
print this statement;
}


#include<stdio.h>
int main()
{
int a, b, c;
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);
printf("Enter any number:");
scanf("%d", &c);
if(a>b&&a>c)
{
printf("%d is greater than %d and %d", a, b, c);
}
else if (b>a&&b>c)
{
printf("%d is greater than %d and %d", b, a, c);
}
else 
{
printf("%d is greater than %d and %d", c, b, a);
}
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 2
Enter any number:
If you enter the number 3
Enter any number:
If you enter the number 4
4 is greater than 3 and 2
will be outputted on the screen.

double ampersand "&&" imply and. 
(a>b&&a>c)
(b>a&&b>c)
denote conditions. 
i.e., the condition
(a>b&&a>c) imply:
a is greater than b and a is greater than c
and if this condition is true, then the statement 
{
printf("a is greater than b and c");
}
is executed to print the output:
a is greater than b and c
and if the condition (a>b&&a>c) is not true 
the statement				
{
printf("a is greater than b and c");
}
is not executed; instead the execution skips and pass to the condition (b>a&&b>c) 
and if this condition is true, then the statement 
{
printf("b is greater than a and c");
}
is executed to print the output:
b is greater than a and c
and if the condition (b>a&&b>c) is not true, then the statement
{
printf("b is greater than a and c");
}
is not executed; instead the execution skips and the statement 
{
printf("c is greater than b and a");
}

is executed to print the output:
c is greater than b and a


If the statements: 

if(a>b&&a>c)
{
printf("%d is greater than %d and %d", a, b, c);
}
else if (b>a&&b>c)
{
printf("%d is greater than %d and %d", b, a, c);
}
else 
{
printf("%d is greater than %d and %d", c, b, a);
}

are replaced by the statements:


if(a>b&&a>c)
printf("%d is greater than %d and %d", a, b, c);
else if (b>a&&b>c)
printf("%d is greater than %d and %d", b, a, c);
else 
printf("%d is greater than %d and %d", c, b, a);


i.e., if the program is rewritten as:

#include<stdio.h>
int main()
{
int a, b, c;
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);
printf("Enter any number:");
scanf("%d", &c);
if(a>b&&a>c)
printf("%d is greater than %d and %d", a, b, c);
else if (b>a&&b>c)
printf("%d is greater than %d and %d", b, a, c);
else 
printf("%d is greater than %d and %d", c, b, a);
return 0;
}

There will be no display of error on the screen 
c is greater than b and a
will be successfully outputted on the screen


	What will be the output of the following program ?

#include <stdio.h>
int main()
{
int a, b;
a=2;
b=2;
if(a>b || a= = b)
printf("a is greater than or equal to b");
else 
printf("b is greater than a");
return 0;
}

Answer:
a is greater than or equal to b

Note: symbol || denote OR i.e., a>b || a= = b denote a is greater than or a is equal to b.


Program 1.8
C program to find the average of 10 numbers

#include<stdio.h>
int main()
{
int N1, N2, N3, N4, N5, N6, N7, N8, N9, N10, X;
printf("Enter any 10 numbers:");
scanf("%d%d%d%d%d%d%d%d%d%d", &N1, &N2, &N3, &N4, &N5, &N6, &N7, &N8, &N9, &N10);
X = (N1 + N2 + N3 + N4 + N5 + N6 + N7 + N8 + N9 + N10) /10;
printf("the average of 10 numbers = %d", X);
return 0;
}

The output on the screen:

Enter any 10 numbers:
If you enter ten numbers 1, 2, 3, 4, 5, 6, 7, 8, 9 and 10
the average of 10 numbers = 5
will be outputted on the screen.

	Note: The average of 10 numbers is 5.5, the output on the screen is 5 because the data type int is used instead of float.

•	Any mathematical expression should be written in C equivalent expression to prevent the display of compilation error on the screen because C language does not accept the general mathematical expressions.

Mathematical expression	C equivalent expression
x × y / z	x * y / z
(ax + 1) (by + 2)	(a * x + 1) * (b * y + 2)
(a+b)2/ (a-b)2	(a+b) * (a+b) / (a-b) * (a-b) 
or 
pow((a+b), 2) / pow((a - b), 2)
log 10 (x/y + c)	log 10 (x/y + c)
ax2+bx+c	a*x*x+b*x+c
lnx	log(x)
ex + b	exp (x) + b
sinθ + cosθ	sin (theta) + cos (theta)
α = β + γ	alpha = beta + gamma
x 1/2	sqrt(x)
x 1/3	cbrt(x)
(p2 + q2)1/2	sqrt (p*p + q*q)
2a2 + 3b	2a *a + 3b + 2
a = e x / (1+ sinθ)1/2	a = exp ( x / sqrt ( 1 + sin (theta)))


	What will be the output of the following programs:

(a)

#include <stdio.h>
#include<math.h>
int main()
{
int a, b, x; 
x=2;
b=2;
a = exp (x) + b;
printf("the value of a = %d", a);
return 0;
}

Answer:
the value of a = 9

(b)

#include <stdio.h>
#include<math.h>
int main()
{
int alpha, beta, gamma;
alpha =2;
beta=2;
gamma=  2 * alpha +  beta;
printf("the value of alpha = %d", alpha);
return 0;
}

Answer:
the value of alpha = 2




(c)

#include <stdio.h>
#include<math.h>
int main()
{
double theta,  result;
theta = 90;
result = sin(theta);
printf ("The sine 90 degrees is = %lf ", result);
return 0;
}

Answer:
The sine 90 degrees is = 0.893997

	What is C equivalent expression of (x/y) n-1?

Answer:   pow((x/y), n-1)


Program 1.9

C program to find the square root of a number

#include<stdio.h>
#include<math.h>
int main()
{
int a, b;
printf("Enter any number:");
scanf("%d", & a);
b = sqrt (a);
printf("the square root of a number = %d", b);
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 4
the square root of a number = 2
is outputted on the screen.

Suppose if you enter the number 2, the square root of a number = 1 is outputted on the screen because int is used instead of float. 

	Note: 

Since b = sqrt (a) is written

#include<math.h>

must be included in the above program otherwise compilation error will flag on the screen.
i.e., the program:

#include<stdio.h>
int main()
{
int a, b;
printf("Enter any number:");
scanf("%d", & a);
b = sqrt (a);
printf("the square root of a number = %d", b);
return 0;
}

will flag compilation error on the screen.
If float is used instead of int then the above program take the form:

#include<stdio.h>
#include<math.h>
int main()
{
float a, b;
printf("Enter any number:");
scanf("%d", & a);
b = sqrt (a);
printf("the square root of a number = %f", b);
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 5
the square root of a number = 2.23
is outputted on the screen.

This program can also be written as:

#include<stdio.h>
#include<math.h>
int main()
{
printf("the square root of a number = %f", sqrt (4));
return 0;
}

//--------------------------------------------------------------------------------------------------------------------------------------


|| imply or
> imply greater than
<imply less than
= = imply equal to
! imply not
!= imply not equal to
&& imply and
& imply address


-------------------------------------------------------------------------------------------------------------------------------------//
Program 2.0
C program to find the simple interest

#include<stdio.h>
int main()
{
int P,T, R, SI;
P = 1000;
T = 2;
R = 3;
SI = P*T*R/100;
printf("the simple interest = %d", SI);
return 0;
}

The output on the screen:
the simple interest = 60

	Note: 
If you write SI = PTR/100; instead of SI = P*T*R/100;
Then compilation error is displayed on the screen because C language does not accept the general expressions.

If you want to supply the values for P, T and R through the key board, then the statements:

P = 1000;
T = 2;
R = 3; 

should be replaced by the statements:

printf("Enter any number:");
scanf("%d", &P);
printf("Enter any number:");
scanf("%d", &T);
printf("Enter any number:");
scanf("%d", &R);

i.e., the above program should take the form:

#include<stdio.h>
int main()
{
int P,T, R, SI;
printf("Enter principal amount:");
scanf("%d", &P);
printf("Enter time:");
scanf("%d", &T);
printf("Enter rate of interest:");
scanf("%d", &R);
SI = P*T*R/100;
printf("the simple interest = %d", SI);
return 0;
}

The output on the screen:

Enter principal amount:
If you enter the principal amount 1000
Enter time:
If you enter the time 2
Enter rate of interest:
If you enter the rate of interest 3
the simple interest = 60
will be outputted on the screen.

	Note: If write the statement scanf("%d,"&P); instead of scanf("%d", &P);
or
if write the statement scanf(%d, &P); instead of scanf("%d", &P); i.e., format string for data type int i.e., %d is not enclosed by double quotes ("")
Then compilation error will be displayed on the console screen.

Program 2.1

C program to find whether the person is senior citizen or not

#include<stdio.h>
int main()
{
int age;
age=20;
if(age> = 60)
{
printf("senior citizen");
}
if(age<60)
{
printf("not a senior citizen");
}
return 0;
}

The output on the screen:
not a senior citizen
(age> = 60) means age greater than or equal to 60
If you want to supply the value for age through the key board, then the statement
age=20;
should be replaced by the statements:

printf("Enter age:");
scanf("%d", &age);

i.e., the above program should take the form:

#include<stdio.h>
int main()
{
int age;
printf("Enter age:");
scanf("%d", &age);
if(age>60)
{
printf("senior citizen");
}
if(age<60)
{
printf("not a senior citizen");
}
return 0;
}

The output on the screen:
Enter age:
If you enter the value 60 
senior citizen will be outputted on the screen.
Suppose if you enter the value 27
not a senior citizen will be outputted on the screen.

Program 2.2

C program to get marks for 3 subjects and declare the result.
If the marks >= 35 in all the subjects the student passes else fails.

#include<stdio.h>
int main()
{
int M1, M2,M3;
M1 = 38;
M2= 45;
M3 = 67;
if(M1>= 35 && M2>= 35 && M3>= 35)
{
printf("candidate is passed");
}
else
{
printf("candidate is failed");
}
return 0;
}

The output on the screen:
candidate is passed
													
>= imply greater than or equal to and double ampersand imply and
(M1>= 35 && M2>= 35 && M3>= 35) denote the condition and this condition imply M1 is greater than or equal to 35 
and M2 is greater than or equal to 35 and M3 is greater than or equal to 35. And if this condition is TRUE, then the statement 
{
printf("candidate is passed");
}
is executed to print the output:
candidate is passed
else the statement 
{
printf("candidate is failed");
}
is executed to print the output:
candidate is failed

If you want to supply the integer values for marks M1, M2 and M3 through the key board, then the statements:

M1 = 38;
M2= 45;
M3 = 67; 

should be replaced by the statements:

printf("Enter any three numbers:");
scanf("%d%d%d", &M1, &M2, &M3);

i.e.,

#include<stdio.h>
int main()
{
int M1, M2,M3;
printf("Enter any three numbers:");
scanf("%d%d%d", &M1, &M2, &M3);
if(M1>= 35 && M2>= 35 && M3>= 35)
{
printf("candidate is passed");
}
else
{
printf("candidate is failed");
}
return 0;
}

The output on the screen:
Enter any three numbers:
If you enter three numbers 26, 28, 39
candidate is failed will be outputted on the screen.


Header file in C	the functions it  defines
stdio.h	(standard input output header file)	
	standard input output functions (like scanf and printf functions)
math.h	mathematical functions (like  log(), sqrt(), sin(), cos(), log10() etc.)
stdlib.h	standard library functions (like void abort(void) - a function which causes an abnormal/ unusual program termination)
ctype.h	character manipulation functions
(like isalpha() which checks whether a character is an alphabet or not)
graphics.h	graphical functions
conio.h	(console input output header file)	
console input output functions like clrscr() - a function which clears the screen.


	Note: The term console usually refers to monitor or display screen.


	Write a program to check whether a character is an alphabet or not using the function isalpha()

#include <stdio.h>
#include <ctype.h>
int main()
{
int a =2;
if( isalpha(a) )
{
printf(" the character a  is an alphabet");
}
else
{
printf("the character a  is not an alphabet");
}
return 0;
}
The output on the screen:
the character a  is not an alphabet											
#include <stdio.h>
#include <ctype.h>
int main()
{
char a = 'b';
if( isalpha(a) )
{
printf(" the character a  is an alphabet");
}
else
{
printf("the character a  is not an alphabet");
}
return 0;
}

The output on the screen:
the character a  is an alphabet

If the statement char a = b; is written instead of char a = 'b'; Then the compilation error will be flagged on the display screen.

Program 2.3
C program to find profit or loss

#include<stdio.h>
int main()
{
int CP, SP, loss, profit;
printf("Enter cost price:");
scanf("%d", &CP);
printf("Enter selling price:");
scanf("%d", &SP);
if(SP>CP)
{
printf("profit=%d", SP-CP);
}
else
{
printf("loss =%d", CP-SP);
}
return 0;
}

The output on the screen:
Enter cost price:
If you enter the cost price 25
Enter selling price:
If you enter the selling price 26
profit = 1 will be outputted on the screen.
If the condition (SP>CP) is true, then the statement 

{
printf("profit=%d", SP-CP);
}
is executed to print the output:
profit = SP-CP (in this case profit = 26-25 =1)
else the statement

{
printf("loss=%d", CP-SP);
}

is executed to print the output:
loss = CP-SP
						
Program 2.4
C program to convert inches into centimeter

#include<stdio.h>
int main()
{
float I, C;
I=3.5;
C = 2.54*I;
printf("length in centimeters= %f", C);
return 0;
}

The output on the screen:
length in centimeters = 8.89
	Note: float is used instead of int because I = 3.5 if int is used instead of float then the result will not be clearly outputted i.e., instead of 8.89 the computer displays only 8. And since float is used instead of int, the operator %d is replaced by the operator %f.

If you want to supply the floating value for I through the key board, then the above program should take the form:

#include<stdio.h>
int main()
{
float I, C;
printf("Enter the length in inches:");
scanf("%f", &I);
C = 2.54*I;
printf("length in centimeters= %f", C);
return 0;
}

The output on the screen:
Enter the length in inches:
If you enter the floating point value or fractional or decimal number for I i.e., 25.5
length in centimeters = 64.9 will be outputted on the screen.


Program 2.5

C program to find the incremented and decremented values of two numbers.

#include<stdio.h>
int main()
{
int a, b, c, d, e, f;
a = 10;
b=12;
c=a+1; 
d=b+1;
e=a-1;
f=b-1;
printf("the incremented value of a =%d", c);
printf("the incremented value of b =%d", d);
printf("the decremented value of a =%d", e);
printf("the decremented value of b =%d", f);
return 0;
}

The output on the screen:
the incremented value of a = 11 the incremented value of b = 13 the decremented value of a = 9 the decremented value of b = 11

If the statements:

printf("the incremented value of a =%d", c);
printf("the incremented value of b =%d", d);
printf("the decremented value of a =%d", e);
printf("the decremented value of b =%d", f);

are replaced by the statements:

printf("the incremented value of a =%d\n", c);
printf("the incremented value of b =%d\n", d);
printf("the decremented value of a =%d\n", e);
printf("the decremented value of b =%d\n", f);

Then the output on the screen is:
the incremented value of a = 11
the incremented value of b = 13
the decremented value of a = 9
the decremented value of b = 11

	Note:

Even if the statements:

printf("the incremented value of a =%d\n", c);
printf("the incremented value of b =%d\n", d);
printf("the decremented value of a =%d\n", e);
printf("the decremented value of b =%d\n", f);

are replaced by the statements:

printf("\n the incremented value of a =%d", c);
printf("\n the incremented value of b =%d", d);
printf("\n the decremented value of a =%d", e);
printf("\n the decremented value of b =%d", f);

There will be no change in the output on the screen.

If you want to supply the values for a and b through the key board, then the above program should take the form:

#include<stdio.h>
int main()
{
int a, b, c, d, e, f;
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);
c=a+1;
d=b+1;
e=a-1;
f=b-1;
printf("the incremented value of a =%d\n", c);
printf("the incremented value of b =%d\n", d);
printf("the decremented value of a =%d\n", e);
printf("the decremented value of b =%d\n", f);
return 0;
}

The output on the screen:

Enter any number:
If you enter the number 2
Enter any number:
If you enter the number 3

the incremented value of a = 3
the incremented value of b = 4
the decremented value of a = 1
the decremented value of b = 2

will be outputted on the screen.

Note: b++ is same as b + 1 and b-- is same as b - 1. 

Program 2.6

The percentage marks are entered and the grades are allotted as follows :	
percentage>= 60 First Class
percentage>=50 and per <= 60 Second Class
percentage>= 40 and per <= 50 Pass Class
percentage< 40 Fail
Write a C program for the above:

#include<stdio.h>
int main()
{
int P;
printf("Enter the percentage:");
scanf("%d", &P);
if(P >= 60)
{
printf("first class");
}
if(P>=50&&P <60)
{
printf("second class");
}
else if(P>=40&&P<=50 )
{
printf("pass class");
}
else
{
printf("fail");
}
return 0;
}

The output on the screen:
Enter the percentage:
If you enter the percentage 65 
first class will be outputted on the screen.

Program 2.7

C program to calculate the discounted price and the total price after discount
Given:
If purchase value is greater than 1000, 10% discount
If purchase value is greater than 5000, 20% discount
If purchase value is greater than 10000, 30% discount

	discounted price

#include<stdio.h>
int main()
{
double PV, dis;
printf("Enter purchased value:");
scanf("%lf", &PV);
if(PV>1000)
{
printf("dis=%lf", PV* 0.1);
}
else if(PV>5000)
{
printf("dis =%lf", PV* 0.2);
}
else
{
printf("dis=%lf", PV* 0.3);
}
return 0;
}

The output on the screen:
Enter purchased value:
If you enter the purchased value 6500 
dis = 1300.000000 will be outputted on the screen.

(PV>1000), (PV>5000) denote the conditions and if the condition (PV>1000) is true i.e., purchased value is greater than 1000, then the statement 

{
printf("dis=%d", PV* 0.1);
}

is executed to print the output:
dis= PV* 10% = PV* 10 /100 = PV* 0.1
and if the condition (PV>1000) is false and if the condition (PV>5000) is true i.e., purchased value is greater than 5000, then the statement 

{
printf("dis=%d", PV* 0.2);
}

is executed to print the output:
dis= PV* 20% = PV* 20 /100 = PV* 0.2
and if the condition (PV>5000) is not true i.e., purchased value is less than 5000, then the statement

{
printf("dis=%d", PV* 0.3);
}

is executed to print the output:
dis= PV* 30% = PV* 30 /100 = PV* 0.3

	total price 

#include<stdio.h>
int main()
{
double PV, total;
printf("Enter purchased value:");
scanf("%lf", &PV);
if(PV<1000)
{
printf("total=%lf", PV - PV* 0.1);
}
else if(PV<5000)
{
printf("total =%lf", PV- PV* 0.2);
}
else
{
printf("total=%lf", PV- PV* 0.3);
}
return 0;
}

The output on the screen:
Enter purchased value:
If you enter the purchased value 650 
total = 585.000000  will be outputted on the screen.

If the condition (PV>1000) is true i.e., purchased value is greater than 1000, then the statement 

{
printf("total = %d", PV - PV* 0.1);
}

is executed to print the output:
total =PV- dis = PV- PV*10% = PV- PV* 10 /100 = PV - PV * 0.1
and if the condition (PV>1000) is false and if the condition (PV>5000) is true i.e., purchased value is greater than 5000, then the statement

{
printf("total = %d", PV - PV* 0.2);
}

is executed to print the output:
total =PV- dis = PV- PV*20% = PV- PV* 20 /100 = PV - PV * 0.2
							
and if the condition (PV> 5000) is not true i.e., purchased value is less than 5000, then the statement

{
printf("total = %d", PV - PV* 0.3);
}

is executed to print the output:

total =PV- dis = PV- PV*30% = PV- PV* 30 /100 = PV - PV * 0.3

Now, Combing both the programs (above), we can write:

#include<stdio.h>
int main()
{
double PV, dis, total;
printf("Enter purchased value:");
scanf("%lf", &PV);
if(PV>1000)
{
printf("dis=%lf", PV* 0.1);
printf("total=%lf", PV - PV* 0.1);
}
else if(PV>5000)
{
printf("dis =%lf", PV* 0.2);
printf("total=%lf", PV - PV* 0.1);
}
else
{
printf("dis=%lf", PV* 0.3);
printf("total=%lf", PV - PV* 0.1);
}
return 0;
}

The output on the screen:
Enter purchased value:
If you enter the purchased value 850 
dis = 85.000000
total = 765.000000
will be outputted on the screen.

Program 2.8

	C program to print the first ten natural numbers using for loop statement

#include<stdio.h>
int main()
{
int i;
for (i=1; i<=10; i++)
printf("value of i =%d", i);
return 0;
}

The output on the screen is:
value of i = 1 value of i = 2  value of i= 3  value of i= 4  value of i= 5  value of i= 6 value of i = 7 value of i= 8  value of i = 9  value of i = 10

for (i=1; i<=10; i++) denote the 
for loop statement and the syntax of the 
				for loop statement is:
for (initialization; condition; increment)
Here:
i=1 denote initialization (i.e., from where to start)
i<=10 denote the condition (i.e., stop when 10 is reached)
i++ imply increment (which tells the value of i to increase by 1 each time the loop is executed) and i++ is the same as i+1.

	When a for loop executes, the following occurs:

i = 1
Is the condition (i<=10) is true?
Yes because i=1
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 1
Now, the value of i is:
i =  1+1 = 2
Is the condition (i<=10) is true?
Yes because i=2
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 2
Now, the value of i is:
i =  2+1 = 3
Is the condition (i<=10) is true?
Yes because i=3
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 3
Now, the value of i is:
i =  3+1 = 4
Is the condition (i<=10) is true?
Yes because i=4
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 4
Now, the value of i is:
i =  4+1 = 5
Is the condition (i<=10) is true?
Yes because i=5
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 5
Now, the value of i is:
i =  5+1 = 6
Is the condition (i<=10) is true?
Yes because i=6
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 6
Now, the value of i is:
i =  6+1 = 7
Is the condition (i<=10) is true?
Yes because i=7
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 7
Now, the value of i is:
i =  7+1 = 8
Is the condition (i<=10) is true?
Yes because i=8
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 8
Now, the value of i is:
i =  8+1 = 9
Is the condition (i<=10) is true?
Yes because i=9
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 9
Now, the value of i is:
i =  9+1 = 10
Is the condition (i<=10) is true?
Yes because i=10
The statement printf("value of i =%d", i); is executed to print the output:
value of i = 10
and stop because the condition i<=10 is achieved.

If the statement: 
printf("value of i =%d", i);
is replaced by the statement: 
printf("value of i =%d\n", i);
				               or 
				 printf("\n value of i =%d", i);   
				
Then the output on the screen is:

value of i = 1
value of i = 2
value of i = 3
value of i = 4
value of i = 5
value of i = 6
value of i = 7
value of i = 8
value of i = 9
value of i = 10

If the 
for loop statement: 

for (i=2; i<=10; i++) 

is written instead of the statement: 

for(i=1; i<=10; i++), then the output on the screen is:

value of i = 2  value of i = 3  value of i= 4  value of i= 5  value of i= 6 value of i = 7 value of i= 8  value of i = 9  value of i= 10

If the for loop statement: 
for(i=1; i<10; i++)
is written instead of the statement: 
for (i=1; i<=10; i++), then the output on the screen is:
value of i = 1 value of i = 2  value of i= 3  value of i= 4  value of i= 5  value of i= 6 value of i = 7 value of i= 8  value of i = 9

(Note: the condition i<=10 tells to print till value of i =10 but the condition i<10 tells to print till value of i=9)

If the statement:
for(i=1; i=10; i++) 
is written instead of the statement:
for (i=1; i<=10; i++), then the output on the screen is:
value of i = 10  value of i = 10  value of i = 10  value of  i = 10  value of i= 10  value of i= 10 value of i = 10 value of i= 10  value of i = 10   value of i = 10   value of i = 10   value of i = 10  value of i = 10    value of i = 10   value of i = 10 (continues ...).

Note:

If the statement:
printf("value of i =%d", i); is replaced by the statement printf("%d\n", i);
Then the output on the screen is:
1
2
3
4
5
6
7
8
9
10

	What will be the output of the following program :

#include<stdio.h>
int main()
{
int i;
for (i =1; i<=5; i ++)
printf("Linux is not portable\n", i);
return 0;
}

Answer:

Linux is not portable
Linux is not portable
Linux is not portable
Linux is not portable
Linux is not portable

	C program to print the first ten natural numbers using for while loop statement

The syntax of while loop statement is:
while (this is the condition)
{
execute this statement;
}

#include<stdio.h>
int main()
{
int i = 1;
while (i<=10)
{
printf("%d\n", i++);
}
return 0;
}

The output on the screen is:

1
2
3
4
5
6
7
8
9
10

(i<=10) is the condition and 

The statement 
printf("%d\n", i++);

is repeatedly executed as long as a given condition (i<=10) is true.
If the statement:
int i=1;
is replaced by the statement:
int i;

Then the compilation error will be displayed on the console screen because initialization is not defined i.e., from where to start is not declared.

If the statement:
int i = 1; 
is replaced by the int i = 0; 
Then the output on the screen is:
0
1
2
3
4
5
6
7
8
9
10
Similarly if the statement int i = 0; is replaced by the int i = 7; 
Then the output on the screen is:
7
8
9
10

	C program to print first 10 numbers using do while loop statement

The syntax of do while loop statement is:

do
{
execute this statement;
}
while(this is the condition);

#include<stdio.h>
int main()
{
int i =1;
do 
{
printf(" i= %d\n", i++);
} while (i<=10);
return 0;
}

The output on the screen is:
i=1
i=2
i=3
i=4
i=5
i=6
i=7
i=8
i=9
i=10

The statement:
printf(" i= %d\n", i++);
is executed and then condition (i<=10) is checked. If condition (i<=10) is true then 
The statement:
printf(" i= %d\n", i++);
is executed again. This process repeats until the given condition (i<=10) becomes false.

	Why LOOP is USED?

If loop is not used then the C program to print first 10 numbers should be written as follows:

#include<stdio.h>
int main()
{
printf("\n i = 1");
printf("\n i = 2");
printf("\n i = 3");
printf("\n i = 4");
printf("\n i = 5");
printf("\n i = 6");
printf("\n i = 7");
printf("\n i = 8");
printf("\n i = 9");
printf("\n i = 10");
return 0;
}

It takes pretty long time to write the code and the execution time is pretty long i.e., Because to reduce the time taken to write the code and to reduce the execution time -- loop statement is used.

	Write a program to print:

Never test for an error condition you don't know how to handle

5 times using for loop statement.

Answer:

#include<stdio.h>
int main()
{
int i;
for (i =1; i<=5; i ++)
printf("Never test for an error condition you don't know how to handle \n");
return 0;
}

	Note:

For the program:

#include<stdio.h>
int main()
{
int i;
for (i=1; i=5; i++)
printf("Linux is not portable");
return 0;
} 

The output on the screen is:

Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable …. continues


Program 2.9
C program to print the characters from A to Z using for loop, do while loop and while loop statement.

	C program to print the characters from A to Z using for loop statement:

#include<stdio.h>
int main()
{
char a;
for( a='A'; a<='Z'; a++)
printf("%c\n", a);
return 0;
}

The output on the screen:

A
B
C
D
E
F
G
H
I
J
K
L
M
N
O
P
Q
R
S
T
W
X
Y
Z

char means the data type is character.

The statement 
char a; imply that we are creating the character a.

Since char a is used. Therefore: the format specifier %c should be used instead of  %d or %f otherwise error will be flagged on the screen.

If the statement for( a=A; a<=Z; a++) is written instead of the statement for( a='A'; a<='Z'; a++)
Then the compilation error will be displayed on the console screen.

	C program to print the characters from A to Z  using while loop statement:

#include<stdio.h>
int main()
{
char a = 'A';
while (a<='Z')
{
printf("%c\n", a++);
}
return 0;
}

	C program to print the characters from A to Z using do while loop statement:

#include<stdio.h>
int main()
{
char a = 'A';
do 
{
printf(" %c\n", a++);
} while (a<='Z');
return 0;
}

Program 3.0
C program to print the given number is even or odd.

#include<stdio.h>
int main()
{
int a;
printf("Enter any number:");
scanf ("%d", &a);
if(a%2 = = 0)
{
printf("the number is even");
}
else
{
printf("the number is odd");
}
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 4
the number is even will be outputted on the screen.

	Mathematical symbol % denote modulus and (a%2 = = 0) is the condition and this condition imply: a divided by 2 yields reminder = 0.

For example: if you enter the number 4
Then a = 4
Then 4 divided by 2 yields the remainder = 0
Then the statement 
{
printf("the number is even");
}
is executed to print the output:
the number is even
(Note: in C language = = implies equal to)

Suppose if you enter the number 3
Then a = 3
Then 3 divided by 2 yields the remainder = 1
Then the statement 
{
printf("the number is odd");
}
is executed to print the output:
the number is odd

Data type	Storage size
char	1 byte
short int	2 byte
float, long int	4 byte
double, long double	8 byte


Program 3.1

C program to print the remainder of two numbers 

#include<stdio.h>
int main()
{
int a, b, c;
printf("Enter any number:");
scanf("%d", &a);
printf("Enter any number:");
scanf("%d", &b);
c = a%b;
printf("the remainder of a and b = %d", c);
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 3
Enter any number:
If you enter the number 2
the remainder of a and b = 1 will be outputted on the screen.
						
Since (a=3 and b=2). Therefore:
3 divided by 2 (i.e., a divided by b) yields the remainder equal to 1
				
If the statement:
printf("the remainder of a and b = %d", c); 
is replaced by the statement: 
printf("the remainder of %d and %d = %d", a, b, c);

Then the output on the screen is:
Enter any number:
If you enter the number 3
Enter any number:
If you enter the number 2
the remainder of 3 and 2 = 1 will be outputted on the screen.

Program 3.2
C program to check the equivalence of two numbers.

#include<stdio.h>
int main()
{
int x, y;
printf("Enter any number:");
scanf ("%d", &x);
printf("Enter any number:");
scanf ("%d", &y);
if(x-y==0)
{
printf("the two numbers are equivalent");
}
else
{
printf("the number are not equivalent");
}
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 2
Enter any number:
If you enter the number 2
the two numbers are equivalent will be outputted on the screen.

Since 2-2 is equal to 0 (i.e., x-y = = 0). 
Therefore: the statement 
{
printf("the two numbers are equivalent");
}
is executed to print the output:
two numbers are equivalent

If you enter the integers 3 and 2
The output on the screen:
the two numbers are not equivalent

Since 3-2 is not equal to 0 (i.e., x-y != 0). Therefore: the statement 
{
printf("the two numbers are not equivalent");
}
is executed to print the output:
two numbers are not equivalent
								
(as said earlier: in C language the symbol != implies not equal to)

	What is the mistake in the following program:

#include<stdio.h>
int main()
{
int year;
year =1996;
if(year%4==0)
printf("leap year");
else
printf("not a leap year");
return 0;
}

Answer: 

There is no mistake in the above program. The output on the screen is:
leap year

Since year=1996. Therefore:
1996 divided by 4 (i.e., year divided by 4) yields the remainder equal to 0.
The statement 

printf("leap year");

is executed to print the output:
leap year
If the year is = 1995. Then 
1995 divided by 4 (i.e., year divided by 4) yields the remainder not equal to 0.
The statement 

printf("not a leap year");

is executed to print the output:
not a leap year

	Note: for a year to be leap year, year divided by 4 should yield remainder = zero.



// ----------------------------------------------------------------------------------------------------------------------------------

	An algorithm must be seen to be believed.
Donald Knuth

You might have an algorithm for getting from office home , for making a chunk of code that calculates the terms of the Fibonacci sequence , or for finding what you're looking for in a retail store . Algorithms are the building blocks of computer programs or a sequence of a sequence of unambiguous instructions ( the term 'unambiguous ' indicates that there is no room for subjective interpretation ) that tells how the problem can be addressed and solved - - which is definitely overblown in their importance like road maps for accomplishing a given , well-defined automated reasoning task - - which always have a clear stopping point . Long division and column addition are examples that everyone is familiar with- even a simple function for adding two numbers is an implementation of a particular algorithm. Online grammar checking uses algorithms . Financial computations use algorithms . A search engine like Google uses search engine algorithms (for example , takes search strings of keywords as input , searches its associated database for relevant web pages , and returns results ) . In fact , it is difficult to think of a task performed by your computer that does not use computer procedures that are a lot like a recipes (called algorithms ) .


	The algorithm to add two numbers entered by userwould look something like this:
	Step 1: Start
	Step 2: Declare variables num1, num2 and sum. 
	Step 3: Read values num1 and num2. 
	Step 4: Add num1 and num2 and assign the result to sum.
sum←num1+num2
	Step 5: Display sum 
	Step 6: Stop

Algorithms are the heart of computer science (usually means a procedure or basically an instance of logic written in software that solves a recurrent problem of finding an item with specific properties among a collection of items or transforming data according to specified actions to protect it) , and the subject has countless practical applications as well as intellectual depth that is widely used throughout all areas of information technology including solving a mathematical problem (as of finding the greatest common divisor) in a finite number of steps that frequently involves repetition of an operation. The word algorithm - a mathematical concept whose roots date back to 600 AD with the invention of the decimal system -- derives from the name of the Muslim mathematician and astronomer , Mohammed ibn-Musa al-Khwarizmi , who was part with the royal court in Baghdad and who lived from about 780 to 850 . The use of computers , however , has elevated the use of algorithms in daily transactions (like accessing an automated teller machine (ATM) , booking an air or train or buying something online) to unprecedented levels of real-world problems with solutions requiring advanced algorithms abounds. And their use is only likely to grow. Many of the problems, though they may not seem realistic, require the set of well-defined algorithmic knowledge that comes up every day in the real world. By developing a good understanding of a series of logical steps in an algorithmic language, you will be able to choose the right one for a problem and apply it properly.

The algorithm is written in human readable and understandable form. To search an element in a given array, it can be done in two ways: Linear search and Binary search.

	Linear Search:


Linear search is a very basic and simple search algorithm. In this type of search, a sequential search is made over all elements one by one. Every element is checked and if a match is found then that particular element is returned, otherwise the search continues till the end of the data collection.

For Example:

To search the element 17 it will go step by step in a sequence order:

8	10	12	15	17	20	25
=
17 


Match not found

8	10	12	15	17	20	25
=
17 

Match not found

8	10	12	15	17	20	25
=
17 

Match not found

8	10	12	15	17	20	25
=
17 

Match not found

8	10	12	15	17	20	25
=
17 
Match found

Element 17 is returned

Linear search (whose running time increases linearly with the number of elements in the array. For example if number of elements is doubled then, on average, the search would take twice as long) is rarely used practically because other search algorithms such as the binary search algorithm and hash tables allow significantly faster searching comparison to linear search. 

	Binary Search
http://studytipsandtricks.blogspot.in/2012/08/explanation-of-local-and-global.html

Local variables: 
Variable whose existence is known only to the main program or functions are called local variables. Local variables are declared with in the main program or a function.

Global variables: 
Variables whose existence is known to the both main() as well as other functions are called global variables. Global variables are declared outside the main() and other functions.
The following Program illustrates the concept of both local as well as global variables.

	#include<stdio.h>
	// Global variables
	int A;
	int B;
	int Add()
	{
		return A + B;
	}
	int main()
	{
		int answer; // Local variable
		A = 5;
		B = 7;
		answer = Add();
		printf("%d\n",answer);
		return 0;
	}
Consider the following two definitions of main().
intmain()
{
   /*  */
   return0;
}
Run on IDE
and
intmain(void)
{
   /*  */
   return0;
}
Run on IDE
What is the difference?
In C++, there is no difference, both are same.
Both definitions work in C also, but the second definition with void is considered technically better as it clearly specifies that main can only be called without any parameter.
#include <stdio.h>
int main () {
char greeting[6] = {'H', 'e', 'l', 'l', 'o', '\0'};
printf("Greeting message: %s\n", greeting );
return 0;
}
#include <stdio.h>
#define LENGTH 10   
#define WIDTH  5
#define NEWLINE '\n'

int main() {
int area;  
area = LENGTH * WIDTH;
printf("value of area : %d", area);
printf("%c", NEWLINE);
return 0;
}
#include<stdio.h>
int main(){
constint  LENGTH =10;
constint  WIDTH =5;
constchar NEWLINE ='\n';
int area;
area = LENGTH * WIDTH;
printf("value of area : %d", area);
printf("%c", NEWLINE);
return0;
}
Note that it is a good programming practice to define constants in CAPITALS.
Binary Search is applied on the sorted array or list. In binary search, we first compare the value with the elements in the middle position of the array. If the value is matched, then we return the value. If the value is less than the middle element, then it must lie in the lower half of the array and if it's greater than the element then it must lie in the upper half of the array. We repeat this procedure on the lower (or upper) half of the array. Binary Search is useful when there are large numbers of elements in an array.
We shall learn the process of binary search with a pictorial example. The following is our sorted array and let us assume that we need to search the location of value 31 using binary search.
 
First, we shall determine half of the array by using this formula −
mid = low + (high - low) / 2

Here it is, 0 + (9 - 0 ) / 2 = 4 (integer value of 4.5). So, 4 is the mid of the array.
 
Now we compare the value stored at location 4, with the value being searched, i.e. 31. We find that the value at location 4 is 27, which is not a match. As the value is greater than 27 and we have a sorted array, so we also know that the target value must be in the upper portion of the array.
 
We change our low to mid + 1 and find the new mid value again.
low = mid + 1
mid = low + (high - low) / 2
Our new mid is 7 now. We compare the value stored at location 7 with our target value 31.
 
The value stored at location 7 is not a match, rather it is more than what we are looking for. So, the value must be in the lower part from this location.
 
Hence, we calculate the mid again. This time it is 5.
 
We compare the value stored at location 5 with our target value. We find that it is a match.
 
We conclude that the target value 31 is stored at location 5.


Binary search tree 

Consider a array:

 
2
1
3
5
9
12
18
15
19
17



12 = root 

Left subtree (lesser)  < root 

Right subtree (greater) > root 
-------------------------------------------------------------------------------------------------------------------------------- //

Program 3.3
C program to print whether the given number is positive or negative

#include<stdio.h>
int main()
{
int a;
a = -35;
if(a>0)
{
printf("number is positive");
}
else
{
printf(" number entered is negative");
}
return 0;
}

The output on the screen:
number entered is negative
										
Since a = -35. Therefore:
a is less than 0 i.e., a < 0 because any negative number is always less than zero.
The statement 
{
printf("number is negative");
}
is executed to print the output:
number entered is negative

Program 3.4
C program to print the sum of the first 10 digits using for loop statement

#include<stdio.h>
int main()
{
int i, sum = 0;
for( i=1; i<=10; i++)
sum = sum + i;
printf("sum of the first 10 digits =%d", sum);
return 0;
}

The output on the screen:
sum of the first 10 digits = 55


	How the sum of the first 10 digits = 55 is outputted on the screen through the for Loop statement?

i=1 (sum = 0 because the sum is initialized to 0 in the statement int i, sum = 0;)
Is i<=10 true?
Yes, do this 
sum = sum + i = 0 +1 =1
Now,
i=2 (sum = 1)
Is i<=10 true?
Yes, do this 
sum = sum + i = 1 +2 =3
Now,
i=3 (sum = 3)
Is i<=10 true?
Yes, do this 
sum = sum + i = 3 +3 = 6
Now,
i=4 (sum = 6)
Is i<=10 true?
Yes, do this 
sum = sum + i = 6 + 4= 10
Now,
i=5 (sum = 10)
Is i<=10 true?
Yes, do this 
sum = sum + i = 10 + 5= 15
Now,
i=6 (sum = 15)
Is i<=10 true?
Yes, do this 
sum = sum + i = 15 + 6 = 21
Now,
i=7 (sum = 21)
Is i<=10 true?
Yes, do this 
sum = sum + i = 21 + 7 = 28
Now,
i=8 (sum = 28)
Is i<=10 true?
Yes, do this 
sum = sum + i = 28 + 8 = 36
Now,
i=9 (sum = 36)
Is i<=10 true?
Yes, do this 
sum = sum + i = 36 + 9 = 45
Now,
i=10 (sum = 45)
Is i<=10 true?
Yes, do this 
sum = sum + i = 45 + 10 = 55
stops because the condition i<=10 is achieved

The statement:
printf("sum of the first 10 digits =%d", sum);
is executed to print the output:
sum of the first 10 digits = 55
									
If the statement:
int i, sum = 0;
is replaced by int i, sum = 1;
Then the output on the screen is:
sum of the first10 digits = 56

	What will be the output if the for loop statement for(i =1; i<=10; i++) is replaced by the statement for(i =2; i<10; i++)?

Answer: sum of 10 digits = 44
If the statement int i, sum, sum = 0; is written instead of int i, sum = 0;
Then the compilation error message will be displayed on the screen (stating that sum is twice declared).

If the for loop is ended with a semicolon i.e.,
for( i=1; i<=10; i++);
Then the compilation error will be displayed on the console screen. 

	Note:
	sum = sum + a; is the same as sum + = a;
	sub = sub- a; is the same as sub - = a;
	product = product* a; is the same as product * = a;
	div = div / a; is the same as div /= a;
	a = a% b; is the same as a % = b;


Program 3.5
C program to print the average of the first 10 numbers using for loop statement

#include<stdio.h>
int main()
{
int i, avg, sum = 0;
for( i=1; i<=10; i++)
sum = sum + i;
avg = sum/10;
printf("sum of the first 10 numbers =%d", sum);
printf("average of the first 10 numbers =%d", avg);
return 0;
}

The output on the screen:
sum of the first 10 numbers = 55
average of the first 10 numbers = 5
The average of  the first10 numbers = 55/10 = 5.5 not 5. But the output on the screen is:
average of the first 10 numbers = 5
because int is used instead of float.

If the data type float is used i.e.,
#include<stdio.h>
int main()
{
float i, avg, sum = 0;
for( i=1; i<=10; i++)
sum = sum + i;
avg = sum/10;
printf("sum of the first10 numbers =%f", sum);
printf("average of the first10 numbers = %f", avg);
return 0;
}

The output on the screen:
sum of the first10 numbers = 55
average of the first 10 numbers = 5.5

Program 3.6
C program to print the product of the first 10 digits using for loop statement

#include<stdio.h>
int main()
{
int i, product = 1;
for( i=1; i<=10; i++)
product = product * i;
printf("the product of the first 10 digits =%d", product);
return 0;
}

The output on the screen:
the product of the first 10 digits = 3628800


	How the product of the first 10 digits = 3628800 is outputted on the screen through the for Loop statement?

i=1 (product = 1 because the product is initialized to 1 in the statement int i, product = 1;)
Is i<=10 true?
Yes, do this 
product = product *  i = 1 * 1 =1
Now,
i=2 (product = 1)
Is i<=10 true?
Yes, do this 
product = product *  i = 1 * 2 = 2
Now,
i=3 (product = 2)
Is i<=10 true?
Yes, do this 
product = product *  i = 2 * 3 = 6
Now,
i=4 (product = 6)
Is i<=10 true?
Yes, do this 
product = product *  i = 6 * 4 = 24
Now,
i=5 (product =24)
Is i<=10 true?
Yes, do this 
product = product *  i = 24 * 5 =120
Now,
i=6 (product =120)
Is i<=10 true?
Yes, do this 
product = product *  i = 120 * 6 = 720
Now,
i=7 (product =720)
Is i<=10 true?
Yes, do this 
product = product *  i = 720 * 7 = 5040
Now,
i=8 (product =5040)
Is i<=10 true?
Yes, do this 
product = product *  i = 5040 * 8 = 40320
Now,
i=9 (product = 40320)
Is i<=10 true?
Yes, do this 
product = product *  i = 40320 * 9 = 362880
Now,
i=10 (product = 362880)
Is i<=10 true?
Yes, do this 
product = product *  i = 362880 * 10 = 3628800

stops because the condition i<=10 is achieved.

The statement:
printf("the product of the first 10 digits =%d", product); is executed to display the output:
the product of the first 10 digits = 3628800

If the statement int i, product = 1; is replaced by int i, product = 0;
Then the output on the screen is:
the product of the first 10 digits = 0

If the statement for(i=1; i<=10; i++) is replaced by for(i=5; i<=8; i++)
Then the output on the screen is:
the product of the first 10 digits = 1680


Program 3.7
C Program to print the table of a number using the for loop statement

#include<stdio.h>
int main()
{
int n, i;
printf("Enter any number:");
scanf("%d", &n);
for( i=1; i<=5; i++)
printf("%d * %d = %d\n", n, i, n*i);
return 0;
}

The output on the screen:

Enter any number:
If you enter the number 2 (i.e., n=2)
2 * 1 = 2
2 * 2 = 4
2 * 3 = 6
2 * 4 = 8
2 * 5 = 10
will be outputted on the screen.

	How the execution takes its Way through the for Loop statement

Since you entered the number 2, therefore: n=2.
i=1 
Is i<=5 true?
Yes, print this 
2 * 1 = 2
using the statement printf("%d * %d = %d\n", n, i, n*i);

Now,
i=2
Is i<=5 true?
Yes, print this 
2 * 2 = 4
using the statement printf("%d * %d = %d\n", n, i, n*i);

Now,
i=3
Is i<=5 true?
Yes, print this 
2 * 3 = 6
using the statement printf("%d * %d = %d\n", n, i, n*i);

Now,
i=4
Is i<=5 true?
Yes, print this 
2 * 4 = 8
using the statement printf("%d * %d = %d\n", n, i, n*i);

Now,
i=5
Is i<=5 true?
Yes, print this 
2 * 5 = 10
using the statement printf("%d * %d = %d\n", n, i, n*i);

stop Now because the condition i <=5 is achieved.

If the symbol * is replaced by +
i.e.,

#include<stdio.h>
int main()
{
int n, a;
printf("Enter any number:");
scanf("%d", &n);
for( i=1; i<=5; i++)
printf("%d + %d = %d\n", n, i, n+ i);
return 0;
}

Then the output on the screen is:

Enter any number:
If you enter the number 2 (i.e., n=2)

2 + 1 = 3
2 + 2 = 4
2 + 3 = 5
2 + 4 = 6
2 + 5 = 7

will be outputted on the screen.

Program 3.8 

C program:  
If you enter a character M 
Output must be: ch = M

#include<stdio.h>
int main()
{
char M;
printf("Enter any character:");
scanf("%c", &M);
printf("ch=%c", M);
return 0;
}

The output on the screen: 
Enter any character:
If you enter the character M
ch = M will be outputted on the screen.

	Note:
getchar() function is simplified version of the scanf function

If we replace the statement scanf("%c", &M); by the statement: 
M = getchar();

i.e.,

#include<stdio.h>
int main()
{
char M;
printf("Enter any character:");
M = getchar();
printf("ch=%c", M);
return 0;
}

There will be no change in the output on the screen i.e., The output on the screen is:
Enter any character:
If you enter the character K
ch = K will be outputted on the screen.

putchar() function is simplified version of the printf function
If we replace the statement printf("ch=%c", M);by the statement:
putchar (M);  i.e.,
#include<stdio.h>
int main()
{
char M;
printf("Enter any character:");
scanf("%c", &M);
putchar (M);
return 0;
}

Then there will be no change in the output on the screen i.e., The output on the screen is:
Enter any character:
If you enter the character M
M will be outputted on the screen.

If you replace the statement scanf("%c", &M); by the statement: 
M = getchar();
and the statement printf("ch=%c", M);by the statement:
putchar (M);  i.e.,

#include<stdio.h>
int main()
{
char M;
printf("Enter any character:");
M = getchar();
putchar (M);
return 0;
}

The output on the screen: 
Enter any character:
If you enter the character S
S will be outputted on the screen.

Program 3.9 
C program to print the first 5 numbers starting from one together with their squares.

#include<stdio.h>
int main()
{
int i;
for( i=1; i<=5; i++)
printf("number=%d its square=%d\n", i , i*i);
return 0;
}

The output on the screen:

number=1 its square=1
number=2 its square=4
number=3 its square=9
number=4 its square=16
number=5 its square=25

	How the execution takes its way through the for loop statement
i=1 
Is i<=5 true?
Yes, print this 
number=1 its square=1
using the statement printf("number=%d its square=%d\n", i , i*i);

Now,
i=2 
Is i<=5 true?
Yes, print this 
number=2 its square=4
using the statement printf("number=%d its square=%d\n", i , i*i);

Now,
i=3
Is i<=5 true?
Yes, print this 
number=3 its square=9
using the statement printf("number=%d its square=%d\n", i , i*i);

Now,
i=4 
Is i<=5 true?
Yes, print this 
number=4 its square=16
using the statement printf("number=%d its square=%d\n", i , i*i);

Now,
i=5
Is i<=5 true?
Yes, print this 
number=5 its square=25
using the statement printf("number=%d its square=%d\n", i , i*i);

stop Now because the condition (i<=5) is achieved.

	Note: 

If the statement
printf("number=%d its square=%d\n", i , i*i);
is replaced by the statement: 
printf("\n number=%d/t its square=%d", i , i*i);
					
Then the output on the screen is:

number=1      its square=1
number=2     its square=4
number=3     its square=9
number=4     its square=16
number=5     its square=25

tab /t is included because to leave space between

number=1   and   its square=1

Suppose printf("number=%d its square=%d", a , a*a); is replaced by the statement: 
printf("number=%d\n its square=%d\n", a , a*a);

The output on the screen is:

number=1 
its square=1
number=2 
its square=4 
number=3 
its square=9 
number=4 
its square=16 
number=5 
its square=25 

And if you replace the printf statement:
printf("number=%d its square=%d", a , a*a); by the statement:
printf("number=%d\n, its square=%d\n", a , a*a);
i.e., if you place variable separator ( i.e., comma) between number=%d\n and its square=%d\n
Then the compilation error will be displayed on the screen.

	Write a program to print the first 10 numbers starting from one together with their squares and cubes?

Answer:

#include<stdio.h>
int main()
{
int i;
for( i=1; i<=10; i++)
printf("number=%d its square=%d its cube=%d\n", i , i*i, i*i*i);
return 0;
}

Program 4.0 

	C program to print the sum of two numbers using pointers

If we create an integer variable x by declaring the statement:
int x;
within the body of the main function int main() -- this variable is stored in the computer memory i.e., this variable occupies a specific location in the space of computer memory.
And this integer variable x is assigned an address (i.e., &x) to locate its position in the computer memory (like a house in the street is assigned an address to locate its position in the street). 
Pointers are the variables that represent the address of x in the computer memory i.e., p = &x, where &x imply the address of x in the computer memory and p is the pointer variable (which is the variable that represent the address of x in the computer memory).  
And further if you assign a value to the variable x by declaring the statement:
x=1;
within the body of the main function—this value is stored in the address of x in the computer memory. "*" denote pointer operator and *p denote the pointer  
(which represent the value stored in the address of x in the computer memory).

•	C program to print the address of x and the value assigned to x

#include <stdio.h>
int main()
{
int x, *p;
x = 1;
p = &x;
printf("The address of the variable x =%d", p);
printf("The value of the variable x =%d", *p);
return 0;
}

The output on the screen:
The address of the variable x = 0x7fffc60478a4
The value of the variable x = 1 
Since p = &x:
*p= *&x
The value of the variable x = 1 because you have assigned a value to the variable x by declaring the statement:
x=1;
within the body of the main function.

If the statements: 
printf("The address of the variable x =%d", p);
printf("The value of the variable x =%d", *p);
are replaced by the statement: 
printf("The address of the variable x =%d and its value =%d", p,*p);
i.e.,
#include <stdio.h>
int main()
{
int x, *p;
x=1;
p = &x;
printf("The address of the variable x =%d and its value =%d", p,*p);
return 0;
}
Then the output on the screen is:
The address of the variable x = 0x7fffc60478a4and its value = 1
									
#include <stdio.h>
int main()
{
int x, y, *p, *q, sum;
printf("Enter any number:");
scanf("%d", &x);
printf("Enter any number:");
scanf("%d", &y);
p = &x;
q = &y;
sum = *p + *q;
printf("Sum of entered numbers = %d\n", sum);
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 2
Enter any number:
If you enter the number 3
Sum of entered numbers = 5 will be outputted on the screen.

Since pointer *p imply the value assigned to the variable x (i.e., 2) through the keyboard and the pointer *q imply the value assigned to the variable y (i.e., 3) through the keyboard. Therefore:
sum = *p + *q = 2 + 3 = 5 (which will be outputted on the screen)

	C program to print the product, subtraction and division of two numbers using pointers

#include <stdio.h>
int main()
{
int x, y, *p, *q, product, subtract, div;
printf("Enter any number:");
scanf("%d", &x);
printf("Enter any number:");
scanf("%d", &y);
p = &x;
q = &y;
product = *p * *q;
subtract = *p - *q;
div= *p / *q;
printf("product of entered numbers = %d\n", product);
printf("subtract of entered numbers = %d\n", subtract);
printf("division of entered numbers = %d\n", div);
return 0;
}

The output on the screen:
Enter any number:
If you enter the number 4
Enter any number:
If you enter the number 2
product of entered numbers = 8
subtract of entered numbers = 2
division of entered numbers = 2
will be outputted on the screen.

	C program to find the greatest of two numbers using pointers

#include<stdio.h>
int main()
{
int x, y, *p, *q;
printf("Enter any integer:");
scanf("%d", &x);
printf("Enter any integer:");
scanf("%d", &y);
p = &x;
q = &y;
if(*p>*q)
{
printf("x is greater than y");
}
if(*q>*p)
{
printf("y is greater than x");
}
return 0;
}

The output on the screen:
Enter any integer:
If you enter the integer 10
Enter any integer:
If you enter the integer 16
y is greater than x will be outputted on the screen.

	What is the output of the following programs:

i)

#include <stdio.h>
int main()
{
int x;
x=12;
printf("per = %d%", x);
return 0;
}

Answer:
per=12

ii)

#include <stdio.h>
int main()
{
int x, t, c;
x =12;
t = 2;
c = x/t;
printf("velocity = %d m/s", c);
return 0;
}

Answer:
velocity = 6 m/s

Program 4.1 

	C program to print the sum of two numbers using functions

#include<stdio.h>
int addition(); 
int main()
{   
int answer; 
answer = addition(); 
printf("The sum of two numbers is: %d\n",answer);
return 0;
}

int addition() 
{
int x, y; 
printf("Enter any integer:");
scanf("%d", &x);
printf("Enter any integer:");
scanf("%d", &y);
return x+y;
}

The output on the screen:

Enter any integer:
If you enter the integer 3
Enter any integer:
If you enter the integer 5
sum of two numbers = 8 will be displayed on the screen.

int addition(); // the statement implies function declaration

int means integer and int addition() implies: addition() should return integer value.

int addition()// implies: the function to add the entered values (i.e., 3 and 5) and return the result (i.e., 3 + 5 i.e., 8) to the statement:
printf("sum of two numbers = %d", answer); to 
	make provision to display the output:
sum of two numbers = 8

{
int x, y; 
printf("Enter any integer:");
scanf("%d", &x);
printf("Enter any integer:");
scanf("%d", &y);
return x+y;
} // implies: the body of the function int addition()

answer = addition(); // implies: the function call i.e., this statement calls the function:
addition()
to add the entered values (i.e., 3 and 5) and return the result (i.e., 3 + 5 i.e., 8) 
to the statement:
printf("sum of two numbers = %d", answer);
to make provision to display the output:
sum of two numbers = 8
on the screen.

In the statement: 
printf("sum of two numbers=%d", answer);
the format string %d indicates that the value to be displayed at that point in the string i.e., after the statement:
sum of two numbers = 
needs to be taken from the result returned by the function int addition().

	C program to print the product of two numbers using functions

#include<stdio.h>
int multiplication(); 
int main()
{   
int answer; 
answer = multiplication(); 
printf("The product of two numbers is: %d\n",answer);
return 0;
}

int multiplication() 
{
int x, y; 
printf("Enter any integer:");
scanf("%d", &x);
printf("Enter any integer:");
scanf("%d", &y);
return x*y;
}

The output on the screen:
Enter any integer:
If you enter the integer 3
Enter any integer:
If you enter the integer 5
product of two numbers = 15 will be outputted on the screen.

	C program to print the greatest of two numbers using functions


#include<stdio.h>
int largest(); 
int main()
{   
int answer; 
answer = largest(); 
printf("The largest of two numbers is: %d\n",answer);
return 0;
}

int largest() 
{
int x, y; 
printf("Enter any integer:");
scanf("%d", &x);
printf("Enter any integer:");
scanf("%d", &y);
if(x>y)
return x;
if(y>x)
return y;
}

The output on the screen:
Enter any integer:
If you enter the integer 3
Enter any integer:
If you enter the integer 5
largest of two numbers= 5 will be outputted on the screen.

	C program to print the greatest of three numbers using functions

#include<stdio.h>
int largest(); 
int main()
{

int answer; 
answer = largest();  
printf("largest of three numbers=%d", answer);
return 0;
}
int largest()
{
int x, y, z;
printf("Enter any integer:");
scanf("%d", &x);
printf("Enter any integer:");
scanf("%d", &y);
printf("Enter any integer:");
scanf("%d", &z);

if(x>y&& x>z)
return x;
if(y>x&& y > z)
return y;
if(z>x && z>y)
return z;
}

The output on the screen:
Enter any integer:
If you enter the integer 3
Enter any integer:
If you enter the integer 5
Enter any integer:
If you enter the integer 10
largest of three numbers = 10 will be outputted on the screen.


	C program to print the square of the number using functions

#include<stdio.h>
int square(); 
int main()
{

int answer; 
answer = square();  

printf("square of the given number=%d", answer);
}
int square()
{
int x;
printf("Enter any integer:");
scanf("%d", &x);
return x*x;
}

The output on the screen is:
Enter any integer:
If you enter an integer 5
square of the number = 25 will be outputted on the screen.

	What is the output of the following program:

#include<stdio.h>
int main()
{
int x;
x=6;
printf("The address of x = %d", &x);
return 0;
}

Answer:
The address of x = -604171156
Program 4.2
Switch (case) allows to make decision from the number of choices i.e., from the number of cases

For example:

#include<stdio.h>
int main()
{
char ch;
printf("Enter any character:");
scanf("%c", &ch);
switch(ch)
{
case 'R':
printf("Red");
break;
case 'W':
printf("White");
break;
case 'Y':
printf("Yellow");
break;
case 'G':
printf("Green");
break;
default:
printf("Error");
break;
}
return 0;
}

The output on the screen:
Enter any character:
If you enter a character R
Red will be outputted on the screen.

switch(ch) allow to make decision from the number of choices i.e., from the number of cases 
case 'R':
case 'W':
case 'Y':
case 'G':

Since we have entered the character R (which corresponds to case 'R':)

The statement 
printf("Red");
is executed to display the output: 
Red
on the screen.

Suppose you enter a character K

Then the output on the screen is:
Error

(Entered character K does not correspond to any of the cases:
case 'R':
case 'W':
case 'Y':
case 'G':
Therefore the statement: 
printf("Error"); 
is executed to display the output: 
Error
on the screen).

If the statements:

case 'R':
printf("Red");
break;
case 'W':
printf("White");
break;
case 'Y':
printf("Yellow");
break;
case 'G':
printf("Green");
break;
default:
printf("Error");
break;

are replaced by the statements:

case 'R':
printf("Red");
case 'W':
printf("White");
case 'Y':
printf("Yellow");
break;
case 'G':
printf("Green");
break;
default:
printf("Error");
break;

Then the output on the screen is:
Red
White
Yellow
i.e., the output will be printed till yellow even though you have entered the character R.


Program 4.3

C program to print the output:

Element [0] = 16
Element [1] = 18
Element [2] = 20
Element [3] = 25
Element [4] = 36

using arrays: 

#include<stdio.h>
int main()
{
int i;
int num [5] = {16, 18, 20, 25, 36};
for(i=0; i<5; i++)
printf("\n Element [%d] = %d", i, num[i]);
return 0;
}

The output on the screen:

Element [0] = 16
Element [1] = 18
Element [2] = 20
Element [3] = 25
Element [4] = 36

The statement:
int num [5] = {16, 18, 20, 25, 36};
imply that we are creating an integer array (and the name of array is num) consisting of 5 values (i.e., 16, 18, 20, 25, 36) of the same data type int. 
The number of values between the braces { } cannot be larger than the number of values that we declare for the array between square brackets [ ]. 
There are 5 integers i.e., 16, 18, 20, 25, 36 within the braces { }, so 5 is written within the square brackets [ ]. 
If there were 6 integers i.e., 16, 18, 20, 25, 36, 42 within the braces { }, then 6 must be written within the square brackets [ ].

	Note: With the declaration int num [5], computer creates 5 memory cells with name num[0], num[1], num[2], num[3], num[4].
And since:
int num [5] = {16, 18, 20, 25, 36};
the values 16, 18, 20, 25, 36 are stored in num[0], num[1], num[2], num[3], num[4] respectively.

	How the execution takes its way through the for loop statement

i=0
Is i<5 true?
Yes, print this
Element [0] = 16
using the statement: 
printf("\n Element [%d] = %d", i, num[i])
format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=0) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[0] i.e., 16).

Now,
i=1
Is i<5 true?
Yes, print this
Element [1] = 18
using the statement: 
printf("\n Element [%d] = %d", i, num[i])
format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=1) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[1] i.e., 18).

Now,
i=2
Is i<5 true?
Yes, print this
Element [2] = 20

using the statement: 
printf("\n Element [%d] = %d", i, num[i])
format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=2) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[2] i.e., 20).

Now,
i=3
Is i<5 true?
Yes, print this
Element [3] = 25
using the statement:  
printf("\n Element [%d] = %d", i, num[i])
format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=3) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[3] i.e., 25).

Now,
i=4
Is i<5 true?
Yes, print this
Element [4] = 36
using the statement: 
printf("\n Element [%d] = %d", i, num[i])
Stop because the condition i<5 is achieved.
format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=4) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[4] i.e., 36).

Suppose the statement:
printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement: 
printf("\n Element [%d] = %d", i, num[0]);
Then the output on the screen:
Element [0] = 16
Element [1] = 16
Element [2] = 16
Element [3] = 16
Element [4] = 16

Suppose the statement:
printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement: 
printf("\n Element [%d] = %d", i, num[1]);

The output on the screen:
Element [0] = 18
Element [1] = 18
Element [2] = 18
Element [3] = 18
Element [4] = 18

Suppose the statement:
printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement: 
printf("\n Element [%d] = %d", i, num[2]);
The output on the screen:
Element [0] = 20
Element [1] = 20
Element [2] = 20
Element [3] = 20
Element [4] = 20

Suppose the statement:
printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement: 
printf("\n Element [%d] = %d", i, num[3]);
The output on the screen:
Element [0] = 25
Element [1] = 25
Element [2] = 25
Element [3] = 25
Element [4] = 25

Suppose the statement:
printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement: 
printf("\n Element [%d] = %d", i, num[4]);
The output on the screen:
Element [0] = 36
Element [1] = 36
Element [2] = 36
Element [3] = 36
Element [4] = 36

If the condition:
i<5 
is replaced by the condition:
i<=5
Then the output on the screen is:
Element [0] = 16
Element [1] = 18
Element [2] = 20
Element [3] = 25
Element [4] = 36
Element [5] = 3656
3656 is the number stored in the memory i.e., any number stored in the memory will be displayed.

If the statement:
int num [5] = {16, 18, 20, 25, 36}; is replaced by the statement:
				  int num [i] = {16, 18, 20, 25, 36};
Then the compilation will be displayed on the screen because there are 5 elements within the braces {} not i elements.

	Note:

	C program to print the sum of the elements in array.

#include<stdio.h>
int main()
{
int i, sum = 0;
int num [5] = {16, 18, 20, 25, 36};
for(i=0; i<5; i++)
sum = sum + num[i];
printf("Sum of the Elements in the array = %d", sum);
return 0;
}

The output on the screen:
Sum of the Elements in the array = 115
i.e., 16 + 18 + 20 + 25 + 36 = 115

	How the Execution takes its way through the for loop statement

i=0 (sum = 0)
Is i<5 true?
Yes, do this 
sum = sum + num[i] = sum + num[0] = 0 +16 =16

Now,
i=1 (sum = 16)
Is i<5 true?
Yes, do this 
sum = sum + num[i] = sum + num[1] = 16 +18 =34

Now,
i=2 (sum = 34)
Is i<5 true?
Yes, do this 
sum = sum + num[i]  = sum + num[2] = 34 +20 =54

Now,
i=3 (sum = 54)
Is i<5 true?
Yes, do this 
sum = sum + num[i] = sum + num[3] = 54 +25 =79

Now,
i=5 (sum = 79)
Is i<5 true?
Yes, do this 
sum = sum + num[i] = sum + num[5] = 79 + 36 =115
stop because the condition i<5 is achieved

The statement:
printf("Sum of the Elements in the array  = %d", sum); is executed to display the output:
Sum of the Elements in the array = 115 
on the screen.

If the statement: 
int i, sum = 0; 
is replaced by int i, sum = 1;
Then The output on the screen:
Sum of the Elements in the array = 116

	C program to print the average of the elements in array 

#include<stdio.h>
int main()
{
int i, avg, sum = 0;
int num [5] = {16, 18, 20, 25, 36};
for(i=0; i<5; i++)
sum = sum + num [i];
avg = sum/5;
printf("Sum of the Elements in the array = %d", sum);
printf("average of the elements in the array= %d", avg);
return 0;
}

The output on the screen:
Sum of the Elements in the array = 115
average of the elements in the array = 23

Write a program to print: 

Einstein [0] = E
Einstein [1] = I
Einstein [2] = N
Einstein [3] = S
Einstein [4] = T
Einstein [5] = E
Einstein [6] = I
Einstein [7] = N

using arrays

Answer:

#include<stdio.h>
int main()
{
int i;
char name [8] = {' E' , ' I', ' N', ' S', ' T ', ' E', ' I', ' N'};
for(i=0; i<8; i++)
printf("\n Element [%d] = %c", i, name[i]);
return 0;
}

	Note:

If the format string %d is used instead of %c i.e., if the statement: 
printf("\n Element [%d] = %c", name[i], name[i]); is written instead of the statement: 
printf("\n Element [%c] = %c", name[i], name[i]);
						
Then the output on the screen is:

Element [69] = E
Element [73] = I
Element [78] = N
Element [83] = S
Element [84] = T
Element [69] = E
Element [73] = I
Element [78] = N


	What will be the output of the following programs?

i)
#include <stdio.h>
#include <math.h>
int main()
{
printf("%f", cbrt(27));
return 0;
}

Answer:
3.000

ii)

#include <stdio.h>
int main()
{
char i;  
char body [4] = {'b', 'o', 'd', 'y'};
for(i=0; i<4; i++)
printf("\n body[%c] = %c", body[i] , body[i]);
return 0;
}

Answer:

body [b] = b
body [o] = o
body [d] = d
body [y] = y

iii)

#include <stdio.h>
#include <malloc.h>
int main()
{
int x=2;  
printf("%d", malloc ( 200*sizeof(x)));
return 0;
}

Answer:
8183824

	What is the mistake in the following program:

#include<stdio.h>
int main()
{
int i;
int num [] = {16, 18, 20, 25, 36};
for(i=0; i<5; i++)
printf("\n Element [%d] = %d", i, num[i]);
return 0;
}

Answer: There is no mistake in the above program. The output on the screen is:

Element [0] = 16
Element [1] = 18
Element [2] = 20
Element [3] = 25
Element [4] = 36

Program 4.3
C program to print the output:

Name of the book = B
Price of the book = 135.00
Number of pages = 300
Edition = 8

using structures 

#include<stdio.h>
int main()
{
struct book {
char name;
float price;
int pages;
int edition;
};

struct book b1;
b1.name = 'B';
b1.price = 135.00;
b1.pages = 300;
b1.edition = 8;
printf("\n Name of the book = %c", b1.name);
printf("\n Price of the book = %f", b1.price);
printf("\n Number of pages = %d", b1.pages);
printf("\n Edition of the book = %d", b1.edition);
return 0;
}

The output on the screen:

Name of the book = B
Price of the book = 135.00
Number of pages = 300
Edition of the book = 8

The statement:

struct book {
char name;
float price;
int pages;
int edition;
}; 

imply the structure definition i.e., we are defining a structure (and the data type name of the structure is book) and it consists of elements: 
name (which is of data type char), price (which is of data type float), pages (which is of data type int), edition (which is of data type int) – which are placed within the body of the structure. 

The statement: 
struct book b1;
imply the structure variable declaration (where b1 denote the structure variable)

	Why structure variable b1 is declared or defined?

In order to assign the values to the elements within the body of the structure,  each element must be linked with structure variable with dot operator or period operator or member accessibility operator. 
For example: name is the element which must be linked with structure variable b1 with dot operator to assign a value B to the element “name”.

format string %c (corresponding to the data type char) in the statement: 
printf("\n Name of the book = %c", b1.name);
indicates that the value to be displayed at that point in the string i.e., after the statement (\n Name of the book = ) needs to be taken from b1.name.

The statement: 
printf("\n Name of the book = %c", b1.name);
make provision to print the output:
Name of the book = B
on the screen.

format string %f (corresponding to the data type float) in the statement: 
printf("\n Price of the book = %f", b1.price);
indicates that the value to be displayed at that point in the string i.e., after the statement (\n Price of the book = ) needs to be taken from b1.price.

The statement: 
printf("\n Price of the book = %f", b1.price);
make provision to print the output:
Price of the book = 135.00
on the screen.

format string %d (corresponding to the data type int) in the statement: 
printf("\n Number of pages = %d", b1.pages);
indicates that the value to be displayed at that point in the string i.e., after the statement (\n Number of pages = ) needs to be taken from b1.pages.

The statement: 
printf("\n Number of pages = %d", b1.pages);
make provision to print the output:
Number of pages = 300
on the screen.

format string %d (corresponding to the data type int) in the statement: 
printf("\n Edition of the book = %d", b1.edition);
indicates that the value to be displayed at that point in the string i.e., after the statement (\n Edition of the book = ) needs to be taken from b1.edition.

The statement: 
printf("\n Edition of the book = %d", b1.edition);
make provision to print the output:
Edition of the book = 8
on the screen.

	What will be output of the following programs?

A)

#include<stdio.h>
struct book {
char name;
float price;
int pages;
int edition;
};
int main()
{ 
struct book b1;
b1.name = 'B';
b1.price = 135.00;
b1.pages = 300;
b1.edition = 8;
printf("\n Name of the book = %c", b1.name);
printf("\n Price of the book = %f", b1.price);
printf("\n Number of pages = %d", b1.pages);
printf("\n Edition of the book = %d", b1.edition);
}

Answer:

Name of the book = B
Price of the book = 135.000000
Number of pages = 300
Edition of the book = 8

B)

#include <stdio.h>
int main(){

for( ; ; ) {
printf("This loop will run forever.\n");
}
return 0;
}

Answer:

This loop will run forever.
This loop will run forever.
This loop will run forever.
This loop will run forever.
This loop will run forever.
This loop will run forever. ......... continues

C) 

#include<stdio.h>
int main()
{
char  ch [5];
printf( "Enter the name: ");
scanf("%s", &ch);
printf( "the name you entered = %s", ch);
return 0;
}

Answer:

Enter the name:
If you enter the name Dennis
the name you entered = Denni will be outputted on the screen.

Instead of Dennis, only Denni will be displayed on the screen because of the statement char  ch [5];

The statement: 
char  ch [5];
make provision only for 5 lettered name to be displayed on the screen.

If the statement:
char  ch [5]; is replaced by the statement char  ch [6];
Then the output on the screen is:
Enter the name:
If you enter the name Dennis
the name you entered = Dennis will be outputted on the screen.

Note: %s implies the format specifier for string.

Program 4.4
Continue and break statements: 

i) 

#include <stdio.h>
int main()
{
int i;
for (i=1; i<=5; i++)
{
if (i==3)
{
continue;
}

printf("%d\n ", i);
}
return 0;
}

Output on the screen:

1
2
4
5

	Note:

i = 1
Is the condition (i<=5) is true?
Yes because i=1
The statement printf("%d\n ", i); is executed to print the output:
1
Now, the value of i is:
i =  1+1 = 2
Is the condition (i<=5) is true?
Yes because i=2
The statement printf("%d\n ", i); is executed to print the output:
2
Now, the value of i is:
i =  2+1 = 3
Is the condition (i<=5) is true?
Yes because i=3
The statement printf("%d\n ", i); is not executed to print the output:
3
Because of the statement:

if (i==3)
{
continue;
}

//  Execution skips  //

Now, the value of i is:
i =  3+1 = 4
Is the condition (i<=5) is true?
Yes because i=4
The statement printf("%d\n ", i); is executed to print the output:
4
Now, the value of i is:
i =  4+1 = 5
Is the condition (i<=5) is true?
Yes because i=5
The statement printf("%d\n ", i);  is executed to print the output:
5
and stop because the condition i<=5 is achieved.

ii) 

#include <stdio.h>
int main()
{
int i;
for (i=1; i<=5; i++)
{
if (i==3)
{
break;
}

printf("%d\n ", i);
}
return 0; 
}

Output on the screen:

1
2

	Note:
i = 1
Is the condition (i<=5) is true?
Yes because i=1
The statement printf("%d\n ", i); is executed to print the output:
1
Now, the value of i is:
i =  1+1 = 2
Is the condition (i<=5) is true?
Yes because i=2
The statement printf("%d\n ", i); is executed to print the output:
2
Now, the value of i is:
i =  2+1 = 3
Is the condition (i<=5) is true?
Yes because i=3
The statement printf("%d\n ", i); is not executed to print the output:

Because of the statement:

if (i==3)
{
break;
}

The for loop:
for (i=1; i<=5; i++)

is immediately terminated (even before the condition i<=5 is achieved) and program execution stops.

//---------------------------------------------------------------------------------------------------------------------------------

The goto statement:

#include <stdio.h>
int main()
{
int i;
for(i=1;i<=5;i++)
{
if(i==3)
{
goto HAI;
}
printf("\n %d ",i);
}

HAI : printf("\n Linux");
}

Output on the screen:

1
2
Linux


	Note:

i = 1
Is the condition (i<=5) is true?
Yes because i=1
The statement printf("\n %d ",i); is executed to print the output:
1
Now, the value of i is:
i =  1+1 = 2
Is the condition (i<=5) is true?
Yes because i=2
The statement printf("\n %d ",i); is executed to print the output:
2
Now, the value of i is:
i =  2+1 = 3
Is the condition (i<=5) is true?
Yes because i=3
The statement printf("%d\n ", i); is not executed to print the output:
3

Rather
The statement printf("\n Linux"); is executed to print the output:

Linux
Because of the statement:

if(i==3)
{
goto HAI;
}

The for loop:
for (i=1; i<=5; i++)

is immediately terminated (even before the condition i<=5 is achieved) and program execution stops.

---------------------------------------------------------------------------------------------------------------------------//
Program 4.5
C program to convert the upper case letter to lower case letter

#include<stdio.h>
int main()
{
char ch = 'A';
char b = tolower(ch);
printf("upper case letter %c is converted to lower case letter %c", ch, b);
return 0;
}

Output on the screen:
upper case letter A is converted to lower case letter a

If you want to enter the character through the keyboard, then the above program should take the form:

#include<stdio.h>
int main()
{
char ch;
printf("Enter any character:");
scanf("%c", &ch);
char b = tolower(ch);
printf("upper case letter %c is converted to lower case letter %c", ch, b);
return 0;
}

Output on the screen:
Enter any character:
If you enter the character C
upper case letter C is converted to lower case letter c will be outputted on the screen.

Program 4.6 
C program to convert the lower case letter to upper case letter

#include<stdio.h>
int main()
{
char ch = 'a';
char b = toupper(ch);
printf("lower case letter %c is converted to upper case letter %c", ch, b);
return 0;
}

Output on the screen:
lower case letter a is converted to upper case letter A
							
If you want to enter the character through the keyboard, then the above program should take the form:

#include<stdio.h>
int main()
{
char ch;
printf("Enter any character:");
scanf("%c", &ch);
char b = toupper(ch);
printf("lower case letter %c is converted to upper case letter %c", ch, b);
return 0;
}

Output on the screen:
Enter any character:
If you enter the character h
lower case letter h is converted to upper case letter H will be outputted on the screen.

Program 4.7
C program to test whether the entered character is upper case letter or not

#include<stdio.h>
int main()
{
char ch = 'a';
if(isupper(ch))
printf("you have entered the upper case letter");
else
printf("you have entered the lower case letter");
return 0;
}

Output on the screen:
you have entered the lower case letter

If the statement:
char ch = 'a'; is replaced by the statement:
char ch = 'A';
Then the output on the screen is:
you have entered the upper case letter

Program 4.8

C program to test whether the entered character is lower case letter or not

#include<stdio.h>
int main()
{
char ch = 'a';
if(islower(ch))
printf("you have entered the lower case letter");
else
printf("you have entered the upper case letter");
return 0;
}

Output on the screen:
you have entered the lower case letter

Program 4.9
C program to print the value of tan inverse x (i.e., the value of tan-1x)

#include<stdio.h>
#include<math.h>
int main()
{
int x = 20;
printf("the value of tan inverse x = %f", atan(x));
return 0;
}

Output on the screen:
the value of tan inverse x = 1.520838

Program 5.0

C program to print the value of tan inverse x/y (i.e., the value of tan-1x/y)

#include<stdio.h>
#include<math.h>
int main()
{
int x,y;
x = 20;
y =20;
printf("the value of tan inverse x/y = %f",  atan2(x,y));
return 0;
}

Output on the screen:
the value of tan inverse x/y = 0.785398

Program 5.1
C program to print the value of fmod(x, y)

#include<stdio.h>
#include<math.h>
int main()
{
float x = 20.500000;
float y =20.799999;
printf("the remainder of %f divided by %f is %f", x, y, fmod(x,y));
return 0;
}

Output on the screen:
the remainder of 20.500000 divided by 20.799999 is 20.500000


Program 5.2
C program to print the value of ~x

#include<stdio.h>
int main()
{
int x, y;
x = 205;
y=~x;
printf("the value of y is:%d", y);
return 0;
}

Output on the screen:
the value of y is:-206
										
If the statement:
y=~x; is replaced by the statement:
y= -(~x);

Then the output on the screen is:
the value of y is: 206

Program 5.3

C program to print the ASCII (American Standard Code for Information Interchange) value of the entered character

#include<stdio.h>
int main()
{
char ch ='A';
printf("the ASCII value of ch is: %d", ch);
return 0;
}

Output on the screen:
the ASCII value of ch is: 65
								
If the statement:
printf("the ASCII value of ch is: %d", ch);
is replaced by the statement:
printf("the ASCII value of ch is: %c", ch);

Then the output on the screen is:
the ASCII value of ch is: A


	What will be the output of the following programs:

i)

#include<stdio.h>
int main()
{
int i;
int num [5] ={16,18,19,20,21};
for(i=0;i<5;i++)
printf("\n Element = %d", num[i] +1);
return 0;
}

Answer:

Element = 17
Element = 19
Element = 20
Element = 21
Element = 22

ii)

#include<stdio.h>
int main()
{
int i = 54;
int y = i<<1;
printf("The value of y = %d", y);
return 0;
}

Answer:
The value of y = 108
							
If the statement:
i<<1 is replaced by the statement: i<<2
Then the output on the screen is:
The value of y = 216

	Note:

i<<1 implies 54 * 2 = 108
i<<2 implies 54 * 4 = 216
i<<3 implies 54 * 6 = 324
i<<4 implies 54 * 8 = 432

iii)

#include<stdio.h>
int main()
{
int i = 54;
int y = i>>1;
printf("The value of y = %d", y);
return 0;
}

Answer:
The value of y = 27

If the statement:
i>>1 is replaced by the statement: i>>2
Then the output on the screen is:
The value of y = 13

	Note:
i>>1 implies 54 / 2 = 27
i>>2 implies 54 / 4 = 13
i>>3 implies 54 / 6 = 9
i>>4 implies 54 / 8 = 6

<< implies: left shift operator 
		>> implies: right shift operator 

Program 5.4

C program to print the length of the entered character (i.e., to print the length of the string)

#include<stdio.h>
#include<string.h>
int main()
{
char ch[4];
printf("Enter any word: ");
scanf("%c", &ch);
printf("The length of the string = %d", strlen(ch));
return 0;
}

Output on the screen:
Enter any word:
If you enter the word dog
The length of the string = 3
	will be displayed on the console screen because there are three letters in the word dog.

Suppose if you enter the word tech
The length of the string = 4
	will be displayed on the console screen because there are four letters in the word tech.

Program 5.5
C program to print the factorial of the entered number

#include<stdio.h>
int main()
{
int i, n, fact=1 ;
printf("Enter any number:");
scanf("%d", &n);
for(i=1; i<=n; i++)
fact = fact *i;
printf("\n Entered number is: %d", n);
printf("\n The factorial of the entered number %d is: %d", n, fact);
return 0;
}

Output on the screen:
Enter any number:
If you enter the number 2
Entered number is: 2
The factorial of the entered number 2 is: 2
will be displayed on the screen.

Suppose if you enter the number 4
Entered number is: 4
The factorial of the entered number 4 is: 24
will be displayed on the screen.
				
	What will be the output of the following program:

#include <stdio.h>
int main()
{
printf("\nLinux \' linux ");
printf("\nLinux \? linux ");
return0;
}

Answer:
Linux ' linux
Linux ? linux

#include<stdio.h>
#include<stdlib.h>
int main () {
printf("linux\n");
exit (0);
printf("php\n");
return 0;
}

Answer:
linux

Note: exit(0) is useful for terminating a program upon having discovered some error which prevents the program from continuing to execute normally. The header file for exit (0); is stdlib.h.
