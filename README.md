<p><strong>C Programming</strong></p>
<ul>
<li>A High Level Programming Language (which uses alphabets, digits, punctuations and some special symbols and cannot be executed directly without being converted into machine level language (the language which uses only 0 and 1))</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>developed by a man named Dennis Ritchie</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li>in 1970s at Bell Telephone laboratories (now named AT &amp; T Bell laboratories), Murray Hill, New Jersey</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>to develop the UNIX operating system.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>using the two early programming languages -- Basic Combined Programming Language (BCPL) and BASIC (Beginner's All-purpose Symbolic Instruction Code) language</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>Uses: used in the development of a) operating systems like LINUX, UNIX&nbsp; b) embedded systems like ATMs, printers.Most of the state-of-the-art software have been developed using C.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>Advantages: relatively simple language, reliable (able to be trusted), easy to understand, easy to use, write, modify and debug and quick to learn.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>MYSQLDatabase, LINUX Drivers, Text Editors are written in C.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>C is called a structured programming language because it divides the problem into smaller modules called functions or procedures each of which handles a particular responsibility. Hence it is simple and easy to understand and well sited for small size implementation. However this is not restricted. A large size implementation is possible but complex design and full object oriented design cannot be implemented (because complex design concepts like Polymorphism and inheritance are not available in C).</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>A Simple C program basically comprises of the following parts:</li>
</ul>
<ul>
<li>Preprocessor Commands</li>
<li>Functions</li>
<li>Variables</li>
<li>Statements &amp; Expressions</li>
<li>Comments</li>
</ul>
<p>// -------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>/* My First C Program&nbsp; */&nbsp;&nbsp; Comment</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt; // preprocessor command</p>
<p>int main() // Function where the program execution begins.</p>
<p>{</p>
<p>printf("Hello,world!"); // statement</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>-------------------------------------------------------------------------------------&nbsp; //</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Process of C Program Execution: A C program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello,world!");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is written using Text Editor , such as [ Notepad (in case of Windows Operating System), vim or vi (in case of Linux Operating System)] and saved with [.C] Extension.</p>
<p>File Saved with [.C] extension is called Source Program or Source Code.</p>
<p>C Source code with [.C] Extension is sent to preprocessor first.</p>
<p>The preprocessor generates an expanded source code:</p>
<p>&nbsp;</p>
<p>// ----------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>The contents of &lt;stdio.h&gt; would be pasted at the location of #include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello,world!");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>------------------------------------------------------------------------------------------------------&nbsp; //</p>
<p>&nbsp;</p>
<ul>
<li>Expanded source code is given as input to compiler where the expanded source program is compiled (i.e., the program is entirely read and translated to instructions the computer can understand i.e., machine understandable / readable language i.e., to machine code sequence of 0s and 1s). If the C compiler finds any error during compilation, it provides information about the error to the programmer.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>The programmer has to review code and re-edit the program. After re-editing program, Compiler again check for any error.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>If program is error-free then it is sent to assembler (where the code is assembled and converted into object code. Now a simple.obj file is generated).</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>The object code is sent to linker (where the object code is linked with appropriate libraries). Then it is converted into a single executable code. A simple.exe file is generated.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>The executable code is sent to loader (where the executable code is loaded into memory and then it is executed).</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>After execution, output:</li>
</ul>
<p>Hello,world!</p>
<p>is displayed on the console screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>C is <strong>case sensitive language</strong>: only lower case letters (or small letters) must be used.&nbsp;</p>
<p>&nbsp;</p>
<p>Capital letters (or upper case letters) must be avoided to prevent the display of error on the screen</p>
<p>(For example: If the statement PRINTF("Hello,world!"); is written instead of printf("Hello,world!");</p>
<p>or INT MAIN() is written instead of int main(), compilation Error will be displayed on the console screen).</p>
<p>&nbsp;</p>
<p>Parentheses () indicate a function and the word main indicate the name of the function.</p>
<p>main() implies: main function</p>
<p>&nbsp;</p>
<p>And if we forget to end each statement within the body of the main function with a semicolon (;), then the compilation Error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>There should be no space between main and the parentheses ()</p>
<p>&nbsp;</p>
<p>i.e., int main()</p>
<p>&nbsp;</p>
<p>and there should be no space inside the parentheses ()</p>
<p>&nbsp;</p>
<p>i.e., int main()</p>
<p>&nbsp;</p>
<p>to prevent the display of compilation error on the screen.</p>
<p>&nbsp;</p>
<p>As we know C is Platform dependent language. So the Operating system needs to know when the program execution ends.</p>
<p>&nbsp;</p>
<p>So when there is value returns from the main function</p>
<p>the Operating System get to know that the program execution is over.</p>
<p>int main () implies: main() should return integer value.</p>
<p>&nbsp;</p>
<ul>
<li>If the main function returns 0 to the operating system, then the</li>
</ul>
<p>program has completed execution successfully.</p>
<p>&nbsp;</p>
<ul>
<li>If the main function returns 1 to the operating system, then the</li>
</ul>
<p>program has not completed execution successfully.</p>
<p>&nbsp;</p>
<p>The statement</p>
<p><strong>#include&lt;stdio.h&gt;</strong></p>
<p>tells the compiler to include the text from the file stdio.h (which is already present in the operating system) before it translates or compiles the program into a sequence of 0s and 1s.</p>
<p>&nbsp;</p>
<ul>
<li>stdio means standard input output and stdio.h means standard input output header file (printf() &amp; scanf() are not part of the C language, because there is no input or output defined in C language itself-- stdio.h comprises standard input output functions like scanf, printf etc.</li>
<li>and allows standard input /output operations -- note: scanf is an input function and printf is an output function (note: Letter f denote formatted) and it is included into the C program by writing the statement <strong>#include &lt;stdio.h&gt;</strong>).</li>
<li>If a program is written without the statement:</li>
</ul>
<p><strong>#include&lt;stdio.h&gt;</strong>, then the C compiler can't compile and a compilation error is displayed on the screen (because C compiler fails to recognize the functions such as printf() and scanf()).</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> We can also write <strong>#include "stdio.h"</strong> instead of <strong>#include &lt;stdio.h&gt;</strong> but some online compilers will flag error message. So the statement <strong>#include &lt;stdio.h&gt;</strong> is generally preferred and the statement #include "stdio.h" is generally ignored.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>main() </strong>&rarr;&nbsp; The program begins its execution with the function main() -- which is called the user defined function (because this function is defined by the user) - the main function -- the entry point of the program execution i.e., the point from where the execution of C program begins and the point at which the operating system passes control of&nbsp; the computer over to that program.</p>
<p>&nbsp;</p>
<p><strong>int main()</strong> {</p>
<p>} &rarr; implies body of the main function within which the sequence of instructions in the form of statements</p>
<p>i.e., the program&nbsp; is written and executed. The left curly brace</p>
<p>{</p>
<p>implies: the beginning of the main function</p>
<p>and the right curly brace</p>
<p>}</p>
<p>implies: the end of the main function.</p>
<p>&nbsp;</p>
<p><strong>return 0;</strong> &rarr; implies the exit status of execution of the program i.e., at this point,</p>
<p>main function returns back the control of the computer to the operating system since</p>
<p>the execution is terminated at this point and once a return statement</p>
<p>i.e., return 0; is executed, no further instructions within the main function are executed</p>
<p>&nbsp;</p>
<p>For example:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello,world!");</p>
<p>return 0;</p>
<p>printf("Hello,world!");</p>
<p>}</p>
<p>&nbsp;</p>
<p>Output on the screen:</p>
<p>Hello,world!</p>
<p>&nbsp;</p>
<p><strong>;</strong> &rarr; implies semicolon or statement terminator &rarr; A program is a well-defined set of instructions and each well-defined instruction (in the form of a statement) is ended by a semicolon (which is C language punctuation -- like a period in English i.e., in an English paragraph each sentence is ended by a full stop which tells that one sentence ends and another begins, semicolon implies the end of one logical entity -- that one instruction (or statement) ends and another begins).</p>
<p><strong>&nbsp;</strong></p>
<p><strong>printf()</strong>&rarr; output function of the C language which makes provision to print the output:</p>
<p>&nbsp;</p>
<p>Hello,world!</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>on the screen. Parentheses () indicate a function and the word printf indicate the name of the function.</p>
<p>&nbsp;</p>
<p>The text</p>
<p>Hello,world!</p>
<p>should be enclosed by the double quotation marks ("") and should be written within the printf function and this</p>
<p>printf function should be ended with the semicolon i.e.,</p>
<p>printf("Hello,world!");</p>
<p>otherwise the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 1.1</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print the word "hello Bill Gates" on screen</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("hello Bill Gates");</p>
<p>return 0;</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>hello Bill Gates</p>
<p>&nbsp;</p>
<p><strong>Program 1.2</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print </strong></p>
<p><strong>*</strong></p>
<p><strong>*****</strong></p>
<p><strong>*****</strong></p>
<p><strong>*****</strong></p>
<p><strong>*****</strong></p>
<p><strong>on screen</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>printf("\n&nbsp; ***** ");</p>
<p>printf("\n&nbsp; ***** ");</p>
<p>printf("\n&nbsp; ***** ");</p>
<p>printf("\n&nbsp; ***** ");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>If new line sequence (\n)&nbsp; is not included in the above program then the output on the screen is:</p>
<p>&nbsp;</p>
<p>*********************</p>
<p>In the above code, the new line character has the ASCII value of 10 which means it is a new line. The author has put the ASCII values table for different characters that can be used in the programs to solve real time problems.</p>
<ul>
<li><strong>Write a program to print the following outputs:</strong></li>
</ul>
<p>&nbsp;</p>
<p>(a)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>&nbsp;</p>
<p>*</p>
<p>****</p>
<p>*******</p>
<p>****</p>
<p>*</p>
<p>(b)</p>
<p>&nbsp;</p>
<p>****************</p>
<p>* *</p>
<p>* Hello World! *</p>
<p>* *</p>
<p>****************</p>
<p>&nbsp;</p>
<p>(c)</p>
<p>&nbsp;</p>
<p>Braces come in pairs!</p>
<p>Comments come in pairs!</p>
<p>All statements end with a semicolon!</p>
<p>Spaces are optional!</p>
<p>Must have a main function!</p>
<p>C is done mostly in lowercase. It's a case-sensitive language</p>
<p>&nbsp;</p>
<p><strong>Answers:</strong></p>
<p>&nbsp;</p>
<p>(a)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****&nbsp; ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ******* ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****&nbsp;&nbsp;&nbsp; ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>(b)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****************&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * Hello World! *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");&nbsp;&nbsp;&nbsp;</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>printf("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****************&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>(c)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("\n Braces come in pairs!");</p>
<p>printf("\n Comments come in pairs!");</p>
<p>printf("\n&nbsp; All statements end with a semicolon!");</p>
<p>printf("\n&nbsp; Spaces are optional!");</p>
<p>printf("\n Must have a main function!");</p>
<p>printf("\n C is done mostly in lowercase. It's a case-sensitive language");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 1.3</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to find the area of a circle </strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int r, area;</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>printf("The area of the circle = %d", area);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>The area of the circle = 50</p>
<p>&nbsp;</p>
<p>int means the data type (an attribute that tells what kind of data that value can own) is integer and the storage size of int data type is 2 or 4 or 8 byte.</p>
<p><strong>Note:</strong></p>
<ul>
<li>A string, for example, is a data type that is used to categorize text and an integer is a data type used to categorize whole numbers / non fractional values.</li>
<li>We can't store decimal values using int data type.</li>
<li>If we use int data type to store decimal values, decimal values will be shortened and we will get only whole number. In this case, float data type can be used to store decimal values in a variable.</li>
</ul>
<p>&nbsp;</p>
<p>The statement</p>
<p>int r, area;</p>
<p>imply that we are creating the integer variables r , area.</p>
<p>Equal sign (" = ") implies storage operator.</p>
<p>&nbsp;</p>
<p>The statements</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>imply that we are storing the values to the created variables (i.e., we are storing the value 2 for r</p>
<p>and 4 * 3.14 * r * r = 4 * 3.14 * 2 * 2 = 50 for area).</p>
<p>&nbsp;</p>
<p>Comma in the statement</p>
<p>int r, area;</p>
<p>imply variable separator.</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>printf("The area of the circle = %d", area);</p>
<p>make provision to print the output:</p>
<p><strong>The area of the circle = 50</strong></p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>In the statement</p>
<p>printf("The area of the circle = %d", area);</p>
<p>format string or format specifier %d indicates that the integer value to be displayed after the statement</p>
<p>The area of the circle =</p>
<p>enclosed by double quotes needs to be taken from a variable area.</p>
<p>&nbsp;</p>
<p>The area of the circle is 50. 24 (for r = 2) but The area of the circle = 50 is displayed on the screen</p>
<p>because data type int is used instead of float and format specifier %d is used instead of %f.</p>
<p>&nbsp;</p>
<p>If float r, area; is used instead of int r, area;</p>
<p>and</p>
<p>If the statement</p>
<p>printf("The area of the circle = %f", area);</p>
<p>is written instead of</p>
<p>printf("The area of the circle = %d", area);</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float r, area;</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>printf("The area of the circle = %f", area);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the output on the screen:</p>
<p>The area of the circle = 50.24</p>
<p>&nbsp;</p>
<p>float means the data type is float.</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>float r, area;</p>
<p>imply that we are creating the floating variables r, area.</p>
<p>&nbsp;</p>
<p>(floating point variable means fractional variable or decimal number (for example: 1.5, 2.5, 3.5, 4.7 &hellip; etc.) whereas integer means non-fractional variable or whole number (for example: 1, 2, 3, 4 &hellip; etc.))</p>
<p>&nbsp;</p>
<p>data type float is used instead of int (and format string %f is used instead of %d) because if the data type int is used instead of float then the result will not be clearly outputted i.e., instead of 50.24 the computer displays only 50.</p>
<p>&nbsp;</p>
<p>If the statement</p>
<p>printf("The area of the circle = %2f", area);</p>
<p>is written instead of the statement</p>
<p>printf("The area of the circle = %f", area);</p>
<p>Then the output on the screen is:</p>
<p>The area of the circle =&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 50.24</p>
<p>i.e., the statement</p>
<p>&nbsp;</p>
<p>printf("The area of the circle = %f", area); yields the output:</p>
<p>&nbsp;</p>
<p>The area of the circle = 50.24</p>
<p>whereas the statement</p>
<p>printf("The area of the circle = %2f", area); yields the output:</p>
<p>&nbsp;</p>
<p>The area of the circle =&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 50.24</p>
<p>&nbsp;</p>
<p>If you want to supply the value for r through the key board, then the statement</p>
<p>&nbsp;</p>
<p>r =2;</p>
<p>should be replaced by the statements</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;r);</p>
<p>&nbsp;</p>
<p>i.e., the program should be rewritten as:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float r, area;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;r);</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>printf("The area of the circle = %f", area);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>The area of the circle = 50.24 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>float r, area;</p>
<p>imply that we are creating the float variables r and area and these variables are stored in the computer memory and they are assigned an address to locate their position in the computer memory (like houses in a street are assigned an address to locate their position in the street).</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>printf("Enter any number:");</p>
<p>make provision to print the text</p>
<p>Enter any number:</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>scanf("%d", &amp;r);</p>
<p>make provision to enter a number for r through the keyboard and store the number entered for r through the keyboard in the address of r in the computer memory. &amp; symbol imply the address and &amp;r imply the address of r in the computer memory.</p>
<p>&nbsp;</p>
<p>Format string %d in the statement scanf("%d", &amp;r); tells the input function scanf to read the number entered through the keyboard (which is a integer) and since "%d" is followed by , &amp;r&nbsp; ---&nbsp; %d tells the scanf function to read the integer entered through the keyboard for r&nbsp; and store it in the address of r in the computer memory (i.e., store the number in &amp;r).</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>As told earlier: when you enter an integer for r through the keyboard, this integer will be stored in the computer memory. If you want to know the storage size of the integer&nbsp; in computer memory (i.e., space occupied by the entered integer in the computer memory), you need to appeal to the following program:</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int r;</p>
<p>r=10;</p>
<p>printf("size of r = %d", sizeof(r));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>size of r = 4</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>i.e., integer entered for r i.e., 10 has occupied a space of 4 bytes in the computer memory.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the circumference of the circle (given r = 2.5)</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float r, area;</p>
<p>r = 2.5;</p>
<p>circumference = 3.14 * r * r;</p>
<p>printf("The circumference of the circle = %f", circumference);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the area of the rectangle (given l = 2.5 and b = 3)</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float l, b, area;</p>
<p>l = 2.5;</p>
<p>b = 3;</p>
<p>area = 1*b;</p>
<p>printf("The area of the rectangle = %f", area);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Format Specifiers in C </strong></p>
<p>&nbsp;</p>
<table width="204">
<tbody>
<tr>
<td width="78">
<p><strong>Data Type</strong></p>
</td>
<td width="126">
<p><strong>Format Specifier</strong></p>
</td>
</tr>
<tr>
<td width="78">
<p>int</p>
</td>
<td width="126">
<p>%d</p>
</td>
</tr>
<tr>
<td width="78">
<p>float</p>
</td>
<td width="126">
<p>%f or %e</p>
</td>
</tr>
<tr>
<td width="78">
<p>char</p>
</td>
<td width="126">
<p>%c</p>
</td>
</tr>
<tr>
<td width="78">
<p>double</p>
</td>
<td width="126">
<p>%lf or %le</p>
</td>
</tr>
<tr>
<td width="78">
<p>long int</p>
</td>
<td width="126">
<p>%ld</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><strong>Program 1.3</strong></p>
<p><strong>C program to find the sum of two numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, sum;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>sum = a + b;</p>
<p>printf("the sum of a and b = %d", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the sum of a and b = 3</p>
<p>&nbsp;</p>
<p>If you want to assign the floating point values i.e., fractional numbers for a &amp; b (i.e., 1.5 for a &amp;&nbsp; 2.6 for b) through the keyboard,</p>
<p>then the statement</p>
<p>int a, b, sum;</p>
<p>should be replaced by the statement</p>
<p>float a, b, sum;</p>
<p>and the statement</p>
<p>printf("the sum of a and b = %d", sum); should be replaced by the statement</p>
<p>&nbsp;</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float a, b, sum;</p>
<p>a=1.5;</p>
<p>b=2.6;</p>
<p>sum = a + b;</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>return 0;</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>the sum of a and b = 4.1</p>
<p>The statement</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>make provision to print the output:</p>
<p>the sum of a and b = 4.1</p>
<p>In the statement</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>format string %f tells the printf function to print a floating point value which is sum.</p>
<p>Since a = 1.5 and b = 2.6 therefore:</p>
<p>&nbsp;</p>
<p>the sum of a and b = 1.5 + 2.6 = 4.1 which is outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the statement</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>is replaced by the statement</p>
<p>printf("the sum of a and b = %f, sum");</p>
<p>Then output on the screen is:</p>
<p>the sum of a and b = %f, sum</p>
<p>&nbsp;</p>
<p>And if the statement printf("the sum of a and b = %f", sum); is omitted from the C program,</p>
<p>then the program will be successfully executed but there will be no display of the output on the screen.</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then the statements</p>
<p>&nbsp;</p>
<p>a=1.5;</p>
<p>b=2.6;</p>
<p>&nbsp;</p>
<p>should be replaced by the statements</p>
<p>&nbsp;</p>
<p>printf("Enter any two numbers:");</p>
<p>scanf("%f %f", &amp;a, &amp;b);</p>
<p>&nbsp;</p>
<p>i.e., the program should be rewritten as:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float a, b, sum;</p>
<p>printf("Enter any two numbers:");</p>
<p>scanf("%f %f", &amp;a, &amp;b);</p>
<p>sum = a+ b;</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two numbers:</p>
<p>If you enter two numbers 2.9 &amp; 3.6</p>
<p>the sum of a and b = 6.5 will be outputted on the screen with trailing zero&rsquo;s to fill up memory.</p>
<p>&nbsp;</p>
<ul>
<li><strong>As Said Earlier:</strong></li>
</ul>
<p>&nbsp;</p>
<p>ampersand ("&amp;") imply the address and &amp;a and &amp;b imply the addresses of the created float variables a and b stored in the computer memory&nbsp; i.e., when we enter a number for a and b through the keyboard, these numbers are read by scanf() function and they are stored in the computer memory (i.e., the number entered for a is stored in the address of a (i.e., stored in &amp;a)&nbsp; and the number entered for b is stored in the address of b (i.e., stored in &amp;b)).</p>
<p>&nbsp;</p>
<p>There are 2 format strings in the statement</p>
<p>scanf("%f %f", &amp;a, &amp;b);</p>
<ul>
<li>one format string %f corresponds to &amp;a i.e., %f tells the scanf() function to read the number entered through the keyboard for a and store it in the address of a in the computer memory.</li>
<li>and the other format string %f corresponds to &amp;b i.e., %f tells the scanf() function to read the number entered through the keyboard for b and store it in the address of b in the computer memory.</li>
</ul>
<p>&nbsp;</p>
<p>If the two format strings are separated by a comma i.e.,</p>
<p>scanf("%f, %f", &amp;a, &amp;b);</p>
<p>Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>The statement printf("Enter any two numbers:"); make provision to print</p>
<p>Enter any two numbers:</p>
<p>on the screen and the statement scanf("%f %f", &amp;a, &amp;b); read the two numbers 2.9 and 3.6 entered through the keyboard and store them in the computer memory.</p>
<p>&nbsp;</p>
<p>If the statements</p>
<p>&nbsp;</p>
<p>printf("Enter any two numbers:");</p>
<p>scanf("%f %f", &amp;a, &amp;b);</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%f", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%f", &amp;b);</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float a, b, sum;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%f", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%f", &amp;b);</p>
<p>sum = a+ b;</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter any number:</p>
<p>If you enter a number 2.9</p>
<p>Enter any number:</p>
<p>If you enter a number 3.6</p>
<p>the sum of a and b = 6.5 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the statement</p>
<p>printf("the sum of a and b = %f", sum);</p>
<p>is replaced by the statement</p>
<p>printf("the sum of %f and %f = %f", a, b, sum);</p>
<p>Then the output on the screen is:</p>
<p>the sum of 2.9 and 3.6 = 6.5</p>
<p>&nbsp;</p>
<p>In the statement</p>
<p>printf("the sum of %f and %f = %f", a, b, sum);</p>
<p>there are three format strings:</p>
<ul>
<li>The format string %f after the statement (the sum of) indicates that the value to be displayed needs to be taken from a variable a.</li>
<li>The format string %f after the statement (the sum of %f and) indicates that the value to be displayed needs to be taken from a variable b.</li>
<li>The format string %f after the statement (the sum of %f and %f = ) indicates that the value to be displayed needs to be taken from a variable sum.</li>
</ul>
<p><strong>Program 1.4</strong></p>
<p><strong>C program to convert the temperature in Celsius to Fahrenheit</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float C, F;</p>
<p>C=38.5;</p>
<p>F = 9*C/5 +32;</p>
<p>printf("temperature in Fahrenheit= %f", F);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>temperature in Fahrenheit= 101.3</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> If x is used instead of * and F = 9C/5 +32 is used of F = 9*C/5 +32, then the compilation error will be displayed on the screen.</li>
</ul>
<p>&nbsp;</p>
<p>If you want to supply a number 16 digits after decimal point i.e., 36.5555555555555555 for C, then the statement</p>
<p>&nbsp;</p>
<p>double C, F; should be used instead of the statement float C, F;</p>
<p>&nbsp;</p>
<p>and %lf should be used instead of %f</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double C, F;</p>
<p>C=38.5555555555555555;</p>
<p>F = 9*C/5 +32;</p>
<p>printf("temperature in Fahrenheit= %lf", F);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>And if you want to supply the number 16 digits after decimal point for C through the key board, then the statement</p>
<p>C = 38.5;</p>
<p>should be replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%lf", &amp;C);</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double C, F;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%lf", &amp;C);</p>
<p>F = 9*C/5 +32;</p>
<p>printf("temperature in Fahrenheit= %lf", F);</p>
<p>return 0;</p>
<p>}</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double C, F;</p>
<p>C = 25.3333333333333333;</p>
<p>F = 9*C/5 +32;</p>
<p>printf("temperature in Fahrenheit= %lf", F);</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>temperature in Fahrenheit = 77.600000</p>
<p>&nbsp;</p>
<p>If the statement double C, F; is replaced by the statements</p>
<p>&nbsp;</p>
<p>double C;</p>
<p>float F;</p>
<p>&nbsp;</p>
<p>i.e., if the above program is rewritten as:</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double C;</p>
<p>float F;</p>
<p>C = 25.3333333333333333;</p>
<p>F = 9*C/5 +32;</p>
<p>printf("temperature in Fahrenheit= %f", F); // %f is used because the data type for F is float</p>
<p>return 0;</p>
<p>}</p>
<p>Then there is slight change in the output on the screen:</p>
<p>temperature in Fahrenheit = 77.599998</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>Write a program to print the sum of three numbers</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c, sum;</p>
<p>printf("Enter any three numbers:");</p>
<p>scanf("%d %d%d", &amp;a, &amp;b, &amp;c);</p>
<p>sum = a + b + c;</p>
<p>printf("the sum of a, b and c = %d", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the Equivalent hexadecimal value of an integer</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a = 45;</p>
<p>printf("%x", a);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>2d</p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>Write a program to print the area of a triangle, given </strong></li>
</ul>
<p><strong>area = (s (s-a) (s-b) (s-c))<sup>1/2</sup> where s = (a + b + c) / 2 </strong></p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c, s, area;</p>
<p>a = 3;</p>
<p>b= 4;</p>
<p>c=5;</p>
<p>s = (a + b + c) / 2;</p>
<p>area = sqrt ((s * (s-a) * (s-b) * (s-c));</p>
<p>printf("the area of the triangle = %d", area);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> since sqrt() is not part of C language or of standard input output file i.e., (stdio.h file), it is part of math file i.e., (math.h file which defines various mathematical functions) the statement <strong>#include&lt;math.h&gt;</strong> should be included in the C program otherwise the compilation error will be flagged on the screen stating that sqrt() is not declared or defined.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> If the statement area = (s (s-a) (s-b) (s-c)) <sup>1/2</sup>&nbsp;&nbsp; is written instead of</li>
</ul>
<p>area = sqrt ((s * (s-a) * (s-b) * (s-c));</p>
<p>Then the compilation error will be displayed on the screen because C does not support</p>
<p>area = (s (s-a) (s-b) (s-c)) <sup>1/2</sup> .</p>
<p>&nbsp;</p>
<ul>
<li><strong>Stuff you need to know about:</strong></li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong><em>1 kilobyte = 1024 bytes</em></strong></li>
<li><strong><em>1 megabyte = 1024 &times; 1024 bytes</em></strong></li>
<li><strong><em>1 gigabyte = 1024 &times; 1024 &times; 1024 bytes</em></strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Program 1.5</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to find the product of two numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, product;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>product = a * b;</p>
<p>printf("the product of a and b = %d", product);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of a and b = 2</p>
<p>&nbsp;</p>
<p>If you want to insert a 10 digit number for a and b i.e.,</p>
<p>&nbsp;</p>
<p>a=1000000000</p>
<p>b=3000000000, then the statement:</p>
<p>int a, b, product; should be replaced by the statement long int a, b, product;</p>
<p>and %ld should be used instead of %d</p>
<p>&nbsp;</p>
<p>i.e., the program should be rewritten as:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>long int a, b, product;</p>
<p>a=1000000000;</p>
<p>b=2000000000;</p>
<p>product = a * b;</p>
<p>printf("the product of a and b = %ld", product);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of a and b = 3000000000000000000</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then the statements</p>
<p>a=1;</p>
<p>b=2;&nbsp; should be replaced by the statements</p>
<p>printf("Enter any two numbers:");</p>
<p>scanf("%d %d", &amp;a, &amp;b);</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, product;</p>
<p>printf("Enter any two numbers:");</p>
<p>scanf("%d%d", &amp;a, &amp;b);</p>
<p>product = a* b;</p>
<p>printf("the product of a and b = %d", product);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two numbers:</p>
<p>If you enter two numbers 1 and 3</p>
<p>the product of a and b = 3 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If you replace the statements</p>
<p>printf("Enter any two numbers:");</p>
<p>scanf("%d%d", &amp;a, &amp;b);</p>
<p>&nbsp;</p>
<p>by the statements</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen will be:</strong></p>
<p>&nbsp;</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>the product of a and b = 9</p>
<p>will be outputted on the screen.</p>
<p>If the statement</p>
<p>printf("the product of a and b = %d"; product);</p>
<p>is written instead of the statement</p>
<p>printf("the product of a and b = %d", product);</p>
<p>i.e., instead of variable separator (i.e., comma) semicolon is used -- Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello, World!");</p>
<p>printf("Hello, World!\b");</p>
<p>printf("Hello, World!\b");</p>
<p>printf("Hello, World!\b");</p>
<p>return 0;</p>
<p>}</p>
<p>i.e., if&nbsp; back space \b is used then</p>
<p>Hello, World!Hello, World!Hello, World!Hello, World!</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If carriage return \r is used instead of \b</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello, World!");</p>
<p>printf("Hello, World!\r");</p>
<p>printf("Hello, World!\r");</p>
<p>printf("Hello, World!\r");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>Hello, World!Hello, World!</p>
<p>Hello, World!</p>
<p>Hello, World!</p>
<p>&nbsp;</p>
<p>If Horizontal tab \t is used instead of \r</p>
<p>i.e.,</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello, World!\t");</p>
<p>printf("Hello, World!\t");</p>
<p>printf("Hello, World!\t");</p>
<p>printf("Hello, World!\t");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>&nbsp;</p>
<p>Hello, World!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hello, World!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hello, World!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Hello, World!</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>If vertical tab \v is used instead of \t</p>
<p>i.e.,</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("Hello, World!\v");</p>
<p>printf("Hello, World!\v");</p>
<p>printf("Hello, World!\v");</p>
<p>printf("Hello, World!\v");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>Hello, World!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Hello, World!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Hello, World!&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Hello, World!</p>
<p>&nbsp;</p>
<p><strong>Program 1.5</strong></p>
<p><strong>C program to find the square of a number</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b = a * a;</p>
<p>printf("the square of a = %d", b);</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the square of a = 4</p>
<p>&nbsp;</p>
<p>If the statement b = a * a; is replaced by b = pow((a), 2);</p>
<p>i.e., if the above program is rewritten as:</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b = pow((a), 2);</p>
<p>printf("the square of a = %d", b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then there will be no display of compilation error on the screen or there will be no change in the output on the screen i.e.,</p>
<p>the square of a = 4 will be outputted on the screen.</p>
<p><strong>which means:</strong></p>
<p>b = pow((a), 2); is the same as b = a*a;</p>
<p>Since b = pow((a), 2); is used instead of&nbsp; b = a*a;</p>
<p>#include&lt;math.h&gt; should be included in the C program as b = pow((a), 2); is supported by #include&lt;math.h&gt;</p>
<p>Otherwise compilation Error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>If you want to supply the integer value for a through the key board, then the statement</p>
<p>a=2; is replaced by the statements</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>i.e.,</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>b = a * a;</p>
<p>printf("the square of a = %d", b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter any number:</p>
<p>If you enter a number 4</p>
<p>the square of a = 16 will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>If scanf(%d, &amp;a); is written instead of scanf("%d", &amp;a);</p>
<p>If printf(the square of a = %d, b); is written instead of printf("the square of a = %d", b);</p>
<p>&nbsp;</p>
<p>If the main function is followed by a semicolon i.e.,</p>
<p>int main(); is written instead of int main()</p>
<p>Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>But if the body of the main function is followed by a semicolon i.e.,</p>
<p>int main()</p>
<p>{</p>
<p>}; is written instead of</p>
<p>int main()</p>
<p>{</p>
<p>&nbsp;</p>
<p>}</p>
<p>There will be no display of the compilation error on the screen.</p>
<p>int main(); &rarr; ERROR</p>
<p>int main()</p>
<p>{</p>
<p>}; &rarr; NO ERROR</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the cube of a number </strong></li>
</ul>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b = pow((a), 3);</p>
<p>printf("the cube of a = %d", b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the energy of the substance using energy = mc<sup>2</sup></strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int m;</p>
<p>long int c, energy;</p>
<p>m=2;</p>
<p>c = 300000000;</p>
<p>energy = m * pow((c), 2);</p>
<p>printf("the energy of the substance&nbsp; = %ld joules", energy);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 1.6</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to find the greatest of two numbers using if - else statement</strong></p>
<p>&nbsp;</p>
<p>The syntax of if &ndash; else statement (<strong>Conditional Statements</strong>):</p>
<p>&nbsp;</p>
<p><strong><em>if (this condition is true)</em></strong></p>
<p><strong><em>{</em></strong></p>
<p><strong><em>print this statement;</em></strong></p>
<p><strong><em>}</em></strong></p>
<p><strong><em>else </em></strong></p>
<p><strong><em>{</em></strong></p>
<p><strong><em>print this statement;</em></strong></p>
<p><strong><em>}</em></strong></p>
<p><strong><em>&nbsp;</em></strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a = 2;</p>
<p>b = 3;</p>
<p>if(a&gt;b)</p>
<p>{</p>
<p>printf("a is greater than b");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("b is greater than a");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>b is greater than a</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Since the condition a&gt;b within the parentheses is not true, the statement a is greater than b is not executed;</p>
<p>instead the execution skips and pass to print the statement b is greater than a.</p>
<p>&nbsp;</p>
<p>In simpler words,</p>
<p>(a&gt;b) is the condition (i.e., logical expression that results in true or false) and</p>
<p>if the condition (a&gt;b) is true, then the statement:</p>
<p>{</p>
<p>printf("a is greater than b");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>a is greater than b</p>
<p>else the statement</p>
<p>{</p>
<p>printf("b is greater than a");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p><strong>b is greater than a</strong></p>
<p>&nbsp;</p>
<p>If you want to supply the integer values for a and b through the key board, then the statements</p>
<p>&nbsp;</p>
<p>a=2;</p>
<p>b=3; should be replaced by the statements</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>&nbsp;</p>
<p>i.e., the program should be rewritten as:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>if(a&gt;b)</p>
<p>{</p>
<p>printf("a is greater than b");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("b is greater than a");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 6</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>a is greater than b</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 1.7</strong></p>
<p><strong>C program to find the greatest of three numbers using if - else if - else statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>The syntax of if - else&nbsp; if - else statement:</p>
<p>&nbsp;</p>
<p><strong><em>if (this condition is true)</em></strong></p>
<p><strong><em>{</em></strong></p>
<p><strong><em>print this statement;</em></strong></p>
<p><strong><em>}</em></strong></p>
<p><strong><em>else if (this condition is true)</em></strong></p>
<p><strong><em>{</em></strong></p>
<p><strong><em>print this statement;</em></strong></p>
<p><strong><em>}</em></strong></p>
<p><strong><em>else&nbsp; </em></strong></p>
<p><strong><em>{</em></strong></p>
<p><strong><em>print this statement;</em></strong></p>
<p><strong><em>}</em></strong></p>
<p><em>&nbsp;</em></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;c);</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>{</p>
<p>printf("%d is greater than %d and %d", a, b, c);</p>
<p>}</p>
<p>else if (b&gt;a&amp;&amp;b&gt;c)</p>
<p>{</p>
<p>printf("%d is greater than %d and %d", b, a, c);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("%d is greater than %d and %d", c, b, a);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 4</p>
<p>4 is greater than 3 and 2</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>double ampersand "&amp;&amp;" imply and.</p>
<p>(a&gt;b&amp;&amp;a&gt;c)</p>
<p>(b&gt;a&amp;&amp;b&gt;c)</p>
<p>denote conditions.</p>
<p>i.e., the condition</p>
<p>(a&gt;b&amp;&amp;a&gt;c) imply:</p>
<p>a is greater than b and a is greater than c</p>
<p>and if this condition is true, then the statement</p>
<p>{</p>
<p>printf("a is greater than b and c");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>a is greater than b and c</p>
<p>and if the condition (a&gt;b&amp;&amp;a&gt;c) is not true</p>
<p>the statement&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>{</p>
<p>printf("a is greater than b and c");</p>
<p>}</p>
<p>is not executed; instead the execution skips and pass to the condition (b&gt;a&amp;&amp;b&gt;c)</p>
<p>and if this condition is true, then the statement</p>
<p>{</p>
<p>printf("b is greater than a and c");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>b is greater than a and c</p>
<p>and if the condition (b&gt;a&amp;&amp;b&gt;c) is not true, then the statement</p>
<p>{</p>
<p>printf("b is greater than a and c");</p>
<p>}</p>
<p>is not executed; instead the execution skips and the statement</p>
<p>{</p>
<p>printf("c is greater than b and a");</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>c is greater than b and a</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>&nbsp;</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>{</p>
<p>printf("%d is greater than %d and %d", a, b, c);</p>
<p>}</p>
<p>else if (b&gt;a&amp;&amp;b&gt;c)</p>
<p>{</p>
<p>printf("%d is greater than %d and %d", b, a, c);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("%d is greater than %d and %d", c, b, a);</p>
<p>}</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>printf("%d is greater than %d and %d", a, b, c);</p>
<p>else if (b&gt;a&amp;&amp;b&gt;c)</p>
<p>printf("%d is greater than %d and %d", b, a, c);</p>
<p>else</p>
<p>printf("%d is greater than %d and %d", c, b, a);</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>i.e., if the program is rewritten as:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;c);</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>printf("%d is greater than %d and %d", a, b, c);</p>
<p>else if (b&gt;a&amp;&amp;b&gt;c)</p>
<p>printf("%d is greater than %d and %d", b, a, c);</p>
<p>else</p>
<p>printf("%d is greater than %d and %d", c, b, a);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>There will be no display of error on the screen</p>
<p>c is greater than b and a</p>
<p>will be successfully outputted on the screen</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program ?</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b=2;</p>
<p>if(a&gt;b || a= = b)</p>
<p>printf("a is greater than or equal to b");</p>
<p>else</p>
<p>printf("b is greater than a");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>a is greater than or equal to b</p>
<p>&nbsp;</p>
<p>Note: symbol || denote OR i.e., a&gt;b || a= = b denote a is greater than or a is equal to b.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 1.8</strong></p>
<p><strong>C program to find the average of 10 numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int N1, N2, N3, N4, N5, N6, N7, N8, N9, N10, X;</p>
<p>printf("Enter any 10 numbers:");</p>
<p>scanf("%d%d%d%d%d%d%d%d%d%d", &amp;N1, &amp;N2, &amp;N3, &amp;N4, &amp;N5, &amp;N6, &amp;N7, &amp;N8, &amp;N9, &amp;N10);</p>
<p>X = (N1 + N2 + N3 + N4 + N5 + N6 + N7 + N8 + N9 + N10) /10;</p>
<p>printf("the average of 10 numbers = %d", X);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter any 10 numbers:</p>
<p>If you enter ten numbers 1, 2, 3, 4, 5, 6, 7, 8, 9 and 10</p>
<p>the average of 10 numbers = 5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> The average of 10 numbers is 5.5, the output on the screen is 5 because the data type int is used instead of float.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>Any mathematical expression should be written in C equivalent expression to prevent the display of compilation error on the screen because C language does not accept the general mathematical expressions.</strong></li>
</ul>
<p>&nbsp;</p>
<table width="419">
<tbody>
<tr>
<td width="181">
<p><strong><em>Mathematical expression</em></strong></p>
</td>
<td width="237">
<p><strong><em>C equivalent expression</em></strong></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>x &times; y / z</em></p>
</td>
<td width="237">
<p><em>x * y / z</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>(ax + 1) (by + 2)</em></p>
</td>
<td width="237">
<p><em>(a * x + 1) * (b * y + 2)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>(a+b)<sup>2</sup>/ (a-b)<sup>2</sup></em></p>
</td>
<td width="237">
<p><em>(a+b) * (a+b) / (a-b) * (a-b)&nbsp;<br /> or&nbsp;<br /> pow((a+b), 2) / pow((a - b), 2)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>log&nbsp;<sub>10</sub>&nbsp;(x/y + c)</em></p>
</td>
<td width="237">
<p><em>log 10 (x/y + c)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>ax<sup>2</sup>+bx+c</em></p>
</td>
<td width="237">
<p><em>a*x*x+b*x+c</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>lnx</em></p>
</td>
<td width="237">
<p><em>log(x)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>ex + b</em></p>
</td>
<td width="237">
<p><em>exp (x) + b</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>sin&theta; + cos&theta;</em></p>
</td>
<td width="237">
<p><em>sin (theta) + cos (theta)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>&alpha; = &beta; + &gamma;</em></p>
</td>
<td width="237">
<p><em>alpha = beta + gamma</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>x&nbsp;<sup>1/2</sup></em></p>
</td>
<td width="237">
<p><em>sqrt(x)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>x&nbsp;<sup>1/3</sup></em></p>
</td>
<td width="237">
<p><em>cbrt(x)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>(p<sup>2</sup>&nbsp;+ q<sup>2</sup>)<sup>1/2</sup></em></p>
</td>
<td width="237">
<p><em>sqrt (p*p + q*q)</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>2a<sup>2</sup>&nbsp;+ 3b</em></p>
</td>
<td width="237">
<p><em>2a *a + 3b + 2</em></p>
</td>
</tr>
<tr>
<td width="181">
<p><em>a = e x / (1+ sin&theta;)<sup>1/2</sup></em></p>
</td>
<td width="237">
<p><em>a = exp ( x / sqrt ( 1 + sin (theta)))</em></p>
</td>
</tr>
</tbody>
</table>
<p><em>&nbsp;</em></p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following programs:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>(a)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, x;</p>
<p>x=2;</p>
<p>b=2;</p>
<p>a = exp (x) + b;</p>
<p>printf("the value of a = %d", a);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>the value of a = 9</p>
<p>&nbsp;</p>
<p>(b)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int alpha, beta, gamma;</p>
<p>alpha =2;</p>
<p>beta=2;</p>
<p>gamma=&nbsp; 2 * alpha +&nbsp; beta;</p>
<p>printf("the value of alpha = %d", alpha);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>the value of alpha = 2</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>(c)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double theta,&nbsp; result;</p>
<p>theta = 90;</p>
<p>result = sin(theta);</p>
<p>printf ("The sine 90 degrees is = %lf ", result);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>The sine 90 degrees is = 0.893997</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is C equivalent expression of (x/y) <sup>n-1</sup>?</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer:</strong>&nbsp;&nbsp; pow((x/y), n-1)</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 1.9</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to find the square root of a number</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp; a);</p>
<p>b = sqrt (a);</p>
<p>printf("the square root of a number = %d", b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 4</p>
<p>the square root of a number = 2</p>
<p>is outputted on the screen.</p>
<p>&nbsp;</p>
<p>Suppose if you enter the number 2, the square root of a number = 1 is outputted on the screen because int is used instead of float.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>&nbsp;</p>
<p>Since b = sqrt (a) is written</p>
<p>&nbsp;</p>
<p>#include&lt;math.h&gt;</p>
<p>&nbsp;</p>
<p>must be included in the above program otherwise compilation error will flag on the screen.</p>
<p>i.e., the program:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp; a);</p>
<p>b = sqrt (a);</p>
<p>printf("the square root of a number = %d", b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>will flag compilation error on the screen.</p>
<p>If float is used instead of int then the above program take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float a, b;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp; a);</p>
<p>b = sqrt (a);</p>
<p>printf("the square root of a number = %f", b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 5</p>
<p>the square root of a number = 2.23</p>
<p>is outputted on the screen.</p>
<p>&nbsp;</p>
<p>This program can also be written as:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("the square root of a number = %f", sqrt (4));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>//--------------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p><strong>&nbsp;</strong></p>
<p><strong><em>|| imply or</em></strong></p>
<p><strong><em>&gt; imply greater than</em></strong></p>
<p><strong><em>&lt;imply less than</em></strong></p>
<p><strong><em>= = imply equal to</em></strong></p>
<p><strong><em>! imply not</em></strong></p>
<p><strong><em>!= imply not equal to</em></strong></p>
<p><strong><em>&amp;&amp; imply and</em></strong></p>
<p><strong><em>&amp; imply address</em></strong></p>
<p><em>&nbsp;</em></p>
<p>&nbsp;</p>
<p>-------------------------------------------------------------------------------------------------------------------------------------//</p>
<p><strong>Program 2.0</strong></p>
<p><strong>C program to find the simple interest</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int P,T, R, SI;</p>
<p>P = 1000;</p>
<p>T = 2;</p>
<p>R = 3;</p>
<p>SI = P*T*R/100;</p>
<p>printf("the simple interest = %d", SI);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the simple interest = 60</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>If you write SI = PTR/100; instead of SI = P*T*R/100;</p>
<p>Then compilation error is displayed on the screen because C language does not accept the general expressions.</p>
<p>&nbsp;</p>
<p>If you want to supply the values for P, T and R through the key board, then the statements:</p>
<p>&nbsp;</p>
<p>P = 1000;</p>
<p>T = 2;</p>
<p>R = 3;</p>
<p>&nbsp;</p>
<p>should be replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;P);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;T);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;R);</p>
<p>&nbsp;</p>
<p>i.e., the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int P,T, R, SI;</p>
<p>printf("Enter principal amount:");</p>
<p>scanf("%d", &amp;P);</p>
<p>printf("Enter time:");</p>
<p>scanf("%d", &amp;T);</p>
<p>printf("Enter rate of interest:");</p>
<p>scanf("%d", &amp;R);</p>
<p>SI = P*T*R/100;</p>
<p>printf("the simple interest = %d", SI);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter principal amount:</p>
<p>If you enter the principal amount 1000</p>
<p>Enter time:</p>
<p>If you enter the time 2</p>
<p>Enter rate of interest:</p>
<p>If you enter the rate of interest 3</p>
<p>the simple interest = 60</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> If write the statement scanf("%d,"&amp;P); instead of scanf("%d", &amp;P);</li>
</ul>
<p>or</p>
<p>if write the statement scanf(%d, &amp;P); instead of scanf("%d", &amp;P); i.e., format string for data type int i.e., %d is not enclosed by double quotes ("")</p>
<p>Then compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.1</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to find whether the person is senior citizen or not</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int age;</p>
<p>age=20;</p>
<p>if(age&gt; = 60)</p>
<p>{</p>
<p>printf("senior citizen");</p>
<p>}</p>
<p>if(age&lt;60)</p>
<p>{</p>
<p>printf("not a senior citizen");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>not a senior citizen</p>
<p>(age&gt; = 60) means age greater than or equal to 60</p>
<p>If you want to supply the value for age through the key board, then the statement</p>
<p>age=20;</p>
<p>should be replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("Enter age:");</p>
<p>scanf("%d", &amp;age);</p>
<p>&nbsp;</p>
<p>i.e., the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int age;</p>
<p>printf("Enter age:");</p>
<p>scanf("%d", &amp;age);</p>
<p>if(age&gt;60)</p>
<p>{</p>
<p>printf("senior citizen");</p>
<p>}</p>
<p>if(age&lt;60)</p>
<p>{</p>
<p>printf("not a senior citizen");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter age:</p>
<p>If you enter the value 60</p>
<p>senior citizen will be outputted on the screen.</p>
<p>Suppose if you enter the value 27</p>
<p>not a senior citizen will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.2</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to get marks for 3 subjects and declare the result.</strong></p>
<p><strong>If the marks &gt;= 35 in all the subjects the student passes else fails.</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int M1, M2,M3;</p>
<p>M1 = 38;</p>
<p>M2= 45;</p>
<p>M3 = 67;</p>
<p>if(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35)</p>
<p>{</p>
<p>printf("candidate is passed");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("candidate is failed");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>candidate is passed</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>&gt;= imply greater than or equal to and double ampersand imply and</p>
<p>(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35) denote the condition and this condition imply M1 is greater than or equal to 35</p>
<p>and M2 is greater than or equal to 35 and M3 is greater than or equal to 35. And if this condition is TRUE, then the statement</p>
<p>{</p>
<p>printf("candidate is passed");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>candidate is passed</p>
<p>else the statement</p>
<p>{</p>
<p>printf("candidate is failed");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>candidate is failed</p>
<p>&nbsp;</p>
<p>If you want to supply the integer values for marks M1, M2 and M3 through the key board, then the statements:</p>
<p>&nbsp;</p>
<p>M1 = 38;</p>
<p>M2= 45;</p>
<p>M3 = 67;</p>
<p>&nbsp;</p>
<p>should be replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("Enter any three numbers:");</p>
<p>scanf("%d%d%d", &amp;M1, &amp;M2, &amp;M3);</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int M1, M2,M3;</p>
<p>printf("Enter any three numbers:");</p>
<p>scanf("%d%d%d", &amp;M1, &amp;M2, &amp;M3);</p>
<p>if(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35)</p>
<p>{</p>
<p>printf("candidate is passed");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("candidate is failed");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any three numbers:</p>
<p>If you enter three numbers 26, 28, 39</p>
<p>candidate is failed will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<table width="458">
<tbody>
<tr>
<td width="125">
<p><strong><em>Header file in C</em></strong></p>
</td>
<td width="333">
<p><strong><em>the functions it&nbsp; defines</em></strong></p>
</td>
</tr>
<tr>
<td width="125">
<p><strong><em>stdio.h</em></strong></p>
</td>
<td width="333">
<p><em>(standard input output header file)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em></p>
<p><em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; standard input output functions (like scanf and printf functions)</em></p>
</td>
</tr>
<tr>
<td width="125">
<p><strong><em>math.h</em></strong></p>
</td>
<td width="333">
<p><em>mathematical functions (like&nbsp; log(), sqrt(), sin(), cos(), log10() etc.)</em></p>
</td>
</tr>
<tr>
<td width="125">
<p><strong><em>stdlib.h</em></strong></p>
</td>
<td width="333">
<p><em>standard library functions (like void abort(void) - a function which causes an abnormal/ unusual program termination)</em></p>
</td>
</tr>
<tr>
<td width="125">
<p><strong><em>ctype.h</em></strong></p>
</td>
<td width="333">
<p><em>character manipulation functions</em></p>
<p><em>(like isalpha() which checks whether a character is an alphabet or not)</em></p>
</td>
</tr>
<tr>
<td width="125">
<p><strong><em>graphics.h</em></strong></p>
</td>
<td width="333">
<p><em>graphical functions</em></p>
</td>
</tr>
<tr>
<td width="125">
<p><strong><em>conio.h</em></strong></p>
</td>
<td width="333">
<p><em>(console input output header file)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em></p>
<p><em>console input output functions like clrscr() - a function which clears the screen.</em></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> The term console usually refers to monitor or display screen.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to check whether a character is an alphabet or not using the function isalpha()</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include &lt;ctype.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a =2;</p>
<p>if( isalpha(a) )</p>
<p>{</p>
<p>printf(" the character a&nbsp; is an alphabet");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("the character a&nbsp; is not an alphabet");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>the character a&nbsp; is not an alphabet&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include &lt;ctype.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char a = 'b';</p>
<p>if( isalpha(a) )</p>
<p>{</p>
<p>printf(" the character a&nbsp; is an alphabet");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("the character a&nbsp; is not an alphabet");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the character a&nbsp; is an alphabet</p>
<p>&nbsp;</p>
<p>If the statement char a = b; is written instead of char a = 'b'; Then the compilation error will be flagged on the display screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.3</strong></p>
<p><strong>C program to find profit or loss</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int CP, SP, loss, profit;</p>
<p>printf("Enter cost price:");</p>
<p>scanf("%d", &amp;CP);</p>
<p>printf("Enter selling price:");</p>
<p>scanf("%d", &amp;SP);</p>
<p>if(SP&gt;CP)</p>
<p>{</p>
<p>printf("profit=%d", SP-CP);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("loss =%d", CP-SP);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter cost price:</p>
<p>If you enter the cost price 25</p>
<p>Enter selling price:</p>
<p>If you enter the selling price 26</p>
<p>profit = 1 will be outputted on the screen.</p>
<p>If the condition (SP&gt;CP) is true, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("profit=%d", SP-CP);</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>profit = SP-CP (in this case profit = 26-25 =1)</p>
<p>else the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("loss=%d", CP-SP);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>loss = CP-SP</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p><strong>Program 2.4</strong></p>
<p><strong>C program to convert inches into centimeter</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float I, C;</p>
<p>I=3.5;</p>
<p>C = 2.54*I;</p>
<p>printf("length in centimeters= %f", C);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>length in centimeters = 8.89</p>
<ul>
<li><strong>Note:</strong> float is used instead of int because I = 3.5 if int is used instead of float then the result will not be clearly outputted i.e., instead of 8.89 the computer displays only 8. And since float is used instead of int, the operator %d is replaced by the operator %f.</li>
</ul>
<p>&nbsp;</p>
<p>If you want to supply the floating value for I through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float I, C;</p>
<p>printf("Enter the length in inches:");</p>
<p>scanf("%f", &amp;I);</p>
<p>C = 2.54*I;</p>
<p>printf("length in centimeters= %f", C);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter the length in inches:</p>
<p>If you enter the floating point value or fractional or decimal number for I i.e., 25.5</p>
<p>length in centimeters = 64.9 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 2.5</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to find the incremented and decremented values of two numbers.</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c, d, e, f;</p>
<p>a = 10;</p>
<p>b=12;</p>
<p>c=a+1;</p>
<p>d=b+1;</p>
<p>e=a-1;</p>
<p>f=b-1;</p>
<p>printf("the incremented value of a =%d", c);</p>
<p>printf("the incremented value of b =%d", d);</p>
<p>printf("the decremented value of a =%d", e);</p>
<p>printf("the decremented value of b =%d", f);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the incremented value of a = 11 the incremented value of b = 13 the decremented value of a = 9 the decremented value of b = 11</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>&nbsp;</p>
<p>printf("the incremented value of a =%d", c);</p>
<p>printf("the incremented value of b =%d", d);</p>
<p>printf("the decremented value of a =%d", e);</p>
<p>printf("the decremented value of b =%d", f);</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("the incremented value of a =%d\n", c);</p>
<p>printf("the incremented value of b =%d\n", d);</p>
<p>printf("the decremented value of a =%d\n", e);</p>
<p>printf("the decremented value of b =%d\n", f);</p>
<p>&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>the incremented value of a = 11</p>
<p>the incremented value of b = 13</p>
<p>the decremented value of a = 9</p>
<p>the decremented value of b = 11</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>Even if the statements:</p>
<p>&nbsp;</p>
<p>printf("the incremented value of a =%d\n", c);</p>
<p>printf("the incremented value of b =%d\n", d);</p>
<p>printf("the decremented value of a =%d\n", e);</p>
<p>printf("the decremented value of b =%d\n", f);</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>printf("\n the incremented value of a =%d", c);</p>
<p>printf("\n the incremented value of b =%d", d);</p>
<p>printf("\n the decremented value of a =%d", e);</p>
<p>printf("\n the decremented value of b =%d", f);</p>
<p>&nbsp;</p>
<p>There will be no change in the output on the screen.</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c, d, e, f;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>c=a+1;</p>
<p>d=b+1;</p>
<p>e=a-1;</p>
<p>f=b-1;</p>
<p>printf("the incremented value of a =%d\n", c);</p>
<p>printf("the incremented value of b =%d\n", d);</p>
<p>printf("the decremented value of a =%d\n", e);</p>
<p>printf("the decremented value of b =%d\n", f);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>&nbsp;</p>
<p>the incremented value of a = 3</p>
<p>the incremented value of b = 4</p>
<p>the decremented value of a = 1</p>
<p>the decremented value of b = 2</p>
<p>&nbsp;</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Note:</strong> b++ is same as b + 1 and b-- is same as b - 1.</p>
<p>&nbsp;</p>
<p><strong>Program 2.6</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>The percentage marks are entered and the grades are allotted as follows :&nbsp;&nbsp;&nbsp;&nbsp; </strong></p>
<p>percentage&gt;= 60 First Class</p>
<p>percentage&gt;=50 and per &lt;= 60 Second Class</p>
<p>percentage&gt;= 40 and per &lt;= 50 Pass Class</p>
<p>percentage&lt; 40 Fail</p>
<p><strong>Write a C program for the above:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int P;</p>
<p>printf("Enter the percentage:");</p>
<p>scanf("%d", &amp;P);</p>
<p>if(P &gt;= 60)</p>
<p>{</p>
<p>printf("first class");</p>
<p>}</p>
<p>if(P&gt;=50&amp;&amp;P &lt;60)</p>
<p>{</p>
<p>printf("second class");</p>
<p>}</p>
<p>else if(P&gt;=40&amp;&amp;P&lt;=50 )</p>
<p>{</p>
<p>printf("pass class");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("fail");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter the percentage:</p>
<p>If you enter the percentage 65</p>
<p>first class will be outputted on the screen.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Program 2.7</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to calculate the discounted price and the total price after discount</strong></p>
<p><strong>Given:</strong></p>
<p>If purchase value is greater than 1000, 10% discount</p>
<p>If purchase value is greater than 5000, 20% discount</p>
<p>If purchase value is greater than 10000, 30% discount</p>
<p>&nbsp;</p>
<ul>
<li><strong>discounted price</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double PV, dis;</p>
<p>printf("Enter purchased value:");</p>
<p>scanf("%lf", &amp;PV);</p>
<p>if(PV&gt;1000)</p>
<p>{</p>
<p>printf("dis=%lf", PV* 0.1);</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>printf("dis =%lf", PV* 0.2);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("dis=%lf", PV* 0.3);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 6500</p>
<p>dis = 1300.000000 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>(PV&gt;1000), (PV&gt;5000) denote the conditions and if the condition (PV&gt;1000) is true i.e., purchased value is greater than 1000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("dis=%d", PV* 0.1);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 10% = PV* 10 /100 = PV* 0.1</p>
<p>and if the condition (PV&gt;1000) is false and if the condition (PV&gt;5000) is true i.e., purchased value is greater than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("dis=%d", PV* 0.2);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 20% = PV* 20 /100 = PV* 0.2</p>
<p>and if the condition (PV&gt;5000) is not true i.e., purchased value is less than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("dis=%d", PV* 0.3);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 30% = PV* 30 /100 = PV* 0.3</p>
<p>&nbsp;</p>
<ul>
<li><strong>total price </strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double PV, total;</p>
<p>printf("Enter purchased value:");</p>
<p>scanf("%lf", &amp;PV);</p>
<p>if(PV&lt;1000)</p>
<p>{</p>
<p>printf("total=%lf", PV - PV* 0.1);</p>
<p>}</p>
<p>else if(PV&lt;5000)</p>
<p>{</p>
<p>printf("total =%lf", PV- PV* 0.2);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("total=%lf", PV- PV* 0.3);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 650</p>
<p>total = 585.000000&nbsp; will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the condition (PV&gt;1000) is true i.e., purchased value is greater than 1000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("total = %d", PV - PV* 0.1);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*10% = PV- PV* 10 /100 = PV - PV * 0.1</p>
<p>and if the condition (PV&gt;1000) is false and if the condition (PV&gt;5000) is true i.e., purchased value is greater than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("total = %d", PV - PV* 0.2);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*20% = PV- PV* 20 /100 = PV - PV * 0.2</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>and if the condition (PV&gt; 5000) is not true i.e., purchased value is less than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>printf("total = %d", PV - PV* 0.3);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>&nbsp;</p>
<p>total =PV- dis = PV- PV*30% = PV- PV* 30 /100 = PV - PV * 0.3</p>
<p>&nbsp;</p>
<p><strong>Now, Combing both the programs (above), we can write:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>double PV, dis, total;</p>
<p>printf("Enter purchased value:");</p>
<p>scanf("%lf", &amp;PV);</p>
<p>if(PV&gt;1000)</p>
<p>{</p>
<p>printf("dis=%lf", PV* 0.1);</p>
<p>printf("total=%lf", PV - PV* 0.1);</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>printf("dis =%lf", PV* 0.2);</p>
<p>printf("total=%lf", PV - PV* 0.1);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("dis=%lf", PV* 0.3);</p>
<p>printf("total=%lf", PV - PV* 0.1);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>The output on the screen:</p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 850</p>
<p>dis = 85.000000</p>
<p>total = 765.000000</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.8</strong></p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>C program to print the first ten natural numbers using for loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i=1; i&lt;=10; i++)</p>
<p>printf("value of i =%d", i);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>value of i = 1 value of i = 2&nbsp; value of i= 3&nbsp; value of i= 4&nbsp; value of i= 5&nbsp; value of i= 6 value of i = 7 value of i= 8&nbsp; value of i = 9&nbsp; value of i = 10</p>
<p>&nbsp;</p>
<p>for (i=1; i&lt;=10; i++) denote the</p>
<p>for loop statement and the syntax of the</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for loop statement is:</p>
<p>for (initialization; condition; increment)</p>
<p>Here:</p>
<p>i=1 denote initialization (i.e., from where to start)</p>
<p>i&lt;=10 denote the condition (i.e., stop when 10 is reached)</p>
<p>i++ imply increment (which tells the value of i to increase by 1 each time the loop is executed) and i++ is the same as i+1.</p>
<p>&nbsp;</p>
<ul>
<li><strong>When a for loop executes, the following occurs:</strong></li>
</ul>
<p>&nbsp;</p>
<p>i = 1</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=1</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 1</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 1+1 = 2</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=2</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 2</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 2+1 = 3</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=3</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 3</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 3+1 = 4</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=4</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 4</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 4+1 = 5</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=5</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 5</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 5+1 = 6</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=6</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 6</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 6+1 = 7</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=7</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 7</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 7+1 = 8</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=8</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 8</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 8+1 = 9</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=9</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 9</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 9+1 = 10</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=10</p>
<p>The statement printf("value of i =%d", i); is executed to print the output:</p>
<p>value of i = 10</p>
<p>and stop because the condition i&lt;=10 is achieved.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>printf("value of i =%d", i);</p>
<p>is replaced by the statement:</p>
<p>printf("value of i =%d\n", i);</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; or</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;printf("\n value of i =%d", i);&nbsp;&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>&nbsp;</p>
<p>value of i = 1</p>
<p>value of i = 2</p>
<p>value of i = 3</p>
<p>value of i = 4</p>
<p>value of i = 5</p>
<p>value of i = 6</p>
<p>value of i = 7</p>
<p>value of i = 8</p>
<p>value of i = 9</p>
<p>value of i = 10</p>
<p>&nbsp;</p>
<p>If the</p>
<p>for loop statement:</p>
<p>&nbsp;</p>
<p>for (i=2; i&lt;=10; i++)</p>
<p>&nbsp;</p>
<p>is written instead of the statement:</p>
<p>&nbsp;</p>
<p>for(i=1; i&lt;=10; i++), then the output on the screen is:</p>
<p>&nbsp;</p>
<p>value of i = 2&nbsp; value of i = 3&nbsp; value of i= 4&nbsp; value of i= 5&nbsp; value of i= 6 value of i = 7 value of i= 8&nbsp; value of i = 9&nbsp; value of i= 10</p>
<p>&nbsp;</p>
<p>If the for loop statement:</p>
<p>for(i=1; i&lt;10; i++)</p>
<p>is written instead of the statement:</p>
<p>for (i=1; i&lt;=10; i++), then the output on the screen is:</p>
<p>value of i = 1 value of i = 2&nbsp; value of i= 3&nbsp; value of i= 4&nbsp; value of i= 5&nbsp; value of i= 6 value of i = 7 value of i= 8&nbsp; value of i = 9</p>
<p>&nbsp;</p>
<p>(Note: the condition i&lt;=10 tells to print till value of i =10 but the condition i&lt;10 tells to print till value of i=9)</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>for(i=1; i=10; i++)</p>
<p>is written instead of the statement:</p>
<p>for (i=1; i&lt;=10; i++), then the output on the screen is:</p>
<p>value of i = 10&nbsp; value of i = 10&nbsp; value of i = 10&nbsp; value of&nbsp; i = 10&nbsp; value of i= 10&nbsp; value of i= 10 value of i = 10 value of i= 10&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10&nbsp; value of i = 10&nbsp;&nbsp;&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10 (continues ...).</p>
<p>&nbsp;</p>
<p>Note:</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>printf("value of i =%d", i); is replaced by the statement printf("%d\n", i);</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>1</p>
<p>2</p>
<p>3</p>
<p>4</p>
<p>5</p>
<p>6</p>
<p>7</p>
<p>8</p>
<p>9</p>
<p>10</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program :</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i =1; i&lt;=5; i ++)</p>
<p>printf("Linux is not portable\n", i);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the first ten natural numbers using for while loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>The syntax of while loop statement is:</p>
<p><strong>while (this is the condition)</strong></p>
<p><strong>{</strong></p>
<p><strong>execute this statement;</strong></p>
<p><strong>}</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i = 1;</p>
<p>while (i&lt;=10)</p>
<p>{</p>
<p>printf("%d\n", i++);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>1</p>
<p>2</p>
<p>3</p>
<p>4</p>
<p>5</p>
<p>6</p>
<p>7</p>
<p>8</p>
<p>9</p>
<p>10</p>
<p>&nbsp;</p>
<p>(i&lt;=10) is the condition and</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>printf("%d\n", i++);</p>
<p>&nbsp;</p>
<p>is repeatedly executed as long as a given condition (i&lt;=10) is true.</p>
<p>If the statement:</p>
<p>int i=1;</p>
<p>is replaced by the statement:</p>
<p>int i;</p>
<p>&nbsp;</p>
<p>Then the compilation error will be displayed on the console screen because initialization is not defined i.e., from where to start is not declared.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int i = 1;</p>
<p>is replaced by the int i = 0;</p>
<p>Then the output on the screen is:</p>
<p>0</p>
<p>1</p>
<p>2</p>
<p>3</p>
<p>4</p>
<p>5</p>
<p>6</p>
<p>7</p>
<p>8</p>
<p>9</p>
<p>10</p>
<p>Similarly if the statement int i = 0; is replaced by the int i = 7;</p>
<p>Then the output on the screen is:</p>
<p>7</p>
<p>8</p>
<p>9</p>
<p>10</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print first 10 numbers using do while loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>The syntax of do while loop statement is:</p>
<p>&nbsp;</p>
<p><strong>do</strong></p>
<p><strong>{</strong></p>
<p><strong>execute this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>while(this is the condition);</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i =1;</p>
<p>do</p>
<p>{</p>
<p>printf(" i= %d\n", i++);</p>
<p>} while (i&lt;=10);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>i=1</p>
<p>i=2</p>
<p>i=3</p>
<p>i=4</p>
<p>i=5</p>
<p>i=6</p>
<p>i=7</p>
<p>i=8</p>
<p>i=9</p>
<p>i=10</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf(" i= %d\n", i++);</p>
<p>is executed and then condition (i&lt;=10) is checked. If condition (i&lt;=10) is true then</p>
<p>The statement:</p>
<p>printf(" i= %d\n", i++);</p>
<p>is executed again. This process repeats until the given condition (i&lt;=10) becomes false.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Why LOOP is USED?</strong></li>
</ul>
<p>&nbsp;</p>
<p>If loop is not used then the C program to print first 10 numbers should be written as follows:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("\n i = 1");</p>
<p>printf("\n i = 2");</p>
<p>printf("\n i = 3");</p>
<p>printf("\n i = 4");</p>
<p>printf("\n i = 5");</p>
<p>printf("\n i = 6");</p>
<p>printf("\n i = 7");</p>
<p>printf("\n i = 8");</p>
<p>printf("\n i = 9");</p>
<p>printf("\n i = 10");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>It takes pretty long time to write the code and the execution time is pretty long i.e., Because to reduce the time taken to write the code and to reduce the execution time -- loop statement is used.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>Never test for an error condition you don't know how to handle</p>
<p>&nbsp;</p>
<p><strong>5 times using for loop statement.</strong></p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i =1; i&lt;=5; i ++)</p>
<p>printf("Never test for an error condition you don't know how to handle \n");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>For the program:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i=1; i=5; i++)</p>
<p>printf("Linux is not portable");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable Linux is not portable &hellip;. continues</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 2.9</strong></p>
<p><strong>C program to print the characters from A to Z using for loop, do while loop and while loop statement.</strong></p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the characters from A to Z using for loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char a;</p>
<p>for( a='A'; a&lt;='Z'; a++)</p>
<p>printf("%c\n", a);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>The output on the screen:</p>
<p>&nbsp;</p>
<p>A</p>
<p>B</p>
<p>C</p>
<p>D</p>
<p>E</p>
<p>F</p>
<p>G</p>
<p>H</p>
<p>I</p>
<p>J</p>
<p>K</p>
<p>L</p>
<p>M</p>
<p>N</p>
<p>O</p>
<p>P</p>
<p>Q</p>
<p>R</p>
<p>S</p>
<p>T</p>
<p>W</p>
<p>X</p>
<p>Y</p>
<p>Z</p>
<p>&nbsp;</p>
<p>char means the data type is character.</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>char a; imply that we are creating the character a.</p>
<p>&nbsp;</p>
<p>Since char a is used. Therefore: the format specifier %c should be used instead of&nbsp; %d or %f otherwise error will be flagged on the screen.</p>
<p>&nbsp;</p>
<p>If the statement for( a=A; a&lt;=Z; a++) is written instead of the statement for( a='A'; a&lt;='Z'; a++)</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the characters from A to Z using while loop statement:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char a = 'A';</p>
<p>while (a&lt;='Z')</p>
<p>{</p>
<p>printf("%c\n", a++);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the characters from A to Z using do while loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char a = 'A';</p>
<p>do</p>
<p>{</p>
<p>printf(" %c\n", a++);</p>
<p>} while (a&lt;='Z');</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 3.0</strong></p>
<p><strong>C program to print the given number is even or odd.</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a;</p>
<p>printf("Enter any number:");</p>
<p>scanf ("%d", &amp;a);</p>
<p>if(a%2 = = 0)</p>
<p>{</p>
<p>printf("the number is even");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("the number is odd");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 4</p>
<p>the number is even will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li>Mathematical symbol % denote modulus and (a%2 = = 0) is the condition and this condition imply: a divided by 2 yields reminder = 0.</li>
</ul>
<p>&nbsp;</p>
<p><strong>For example:</strong> if you enter the number 4</p>
<p>Then a = 4</p>
<p>Then 4 divided by 2 yields the remainder = 0</p>
<p>Then the statement</p>
<p>{</p>
<p>printf("the number is even");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>the number is even</p>
<p>(Note: in C language = = implies equal to)</p>
<p>&nbsp;</p>
<p>Suppose if you enter the number 3</p>
<p>Then a = 3</p>
<p>Then 3 divided by 2 yields the remainder = 1</p>
<p>Then the statement</p>
<p>{</p>
<p>printf("the number is odd");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>the number is odd</p>
<p>&nbsp;</p>
<table width="242">
<tbody>
<tr>
<td width="134">
<p><strong><em>Data type</em></strong></p>
</td>
<td width="108">
<p><strong><em>Storage size</em></strong></p>
</td>
</tr>
<tr>
<td width="134">
<p><em>char</em></p>
</td>
<td width="108">
<p><em>1 byte</em></p>
</td>
</tr>
<tr>
<td width="134">
<p><em>short int</em></p>
</td>
<td width="108">
<p><em>2 byte</em></p>
</td>
</tr>
<tr>
<td width="134">
<p><em>float, long int</em></p>
</td>
<td width="108">
<p><em>4 byte</em></p>
</td>
</tr>
<tr>
<td width="134">
<p><em>double, long double</em></p>
</td>
<td width="108">
<p><em>8 byte</em></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 3.1</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print the remainder of two numbers </strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;a);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;b);</p>
<p>c = a%b;</p>
<p>printf("the remainder of a and b = %d", c);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>the remainder of a and b = 1 will be outputted on the screen.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Since (a=3 and b=2). Therefore:</p>
<p>3 divided by 2 (i.e., a divided by b) yields the remainder equal to 1</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>printf("the remainder of a and b = %d", c);</p>
<p>is replaced by the statement:</p>
<p>printf("the remainder of %d and %d = %d", a, b, c);</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen is:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>the remainder of 3 and 2 = 1 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 3.2</strong></p>
<p><strong>C program to check the equivalence of two numbers.</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y;</p>
<p>printf("Enter any number:");</p>
<p>scanf ("%d", &amp;x);</p>
<p>printf("Enter any number:");</p>
<p>scanf ("%d", &amp;y);</p>
<p>if(x-y==0)</p>
<p>{</p>
<p>printf("the two numbers are equivalent");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf("the number are not equivalent");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>the two numbers are equivalent will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Since 2-2 is equal to 0 (i.e., x-y = = 0).</p>
<p>Therefore: the statement</p>
<p>{</p>
<p>printf("the two numbers are equivalent");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>two numbers are equivalent</p>
<p>&nbsp;</p>
<p>If you enter the integers 3 and 2</p>
<p>The output on the screen:</p>
<p>the two numbers are not equivalent</p>
<p>&nbsp;</p>
<p>Since 3-2 is not equal to 0 (i.e., x-y != 0). Therefore: the statement</p>
<p>{</p>
<p>printf("the two numbers are not equivalent");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>two numbers are not equivalent</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>(as said earlier: in C language the symbol != implies not equal to)</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the mistake in the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int year;</p>
<p>year =1996;</p>
<p>if(year%4==0)</p>
<p>printf("leap year");</p>
<p>else</p>
<p>printf("not a leap year");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Answer:</p>
<p>&nbsp;</p>
<p>There is no mistake in the above program.<strong> The output on the screen is:</strong></p>
<p>leap year</p>
<p>&nbsp;</p>
<p>Since year=1996. Therefore:</p>
<p>1996 divided by 4 (i.e., year divided by 4) yields the remainder equal to 0.</p>
<p>The statement</p>
<p>&nbsp;</p>
<p>printf("leap year");</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>leap year</p>
<p>If the year is = 1995. Then</p>
<p>1995 divided by 4 (i.e., year divided by 4) yields the remainder not equal to 0.</p>
<p>The statement</p>
<p>&nbsp;</p>
<p>printf("not a leap year");</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p><strong>not a leap year</strong></p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> for a year to be leap year, year divided by 4 should yield remainder = zero.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>&nbsp;</strong></p>
<p><strong>// ----------------------------------------------------------------------------------------------------------------------------------</strong></p>
<p><strong>&nbsp;</strong></p>
<ul>
<li>An algorithm must be seen to be believed.</li>
</ul>
<h2>Donald Knuth</h2>
<h2>&nbsp;</h2>
<h2>You might have an algorithm for getting from office home , for making a chunk of code that calculates the terms of the Fibonacci sequence , or for finding what you're looking for in a retail store . Algorithms are the building blocks of computer programs or a sequence of a sequence of unambiguous instructions ( the term 'unambiguous ' indicates that there is no room for subjective interpretation ) that tells how the problem can be addressed and solved - - which is definitely overblown in their importance like road maps for accomplishing a given , well-defined automated reasoning task - - which always have a clear stopping point . Long division and column addition are examples that everyone is familiar with- even a simple function for adding two numbers is an implementation of a particular algorithm. Online grammar checking uses algorithms . Financial computations use algorithms . A search engine like Google uses search engine algorithms (for example , takes search strings of keywords as input , searches its associated database for relevant web pages , and returns results ) . In fact , it is difficult to think of a task performed by your computer that does not use computer procedures that are a lot like a recipes (called algorithms ) .</h2>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<ul>
<li>The algorithm <strong>to add two numbers entered by user</strong>would look something like this:</li>
<li>Step 1: Start</li>
<li>Step 2: Declare variables num1, num2 and sum.</li>
<li>Step 3: Read values num1 and num2.</li>
<li>Step 4: Add num1 and num2 and assign the result to sum.</li>
</ul>
<p>sum&larr;num1+num2</p>
<ul>
<li>Step 5: Display sum</li>
<li>Step 6: Stop</li>
</ul>
<p>&nbsp;</p>
<p>Algorithms are the heart of computer science (usually means a procedure or basically an instance of logic written in software that solves a recurrent problem of finding an item with specific properties among a collection of items or transforming data according to specified actions to protect it) , and the subject has countless practical applications as well as intellectual depth that is widely used throughout all areas of information technology including solving a mathematical problem (as of finding the greatest common divisor) in a finite number of steps that frequently involves repetition of an operation. The word algorithm - a mathematical concept whose roots date back to 600 AD with the invention of the decimal system -- derives from the name of the Muslim mathematician and astronomer , Mohammed ibn-Musa al-Khwarizmi , who was part with the royal court in Baghdad and who lived from about 780 to 850 . The use of computers , however , has elevated the use of algorithms in daily transactions (like accessing an automated teller machine (ATM) , booking an air or train or buying something online) to unprecedented levels of real-world problems with solutions requiring advanced algorithms abounds. And their use is only likely to grow. Many of the problems, though they may not seem realistic, require the set of well-defined algorithmic knowledge that comes up every day in the real world. By developing a good understanding of a series of logical steps in an algorithmic language, you will be able to choose the right one for a problem and apply it properly.</p>
<p><strong>&nbsp;</strong></p>
<p>The algorithm is written in human readable and understandable form. To search an element in a given array, it can be done in two ways: Linear search and Binary search.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Linear Search:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Linear search is a very basic and simple search algorithm. In this type of search, a sequential search is made over all elements one by one. Every element is checked and if a match is found then that particular element is returned, otherwise the search continues till the end of the data collection.</p>
<p>&nbsp;</p>
<p><strong>For Example:</strong></p>
<p>&nbsp;</p>
<p>To search the element 17 it will go step by step in a sequence order:</p>
<p>&nbsp;</p>
<table width="217">
<tbody>
<tr>
<td width="26">
<p>8</p>
</td>
<td width="30">
<p>10</p>
</td>
<td width="30">
<p>12</p>
</td>
<td width="34">
<p>15</p>
</td>
<td width="30">
<p>17</p>
</td>
<td width="36">
<p>20</p>
</td>
<td width="30">
<p>25</p>
</td>
</tr>
</tbody>
</table>
<p>=</p>
<p>17</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>Match not found</p>
<p>&nbsp;</p>
<table width="217">
<tbody>
<tr>
<td width="26">
<p>8</p>
</td>
<td width="30">
<p>10</p>
</td>
<td width="30">
<p>12</p>
</td>
<td width="34">
<p>15</p>
</td>
<td width="30">
<p>17</p>
</td>
<td width="36">
<p>20</p>
</td>
<td width="30">
<p>25</p>
</td>
</tr>
</tbody>
</table>
<p>=</p>
<p>17</p>
<p>&nbsp;</p>
<p>Match not found</p>
<p>&nbsp;</p>
<table width="217">
<tbody>
<tr>
<td width="26">
<p>8</p>
</td>
<td width="30">
<p>10</p>
</td>
<td width="30">
<p>12</p>
</td>
<td width="34">
<p>15</p>
</td>
<td width="30">
<p>17</p>
</td>
<td width="36">
<p>20</p>
</td>
<td width="30">
<p>25</p>
</td>
</tr>
</tbody>
</table>
<p>=</p>
<p>17</p>
<p>&nbsp;</p>
<p>Match not found</p>
<p>&nbsp;</p>
<table width="217">
<tbody>
<tr>
<td width="26">
<p>8</p>
</td>
<td width="30">
<p>10</p>
</td>
<td width="30">
<p>12</p>
</td>
<td width="34">
<p>15</p>
</td>
<td width="30">
<p>17</p>
</td>
<td width="36">
<p>20</p>
</td>
<td width="30">
<p>25</p>
</td>
</tr>
</tbody>
</table>
<p>=</p>
<p>17</p>
<p>&nbsp;</p>
<p>Match not found</p>
<p>&nbsp;</p>
<table width="217">
<tbody>
<tr>
<td width="26">
<p>8</p>
</td>
<td width="30">
<p>10</p>
</td>
<td width="30">
<p>12</p>
</td>
<td width="34">
<p>15</p>
</td>
<td width="30">
<p>17</p>
</td>
<td width="36">
<p>20</p>
</td>
<td width="30">
<p>25</p>
</td>
</tr>
</tbody>
</table>
<p>=</p>
<p>17</p>
<p>Match found</p>
<p>&nbsp;</p>
<p>Element 17 is returned</p>
<p>&nbsp;</p>
<p>Linear search (whose running time increases linearly with the number of elements in the array. For example if number of elements is doubled then, on average, the search would take twice as long) is rarely used practically because other search algorithms such as the binary search algorithm and hash tables allow significantly faster searching comparison to linear search.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Binary Search</strong></li>
</ul>
<p><a href="http://studytipsandtricks.blogspot.in/2012/08/explanation-of-local-and-global.html">http://studytipsandtricks.blogspot.in/2012/08/explanation-of-local-and-global.html</a></p>
<p>&nbsp;</p>
<p><strong>Local variables:</strong>&nbsp;</p>
<p>Variable whose existence is known only to the main program or functions are called local variables. Local variables are declared with in the main program or a function.</p>
<p>&nbsp;</p>
<p><strong>Global variables:</strong>&nbsp;</p>
<p>Variables whose existence is known to the both main() as well as other functions are called global variables. Global variables are declared outside the main() and other functions.</p>
<p>The following Program illustrates the concept of both local as well as global variables.</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #include&lt;stdio.h&gt;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // Global variables</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; int A;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; int B;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; int Add()</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return A + B;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; int main()</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; int answer; // Local variable</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A = 5;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; B = 7;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; answer = Add();</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; printf("%d\n",answer);</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return 0;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</p>
<p>Consider the following two definitions of main().</p>
<table width="495">
<tbody>
<tr>
<td width="495">
<p>intmain()</p>
<p>{</p>
<p>&nbsp;&nbsp;&nbsp;/*&nbsp; */</p>
<p>&nbsp;&nbsp;&nbsp;return0;</p>
<p>}</p>
</td>
</tr>
</tbody>
</table>
<p>Run on IDE</p>
<p>and</p>
<table width="495">
<tbody>
<tr>
<td width="495">
<p>intmain(void)</p>
<p>{</p>
<p>&nbsp;&nbsp;&nbsp;/*&nbsp; */</p>
<p>&nbsp;&nbsp;&nbsp;return0;</p>
<p>}</p>
</td>
</tr>
</tbody>
</table>
<p>Run on IDE</p>
<p>What is the difference?</p>
<p>In C++, there is no difference, both are same.</p>
<p>Both definitions work in C also, but the second definition with void is considered technically better as it clearly specifies that main can only be called without any parameter.</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main () {</p>
<p>char greeting[6] = {'H', 'e', 'l', 'l', 'o', '\0'};</p>
<p>printf("Greeting message: %s\n", greeting );</p>
<p>return 0;</p>
<p>}</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#define LENGTH 10&nbsp;&nbsp;</p>
<p>#define WIDTH&nbsp; 5</p>
<p>#define NEWLINE '\n'</p>
<p>&nbsp;</p>
<p>int main() {</p>
<p>int area;&nbsp;</p>
<p>area = LENGTH * WIDTH;</p>
<p>printf("value of area : %d", area);</p>
<p>printf("%c", NEWLINE);</p>
<p>return 0;</p>
<p>}</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main(){</p>
<p>constint&nbsp; LENGTH =10;</p>
<p>constint&nbsp; WIDTH =5;</p>
<p>constchar NEWLINE ='\n';</p>
<p>int area;</p>
<p>area = LENGTH * WIDTH;</p>
<p>printf("value of area : %d", area);</p>
<p>printf("%c", NEWLINE);</p>
<p>return0;</p>
<p>}</p>
<p>Note that it is a good programming practice to define constants in CAPITALS.</p>
<p>Binary Search is applied on the sorted array or list. In binary search, we first compare the value with the elements in the middle position of the array. If the value is matched, then we return the value. If the value is less than the middle element, then it must lie in the lower half of the array and if it's greater than the element then it must lie in the upper half of the array. We repeat this procedure on the lower (or upper) half of the array. Binary Search is useful when there are large numbers of elements in an array.</p>
<p>We shall learn the process of binary search with a pictorial example. The following is our sorted array and let us assume that we need to search the location of value 31 using binary search.</p>
<p>First, we shall determine half of the array by using this formula &minus;</p>
<p>mid = low + (high - low) / 2</p>
<p>&nbsp;</p>
<p>Here it is, 0 + (9 - 0 ) / 2 = 4 (integer value of 4.5). So, 4 is the mid of the array.</p>
<p>Now we compare the value stored at location 4, with the value being searched, i.e. 31. We find that the value at location 4 is 27, which is not a match. As the value is greater than 27 and we have a sorted array, so we also know that the target value must be in the upper portion of the array.</p>
<p>We change our low to mid + 1 and find the new mid value again.</p>
<p>low = mid + 1</p>
<p>mid = low + (high - low) / 2</p>
<p>Our new mid is 7 now. We compare the value stored at location 7 with our target value 31.</p>
<p>The value stored at location 7 is not a match, rather it is more than what we are looking for. So, the value must be in the lower part from this location.</p>
<p>Hence, we calculate the mid again. This time it is 5.</p>
<p>We compare the value stored at location 5 with our target value. We find that it is a match.</p>
<p>We conclude that the target value 31 is stored at location 5.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Binary search tree </strong></p>
<p>&nbsp;</p>
<p>Consider a array:</p>
<p>&nbsp;</p>
<p>2</p>
<p>1</p>
<p>3</p>
<p>5</p>
<p>9</p>
<p>12</p>
<p>18</p>
<p>15</p>
<p>19</p>
<p>17</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>12 = root</p>
<p>&nbsp;</p>
<p>Left subtree (lesser)&nbsp; &lt; root</p>
<p>&nbsp;</p>
<p>Right subtree (greater) &gt; root</p>
<p><strong>-------------------------------------------------------------------------------------------------------------------------------- //</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Program 3.3</strong></p>
<p><strong>C program to print whether the given number is positive or negative</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a;</p>
<p>a = -35;</p>
<p>if(a&gt;0)</p>
<p>{</p>
<p>printf("number is positive");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>printf(" number entered is negative");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>number entered is negative</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Since a = -35. Therefore:</p>
<p>a is less than 0 i.e., a &lt; 0 because any negative number is always less than zero.</p>
<p>The statement</p>
<p>{</p>
<p>printf("number is negative");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>number entered is negative</p>
<p>&nbsp;</p>
<p><strong>Program 3.4</strong></p>
<p><strong>C program to print the sum of the first 10 digits using for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>printf("sum of the first 10 digits =%d", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 digits = 55</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>How the sum of the first 10 digits = 55 is outputted on the screen through the for Loop statement?</strong></li>
</ul>
<p>&nbsp;</p>
<p>i=1 (sum = 0 because the sum is initialized to 0 in the statement int i, sum = 0;)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 0 +1 =1</p>
<p>Now,</p>
<p>i=2 (sum = 1)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 1 +2 =3</p>
<p>Now,</p>
<p>i=3 (sum = 3)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 3 +3 = 6</p>
<p>Now,</p>
<p>i=4 (sum = 6)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 6 + 4= 10</p>
<p>Now,</p>
<p>i=5 (sum = 10)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 10 + 5= 15</p>
<p>Now,</p>
<p>i=6 (sum = 15)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 15 + 6 = 21</p>
<p>Now,</p>
<p>i=7 (sum = 21)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 21 + 7 = 28</p>
<p>Now,</p>
<p>i=8 (sum = 28)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 28 + 8 = 36</p>
<p>Now,</p>
<p>i=9 (sum = 36)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 36 + 9 = 45</p>
<p>Now,</p>
<p>i=10 (sum = 45)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>sum = sum + i = 45 + 10 = 55</p>
<p>stops because the condition i&lt;=10 is achieved</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("sum of the first 10 digits =%d", sum);</p>
<p>is executed to print the output:</p>
<p>sum of the first 10 digits = 55</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>int i, sum = 0;</p>
<p>is replaced by int i, sum = 1;</p>
<p>Then the output on the screen is:</p>
<p>sum of the first10 digits = 56</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output if the for loop statement </strong>for(i =1; i&lt;=10; i++)<strong> is replaced by the statement </strong>for(i =2; i&lt;10; i++)<strong>?</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong> sum of 10 digits = 44</p>
<p>If the statement int i, sum, sum = 0; is written instead of int i, sum = 0;</p>
<p>Then the compilation error message will be displayed on the screen (stating that sum is twice declared).</p>
<p>&nbsp;</p>
<p>If the for loop is ended with a semicolon i.e.,</p>
<p>for( i=1; i&lt;=10; i++);</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
<li><em>sum = sum + a; is the same as sum + = a;</em></li>
<li><em>sub = sub- a; is the same as sub - = a;</em></li>
<li><em>product = product* a; is the same as product * = a;</em></li>
<li><em>div = div / a; is the same as div /= a;</em></li>
<li><em>a = a% b; is the same as a % = b;</em></li>
</ul>
<p><em>&nbsp;</em></p>
<p>&nbsp;</p>
<p><strong>Program 3.5</strong></p>
<p><strong>C program to print the average of the first 10 numbers using for loop statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i, avg, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>avg = sum/10;</p>
<p>printf("sum of the first 10 numbers =%d", sum);</p>
<p>printf("average of the first 10 numbers =%d", avg);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 numbers = 55</p>
<p>average of the first 10 numbers = 5</p>
<p>The average of&nbsp; the first10 numbers = 55/10 = 5.5 not 5. But the output on the screen is:</p>
<p>average of the first 10 numbers = 5</p>
<p>because int is used instead of float.</p>
<p>&nbsp;</p>
<p>If the data type float is used i.e.,</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float i, avg, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>avg = sum/10;</p>
<p>printf("sum of the first10 numbers =%f", sum);</p>
<p>printf("average of the first10 numbers = %f", avg);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first10 numbers = 55</p>
<p>average of the first 10 numbers = 5.5</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Program 3.6</strong></p>
<p><strong>C program to print the product of the first 10 digits using for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i, product = 1;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>product = product * i;</p>
<p>printf("the product of the first 10 digits =%d", product);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of the first 10 digits = 3628800</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>How the product of the first 10 digits = 3628800 is outputted on the screen through the for Loop statement?</strong></li>
</ul>
<p>&nbsp;</p>
<p>i=1 (product = 1 because the product is initialized to 1 in the statement int i, product = 1;)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 1 * 1 =1</p>
<p>Now,</p>
<p>i=2 (product = 1)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 1 * 2 = 2</p>
<p>Now,</p>
<p>i=3 (product = 2)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 2 * 3 = 6</p>
<p>Now,</p>
<p>i=4 (product = 6)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 6 * 4 = 24</p>
<p>Now,</p>
<p>i=5 (product =24)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 24 * 5 =120</p>
<p>Now,</p>
<p>i=6 (product =120)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 120 * 6 = 720</p>
<p>Now,</p>
<p>i=7 (product =720)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 720 * 7 = 5040</p>
<p>Now,</p>
<p>i=8 (product =5040)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 5040 * 8 = 40320</p>
<p>Now,</p>
<p>i=9 (product = 40320)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 40320 * 9 = 362880</p>
<p>Now,</p>
<p>i=10 (product = 362880)</p>
<p>Is i&lt;=10 true?</p>
<p>Yes, do this</p>
<p>product = product *&nbsp; i = 362880 * 10 = 3628800</p>
<p>&nbsp;</p>
<p>stops because the condition i&lt;=10 is achieved.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("the product of the first 10 digits =%d", product); is executed to display the output:</p>
<p>the product of the first 10 digits = 3628800</p>
<p>&nbsp;</p>
<p>If the statement int i, product = 1; is replaced by int i, product = 0;</p>
<p>Then the output on the screen is:</p>
<p>the product of the first 10 digits = 0</p>
<p>&nbsp;</p>
<p>If the statement for(i=1; i&lt;=10; i++) is replaced by for(i=5; i&lt;=8; i++)</p>
<p>Then the output on the screen is:</p>
<p>the product of the first 10 digits = 1680</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 3.7</strong></p>
<p><strong>C Program to print the table of a number using the for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int n, i;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;n);</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>printf("%d * %d = %d\n", n, i, n*i);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2 (i.e., n=2)</p>
<p>2 * 1 = 2</p>
<p>2 * 2 = 4</p>
<p>2 * 3 = 6</p>
<p>2 * 4 = 8</p>
<p>2 * 5 = 10</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>How the execution takes its Way through the for Loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>Since you entered the number 2, therefore: n=2.</p>
<p>i=1</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 1 = 2</p>
<p>using the statement printf("%d * %d = %d\n", n, i, n*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 2 = 4</p>
<p>using the statement printf("%d * %d = %d\n", n, i, n*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 3 = 6</p>
<p>using the statement printf("%d * %d = %d\n", n, i, n*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 4 = 8</p>
<p>using the statement printf("%d * %d = %d\n", n, i, n*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=5</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 5 = 10</p>
<p>using the statement printf("%d * %d = %d\n", n, i, n*i);</p>
<p>&nbsp;</p>
<p>stop Now because the condition i &lt;=5 is achieved.</p>
<p>&nbsp;</p>
<p>If the symbol * is replaced by +</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int n, a;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;n);</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>printf("%d + %d = %d\n", n, i, n+ i);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen is:</strong></p>
<p>&nbsp;</p>
<p>Enter any number:</p>
<p>If you enter the number 2 (i.e., n=2)</p>
<p>&nbsp;</p>
<p>2 + 1 = 3</p>
<p>2 + 2 = 4</p>
<p>2 + 3 = 5</p>
<p>2 + 4 = 6</p>
<p>2 + 5 = 7</p>
<p>&nbsp;</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 3.8 </strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program:&nbsp; </strong></p>
<p>If you enter a character M</p>
<p><strong>Output must be:</strong> ch = M</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>printf("Enter any character:");</p>
<p>scanf("%c", &amp;M);</p>
<p>printf("ch=%c", M);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen: </strong></p>
<p>Enter any character:</p>
<p>If you enter the character M</p>
<p>ch = M will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>getchar() function is simplified version of the scanf function</p>
<p>&nbsp;</p>
<p>If we replace the statement scanf("%c", &amp;M); by the statement:</p>
<p>M = getchar();</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>printf("Enter any character:");</p>
<p>M = getchar();</p>
<p>printf("ch=%c", M);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>There will be no change in the output on the screen i.e., <strong>The output on the screen is:</strong></p>
<p>Enter any character:</p>
<p>If you enter the character K</p>
<p>ch = K will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>putchar() function is simplified version of the printf function</p>
<p>If we replace the statement printf("ch=%c", M);by the statement:</p>
<p>putchar (M);&nbsp; i.e.,</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>printf("Enter any character:");</p>
<p>scanf("%c", &amp;M);</p>
<p>putchar (M);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then there will be no change in the output on the screen i.e., <strong>The output on the screen is:</strong></p>
<p>Enter any character:</p>
<p>If you enter the character M</p>
<p>M will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If you replace the statement scanf("%c", &amp;M); by the statement:</p>
<p>M = getchar();</p>
<p>and the statement printf("ch=%c", M);by the statement:</p>
<p>putchar (M);&nbsp; i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>printf("Enter any character:");</p>
<p>M = getchar();</p>
<p>putchar (M);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen: </strong></p>
<p>Enter any character:</p>
<p>If you enter the character S</p>
<p>S will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 3.9 </strong></p>
<p><strong>C program to print the first 5 numbers starting from one together with their squares.</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>printf("number=%d its square=%d\n", i , i*i);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>number=1 its square=1</p>
<p>number=2 its square=4</p>
<p>number=3 its square=9</p>
<p>number=4 its square=16</p>
<p>number=5 its square=25</p>
<p>&nbsp;</p>
<ul>
<li><strong>How the execution takes its way through the for loop statement</strong></li>
</ul>
<p>i=1</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=1 its square=1</p>
<p>using the statement printf("number=%d its square=%d\n", i , i*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=2 its square=4</p>
<p>using the statement printf("number=%d its square=%d\n", i , i*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=3 its square=9</p>
<p>using the statement printf("number=%d its square=%d\n", i , i*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=4 its square=16</p>
<p>using the statement printf("number=%d its square=%d\n", i , i*i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=5</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=5 its square=25</p>
<p>using the statement printf("number=%d its square=%d\n", i , i*i);</p>
<p>&nbsp;</p>
<p>stop Now because the condition (i&lt;=5) is achieved.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>&nbsp;</p>
<p>If the statement</p>
<p>printf("number=%d its square=%d\n", i , i*i);</p>
<p>is replaced by the statement:</p>
<p>printf("\n number=%d/t its square=%d", i , i*i);</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>&nbsp;</p>
<p>number=1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; its square=1</p>
<p>number=2&nbsp;&nbsp;&nbsp;&nbsp; its square=4</p>
<p>number=3&nbsp;&nbsp;&nbsp;&nbsp; its square=9</p>
<p>number=4&nbsp;&nbsp;&nbsp;&nbsp; its square=16</p>
<p>number=5&nbsp;&nbsp;&nbsp;&nbsp; its square=25</p>
<p>&nbsp;</p>
<p>tab /t is included because to leave space between</p>
<p>&nbsp;</p>
<p>number=1&nbsp;&nbsp; and&nbsp;&nbsp; its square=1</p>
<p>&nbsp;</p>
<p>Suppose printf("number=%d its square=%d", a , a*a); is replaced by the statement:</p>
<p>printf("number=%d\n its square=%d\n", a , a*a);</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>number=1</p>
<p>its square=1</p>
<p>number=2</p>
<p>its square=4</p>
<p>number=3</p>
<p>its square=9</p>
<p>number=4</p>
<p>its square=16</p>
<p>number=5</p>
<p>its square=25</p>
<p>&nbsp;</p>
<p>And if you replace the printf statement:</p>
<p>printf("number=%d its square=%d", a , a*a); by the statement:</p>
<p>printf("number=%d\n, its square=%d\n", a , a*a);</p>
<p>i.e., if you place variable separator ( i.e., comma) between number=%d\n and its square=%d\n</p>
<p>Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the first 10 numbers starting from one together with their squares and cubes?</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>printf("number=%d its square=%d its cube=%d\n", i , i*i, i*i*i);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 4.0 </strong></p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>C program to print the sum of two numbers using pointers</strong></li>
</ul>
<p>&nbsp;</p>
<p>If we create an integer variable x by declaring the statement:</p>
<p>int x;</p>
<p>within the body of the main function int main() -- this variable is stored in the computer memory i.e., this variable occupies a specific location in the space of computer memory.</p>
<p>And this integer variable x is assigned an address (i.e., &amp;x) to locate its position in the computer memory (like a house in the street is assigned an address to locate its position in the street).</p>
<p>Pointers are the variables that represent the address of x in the computer memory i.e., p = &amp;x, where &amp;x imply the address of x in the computer memory and p is the pointer variable (which is the variable that represent the address of x in the computer memory).&nbsp;</p>
<p>And further if you assign a value to the variable x by declaring the statement:</p>
<p>x=1;</p>
<p>within the body of the main function&mdash;this value is stored in the address of x in the computer memory. "*" denote pointer operator and *p denote the pointer&nbsp;</p>
<p>(which represent the value stored in the address of x in the computer memory).</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the address of x and the value assigned to x</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, *p;</p>
<p>x = 1;</p>
<p>p = &amp;x;</p>
<p>printf("The address of the variable x =%d", p);</p>
<p>printf("The value of the variable x =%d", *p);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>The address of the variable x = 0x7fffc60478a4</p>
<p>The value of the variable x = 1</p>
<p>Since p = &amp;x:</p>
<p>*p= *&amp;x</p>
<p>The value of the variable x = 1 because you have assigned a value to the variable x by declaring the statement:</p>
<p>x=1;</p>
<p>within the body of the main function.</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>printf("The address of the variable x =%d", p);</p>
<p>printf("The value of the variable x =%d", *p);</p>
<p>are replaced by the statement:</p>
<p>printf("The address of the variable x =%d and its value =%d", p,*p);</p>
<p>i.e.,</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, *p;</p>
<p>x=1;</p>
<p>p = &amp;x;</p>
<p>printf("The address of the variable x =%d and its value =%d", p,*p);</p>
<p>return 0;</p>
<p>}</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>The address of the variable x = 0x7fffc60478a4and its value = 1</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y, *p, *q, sum;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;y);</p>
<p>p = &amp;x;</p>
<p>q = &amp;y;</p>
<p>sum = *p + *q;</p>
<p>printf("Sum of entered numbers = %d\n", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Sum of entered numbers = 5 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Since pointer *p imply the value assigned to the variable x (i.e., 2) through the keyboard and the pointer *q imply the value assigned to the variable y (i.e., 3) through the keyboard. Therefore:</p>
<p>sum = *p + *q = 2 + 3 = 5 (which will be outputted on the screen)</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the product, subtraction and division of two numbers using pointers</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y, *p, *q, product, subtract, div;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;y);</p>
<p>p = &amp;x;</p>
<p>q = &amp;y;</p>
<p>product = *p * *q;</p>
<p>subtract = *p - *q;</p>
<p>div= *p / *q;</p>
<p>printf("product of entered numbers = %d\n", product);</p>
<p>printf("subtract of entered numbers = %d\n", subtract);</p>
<p>printf("division of entered numbers = %d\n", div);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 4</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>product of entered numbers = 8</p>
<p>subtract of entered numbers = 2</p>
<p>division of entered numbers = 2</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to find the greatest of two numbers using pointers</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y, *p, *q;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;y);</p>
<p>p = &amp;x;</p>
<p>q = &amp;y;</p>
<p>if(*p&gt;*q)</p>
<p>{</p>
<p>printf("x is greater than y");</p>
<p>}</p>
<p>if(*q&gt;*p)</p>
<p>{</p>
<p>printf("y is greater than x");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 10</p>
<p>Enter any integer:</p>
<p>If you enter the integer 16</p>
<p>y is greater than x will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the output of the following programs:</strong></li>
</ul>
<p>&nbsp;</p>
<p>i)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x;</p>
<p>x=12;</p>
<p>printf("per = %d%", x);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>per=12</p>
<p>&nbsp;</p>
<p>ii)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, t, c;</p>
<p>x =12;</p>
<p>t = 2;</p>
<p>c = x/t;</p>
<p>printf("velocity = %d m/s", c);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>velocity = 6 m/s</p>
<p>&nbsp;</p>
<p><strong>Program 4.1 </strong></p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>C program to print the sum of two numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int addition();</p>
<p>int main()</p>
<p>{&nbsp;&nbsp;</p>
<p>int answer;</p>
<p>answer = addition();</p>
<p>printf("The sum of two numbers is: %d\n",answer);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>int addition()</p>
<p>{</p>
<p>int x, y;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;y);</p>
<p>return x+y;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Enter any integer:</p>
<p>If you enter the integer 3</p>
<p>Enter any integer:</p>
<p>If you enter the integer 5</p>
<p>sum of two numbers = 8 will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>int addition(); // the statement implies function declaration</p>
<p>&nbsp;</p>
<p>int means integer and int addition() implies: addition() should return integer value.</p>
<p>&nbsp;</p>
<p>int addition()// implies: the function to add the entered values (i.e., 3 and 5) and return the result (i.e., 3 + 5 i.e., 8) to the statement:</p>
<p>printf("sum of two numbers = %d", answer); to</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; make provision to display the output:</p>
<p>sum of two numbers = 8</p>
<p>&nbsp;</p>
<p>{</p>
<p>int x, y;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;y);</p>
<p>return x+y;</p>
<p>} <em>// implies: the body of the function int addition</em>()</p>
<p>&nbsp;</p>
<p>answer = addition(); // implies: the function call i.e., this statement calls the function:</p>
<p>addition()</p>
<p>to add the entered values (i.e., 3 and 5) and return the result (i.e., 3 + 5 i.e., 8)</p>
<p>to the statement:</p>
<p>printf("sum of two numbers = %d", answer);</p>
<p>to make provision to display the output:</p>
<p>sum of two numbers = 8</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>In the statement:</p>
<p>printf("sum of two numbers=%d", answer);</p>
<p>the format string %d indicates that the value to be displayed at that point in the string i.e., after the statement:</p>
<p>sum of two numbers =</p>
<p>needs to be taken from the result returned by the function int addition().</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the product of two numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int multiplication();</p>
<p>int main()</p>
<p>{&nbsp;&nbsp;</p>
<p>int answer;</p>
<p>answer = multiplication();</p>
<p>printf("The product of two numbers is: %d\n",answer);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>int multiplication()</p>
<p>{</p>
<p>int x, y;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;y);</p>
<p>return x*y;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 3</p>
<p>Enter any integer:</p>
<p>If you enter the integer 5</p>
<p>product of two numbers = 15 will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the greatest of two numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int largest();</p>
<p>int main()</p>
<p>{&nbsp;&nbsp;</p>
<p>int answer;</p>
<p>answer = largest();</p>
<p>printf("The largest of two numbers is: %d\n",answer);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>int largest()</p>
<p>{</p>
<p>int x, y;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;y);</p>
<p>if(x&gt;y)</p>
<p>return x;</p>
<p>if(y&gt;x)</p>
<p>return y;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 3</p>
<p>Enter any integer:</p>
<p>If you enter the integer 5</p>
<p>largest of two numbers= 5 will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the greatest of three numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int largest();</p>
<p>int main()</p>
<p>{</p>
<p>&nbsp;</p>
<p>int answer;</p>
<p>answer = largest();&nbsp;</p>
<p>printf("largest of three numbers=%d", answer);</p>
<p>return 0;</p>
<p>}</p>
<p>int largest()</p>
<p>{</p>
<p>int x, y, z;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;y);</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;z);</p>
<p>&nbsp;</p>
<p>if(x&gt;y&amp;&amp; x&gt;z)</p>
<p>return x;</p>
<p>if(y&gt;x&amp;&amp; y &gt; z)</p>
<p>return y;</p>
<p>if(z&gt;x &amp;&amp; z&gt;y)</p>
<p>return z;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 3</p>
<p>Enter any integer:</p>
<p>If you enter the integer 5</p>
<p>Enter any integer:</p>
<p>If you enter the integer 10</p>
<p>largest of three numbers = 10 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the square of the number using functions</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int square();</p>
<p>int main()</p>
<p>{</p>
<p>&nbsp;</p>
<p>int answer;</p>
<p>answer = square();&nbsp;</p>
<p>&nbsp;</p>
<p>printf("square of the given number=%d", answer);</p>
<p>}</p>
<p>int square()</p>
<p>{</p>
<p>int x;</p>
<p>printf("Enter any integer:");</p>
<p>scanf("%d", &amp;x);</p>
<p>return x*x;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>Enter any integer:</p>
<p>If you enter an integer 5</p>
<p>square of the number = 25 will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x;</p>
<p>x=6;</p>
<p>printf("The address of x = %d", &amp;x);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>The address of x = -604171156</p>
<p><strong>Program 4.2</strong></p>
<p><strong><em>Switch (case)</em></strong><em> allows to make decision from the number of choices i.e., <strong>from the number of cases</strong></em></p>
<p>&nbsp;</p>
<p><strong>For example:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch;</p>
<p>printf("Enter any character:");</p>
<p>scanf("%c", &amp;ch);</p>
<p>switch(ch)</p>
<p>{</p>
<p>case 'R':</p>
<p>printf("Red");</p>
<p>break;</p>
<p>case 'W':</p>
<p>printf("White");</p>
<p>break;</p>
<p>case 'Y':</p>
<p>printf("Yellow");</p>
<p>break;</p>
<p>case 'G':</p>
<p>printf("Green");</p>
<p>break;</p>
<p>default:</p>
<p>printf("Error");</p>
<p>break;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any character:</p>
<p>If you enter a character R</p>
<p>Red will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>switch(ch) allow to make decision from the number of choices i.e., from the number of cases</p>
<p>case 'R':</p>
<p>case 'W':</p>
<p>case 'Y':</p>
<p>case 'G':</p>
<p>&nbsp;</p>
<p>Since we have entered the character R (which corresponds to case 'R':)</p>
<p>&nbsp;</p>
<p>The statement</p>
<p>printf("Red");</p>
<p>is executed to display the output:</p>
<p>Red</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>Suppose you enter a character K</p>
<p>&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>Error</p>
<p>&nbsp;</p>
<p>(Entered character K does not correspond to any of the cases:</p>
<p>case 'R':</p>
<p>case 'W':</p>
<p>case 'Y':</p>
<p>case 'G':</p>
<p>Therefore the statement:</p>
<p>printf("Error");</p>
<p>is executed to display the output:</p>
<p>Error</p>
<p>on the screen).</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>&nbsp;</p>
<p>case 'R':</p>
<p>printf("Red");</p>
<p>break;</p>
<p>case 'W':</p>
<p>printf("White");</p>
<p>break;</p>
<p>case 'Y':</p>
<p>printf("Yellow");</p>
<p>break;</p>
<p>case 'G':</p>
<p>printf("Green");</p>
<p>break;</p>
<p>default:</p>
<p>printf("Error");</p>
<p>break;</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>case 'R':</p>
<p>printf("Red");</p>
<p>case 'W':</p>
<p>printf("White");</p>
<p>case 'Y':</p>
<p>printf("Yellow");</p>
<p>break;</p>
<p>case 'G':</p>
<p>printf("Green");</p>
<p>break;</p>
<p>default:</p>
<p>printf("Error");</p>
<p>break;</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>Red</p>
<p>White</p>
<p>Yellow</p>
<p>i.e., the output will be printed till yellow even though you have entered the character R.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 4.3</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print the output:</strong></p>
<p>&nbsp;</p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>&nbsp;</p>
<p><strong>using arrays: </strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>printf("\n Element [%d] = %d", i, num[i]);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>imply that we are creating an integer array (and the name of array is num) consisting of 5 values (i.e., 16, 18, 20, 25, 36) of the same data type int.</p>
<p>The number of values between the braces { } cannot be larger than the number of values that we declare for the array between square brackets [ ].</p>
<p>There are 5 integers i.e., 16, 18, 20, 25, 36 within the braces { }, so 5 is written within the square brackets [ ].</p>
<p>If there were 6 integers i.e., 16, 18, 20, 25, 36, 42 within the braces { }, then 6 must be written within the square brackets [ ].</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> With the declaration int num [5], computer creates 5 memory cells with name num[0], num[1], num[2], num[3], num[4].</li>
</ul>
<p>And since:</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>the values 16, 18, 20, 25, 36 are stored in num[0], num[1], num[2], num[3], num[4] respectively.</p>
<p>&nbsp;</p>
<ul>
<li><strong>How the execution takes its way through the for loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>i=0</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [0] = 16</p>
<p>using the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i])</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=0) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[0] i.e., 16).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=1</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [1] = 18</p>
<p>using the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i])</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=1) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[1] i.e., 18).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [2] = 20</p>
<p>&nbsp;</p>
<p>using the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i])</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=2) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[2] i.e., 20).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [3] = 25</p>
<p>using the statement:&nbsp;</p>
<p>printf("\n Element [%d] = %d", i, num[i])</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=3) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[3] i.e., 25).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [4] = 36</p>
<p>using the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i])</p>
<p>Stop because the condition i&lt;5 is achieved.</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=4) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[4] i.e., 36).</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[0]);</p>
<p>Then the <strong>output on the screen</strong>:</p>
<p>Element [0] = 16</p>
<p>Element [1] = 16</p>
<p>Element [2] = 16</p>
<p>Element [3] = 16</p>
<p>Element [4] = 16</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[1]);</p>
<p><strong>&nbsp;</strong></p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 18</p>
<p>Element [1] = 18</p>
<p>Element [2] = 18</p>
<p>Element [3] = 18</p>
<p>Element [4] = 18</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[2]);</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 20</p>
<p>Element [1] = 20</p>
<p>Element [2] = 20</p>
<p>Element [3] = 20</p>
<p>Element [4] = 20</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[3]);</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 25</p>
<p>Element [1] = 25</p>
<p>Element [2] = 25</p>
<p>Element [3] = 25</p>
<p>Element [4] = 25</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[i]); is replaced by the statement:</p>
<p>printf("\n Element [%d] = %d", i, num[4]);</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 36</p>
<p>Element [1] = 36</p>
<p>Element [2] = 36</p>
<p>Element [3] = 36</p>
<p>Element [4] = 36</p>
<p>&nbsp;</p>
<p>If the condition:</p>
<p>i&lt;5</p>
<p>is replaced by the condition:</p>
<p>i&lt;=5</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>Element [5] = 3656</p>
<p>3656 is the number stored in the memory i.e., any number stored in the memory will be displayed.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int num [5] = {16, 18, 20, 25, 36}; is replaced by the statement:</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; int num [i] = {16, 18, 20, 25, 36};</p>
<p>Then the compilation will be displayed on the screen because there are 5 elements within the braces {} not i elements.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the sum of the elements in array.</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i, sum = 0;</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>sum = sum + num[i];</p>
<p>printf("Sum of the Elements in the array = %d", sum);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Sum of the Elements in the array = 115</p>
<p>i.e., 16 + 18 + 20 + 25 + 36 = 115</p>
<p>&nbsp;</p>
<ul>
<li><strong>How the Execution takes its way through the for loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>i=0 (sum = 0)</p>
<p>Is i&lt;5 true?</p>
<p>Yes, do this</p>
<p>sum = sum + num[i] = sum + num[0] = 0 +16 =16</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=1 (sum = 16)</p>
<p>Is i&lt;5 true?</p>
<p>Yes, do this</p>
<p>sum = sum + num[i] = sum + num[1] = 16 +18 =34</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2 (sum = 34)</p>
<p>Is i&lt;5 true?</p>
<p>Yes, do this</p>
<p>sum = sum + num[i]&nbsp; = sum + num[2] = 34 +20 =54</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3 (sum = 54)</p>
<p>Is i&lt;5 true?</p>
<p>Yes, do this</p>
<p>sum = sum + num[i] = sum + num[3] = 54 +25 =79</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=5 (sum = 79)</p>
<p>Is i&lt;5 true?</p>
<p>Yes, do this</p>
<p>sum = sum + num[i] = sum + num[5] = 79 + 36 =115</p>
<p>stop because the condition i&lt;5 is achieved</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("Sum of the Elements in the array&nbsp; = %d", sum); is executed to display the output:</p>
<p>Sum of the Elements in the array = 115</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int i, sum = 0;</p>
<p>is replaced by int i, sum = 1;</p>
<p>Then The <strong>output on the screen</strong>:</p>
<p>Sum of the Elements in the array = 116</p>
<p>&nbsp;</p>
<ul>
<li><strong>C program to print the average of the elements in array </strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i, avg, sum = 0;</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>sum = sum + num [i];</p>
<p>avg = sum/5;</p>
<p>printf("Sum of the Elements in the array = %d", sum);</p>
<p>printf("average of the elements in the array= %d", avg);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Sum of the Elements in the array = 115</p>
<p>average of the elements in the array = 23</p>
<p>&nbsp;</p>
<p><strong>Write a program to print: </strong></p>
<p>&nbsp;</p>
<p>Einstein [0] = E</p>
<p>Einstein [1] = I</p>
<p>Einstein [2] = N</p>
<p>Einstein [3] = S</p>
<p>Einstein [4] = T</p>
<p>Einstein [5] = E</p>
<p>Einstein [6] = I</p>
<p>Einstein [7] = N</p>
<p>&nbsp;</p>
<p><strong>using arrays</strong></p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>char name [8] = {' E' , ' I', ' N', ' S', ' T ', ' E', ' I', ' N'};</p>
<p>for(i=0; i&lt;8; i++)</p>
<p>printf("\n Element [%d] = %c", i, name[i]);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>If the format string %d is used instead of %c i.e., if the statement:</p>
<p>printf("\n Element [%d] = %c", name[i], name[i]); is written instead of the statement:</p>
<p>printf("\n Element [%c] = %c", name[i], name[i]);</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>&nbsp;</p>
<p>Element [69] = E</p>
<p>Element [73] = I</p>
<p>Element [78] = N</p>
<p>Element [83] = S</p>
<p>Element [84] = T</p>
<p>Element [69] = E</p>
<p>Element [73] = I</p>
<p>Element [78] = N</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following programs?</strong></li>
</ul>
<p>&nbsp;</p>
<p>i)</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include &lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("%f", cbrt(27));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>3.000</p>
<p>&nbsp;</p>
<p>ii)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char i;&nbsp;</p>
<p>char body [4] = {'b', 'o', 'd', 'y'};</p>
<p>for(i=0; i&lt;4; i++)</p>
<p>printf("\n body[%c] = %c", body[i] , body[i]);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>body [b] = b</p>
<p>body [o] = o</p>
<p>body [d] = d</p>
<p>body [y] = y</p>
<p>&nbsp;</p>
<p>iii)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>#include &lt;malloc.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x=2;&nbsp;</p>
<p>printf("%d", malloc ( 200*sizeof(x)));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>8183824</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the mistake in the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>int num [] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>printf("\n Element [%d] = %d", i, num[i]);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong> There is no mistake in the above program. The output on the screen is:</p>
<p>&nbsp;</p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>&nbsp;</p>
<p><strong>Program 4.3</strong></p>
<p><strong>C program to print the output:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Name of the book = B</p>
<p>Price of the book = 135.00</p>
<p>Number of pages = 300</p>
<p>Edition = 8</p>
<p>&nbsp;</p>
<p><strong>using structures </strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>struct book {</p>
<p>char name;</p>
<p>float price;</p>
<p>int pages;</p>
<p>int edition;</p>
<p>};</p>
<p>&nbsp;</p>
<p>struct book b1;</p>
<p>b1.name = 'B';</p>
<p>b1.price = 135.00;</p>
<p>b1.pages = 300;</p>
<p>b1.edition = 8;</p>
<p>printf("\n Name of the book = %c", b1.name);</p>
<p>printf("\n Price of the book = %f", b1.price);</p>
<p>printf("\n Number of pages = %d", b1.pages);</p>
<p>printf("\n Edition of the book = %d", b1.edition);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Name of the book = B</p>
<p>Price of the book = 135.00</p>
<p>Number of pages = 300</p>
<p>Edition of the book = 8</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>&nbsp;</p>
<p>struct book {</p>
<p>char name;</p>
<p>float price;</p>
<p>int pages;</p>
<p>int edition;</p>
<p>};</p>
<p>&nbsp;</p>
<p>imply the structure definition i.e., we are defining a structure (and the data type name of the structure is book) and it consists of elements:</p>
<p>name (which is of data type char), price (which is of data type float), pages (which is of data type int), edition (which is of data type int) &ndash; which are placed within the body of the structure.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>struct book b1;</p>
<p>imply the structure variable declaration (where b1 denote the structure variable)</p>
<p>&nbsp;</p>
<ul>
<li><strong>Why structure variable b1 is declared or defined?</strong></li>
</ul>
<p>&nbsp;</p>
<p>In order to assign the values to the elements within the body of the structure,&nbsp; each element must be linked with structure variable with dot operator or period operator or member accessibility operator.</p>
<p>For example: name is the element which must be linked with structure variable b1 with dot operator to assign a value B to the element &ldquo;name&rdquo;.</p>
<p>&nbsp;</p>
<p>format string %c (corresponding to the data type char) in the statement:</p>
<p>printf("\n Name of the book = %c", b1.name);</p>
<p>indicates that the value to be displayed at that point in the string i.e., after the statement (\n Name of the book = ) needs to be taken from b1.name.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("\n Name of the book = %c", b1.name);</p>
<p>make provision to print the output:</p>
<p>Name of the book = B</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>format string %f (corresponding to the data type float) in the statement:</p>
<p>printf("\n Price of the book = %f", b1.price);</p>
<p>indicates that the value to be displayed at that point in the string i.e., after the statement (\n Price of the book = ) needs to be taken from b1.price.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("\n Price of the book = %f", b1.price);</p>
<p>make provision to print the output:</p>
<p>Price of the book = 135.00</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>format string %d (corresponding to the data type int) in the statement:</p>
<p>printf("\n Number of pages = %d", b1.pages);</p>
<p>indicates that the value to be displayed at that point in the string i.e., after the statement (\n Number of pages = ) needs to be taken from b1.pages.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("\n Number of pages = %d", b1.pages);</p>
<p>make provision to print the output:</p>
<p>Number of pages = 300</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>format string %d (corresponding to the data type int) in the statement:</p>
<p>printf("\n Edition of the book = %d", b1.edition);</p>
<p>indicates that the value to be displayed at that point in the string i.e., after the statement (\n Edition of the book = ) needs to be taken from b1.edition.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>printf("\n Edition of the book = %d", b1.edition);</p>
<p>make provision to print the output:</p>
<p>Edition of the book = 8</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be output of the following programs?</strong></li>
</ul>
<p>&nbsp;</p>
<p>A)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>struct book {</p>
<p>char name;</p>
<p>float price;</p>
<p>int pages;</p>
<p>int edition;</p>
<p>};</p>
<p>int main()</p>
<p>{</p>
<p>struct book b1;</p>
<p>b1.name = 'B';</p>
<p>b1.price = 135.00;</p>
<p>b1.pages = 300;</p>
<p>b1.edition = 8;</p>
<p>printf("\n Name of the book = %c", b1.name);</p>
<p>printf("\n Price of the book = %f", b1.price);</p>
<p>printf("\n Number of pages = %d", b1.pages);</p>
<p>printf("\n Edition of the book = %d", b1.edition);</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>Name of the book = B</p>
<p>Price of the book = 135.000000</p>
<p>Number of pages = 300</p>
<p>Edition of the book = 8</p>
<p>&nbsp;</p>
<p>B)</p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main(){</p>
<p>&nbsp;</p>
<p>for( ; ; ) {</p>
<p>printf("This loop will run forever.\n");</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever. ......... continues</p>
<p>&nbsp;</p>
<ol>
<li>C)</li>
</ol>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char&nbsp; ch [5];</p>
<p>printf( "Enter the name: ");</p>
<p>scanf("%s", &amp;ch);</p>
<p>printf( "the name you entered = %s", ch);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>Enter the name:</p>
<p>If you enter the name Dennis</p>
<p>the name you entered = Denni will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Instead of Dennis, only Denni will be displayed on the screen because of the statement char&nbsp; ch [5];</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>char&nbsp; ch [5];</p>
<p>make provision only for 5 lettered name to be displayed on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>char&nbsp; ch [5]; is replaced by the statement char&nbsp; ch [6];</p>
<p>Then the output on the screen is:</p>
<p>Enter the name:</p>
<p>If you enter the name Dennis</p>
<p>the name you entered = Dennis will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Note: %s implies the format specifier for string.</p>
<p>&nbsp;</p>
<p><strong>Program 4.4</strong></p>
<p><strong>Continue and break statements: </strong></p>
<p>&nbsp;</p>
<ol>
<li>i)</li>
</ol>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i=1; i&lt;=5; i++)</p>
<p>{</p>
<p>if (i==3)</p>
<p>{</p>
<p>continue;</p>
<p>}</p>
<p>&nbsp;</p>
<p>printf("%d\n ", i);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>&nbsp;</p>
<p>1</p>
<p>2</p>
<p>4</p>
<p>5</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>i = 1</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=1</p>
<p>The statement printf("%d\n ", i); is executed to print the output:</p>
<p>1</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 1+1 = 2</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=2</p>
<p>The statement printf("%d\n ", i); is executed to print the output:</p>
<p>2</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 2+1 = 3</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=3</p>
<p>The statement printf("%d\n ", i); <strong>is not executed</strong> to print the output:</p>
<p>3</p>
<p>Because of the statement:</p>
<p>&nbsp;</p>
<p><em>if (i==3)</em></p>
<p><em>{</em></p>
<p><em>continue;</em></p>
<p><em>}</em></p>
<p><em>&nbsp;</em></p>
<p><em>//&nbsp; Execution skips&nbsp; //</em></p>
<p><em>&nbsp;</em></p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 3+1 = 4</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=4</p>
<p>The statement printf("%d\n ", i); is executed to print the output:</p>
<p>4</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 4+1 = 5</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=5</p>
<p>The statement printf("%d\n ", i);&nbsp; is executed to print the output:</p>
<p>5</p>
<p>and stop because the condition i&lt;=5 is achieved.</p>
<p>&nbsp;</p>
<ol>
<li>ii)</li>
</ol>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i=1; i&lt;=5; i++)</p>
<p>{</p>
<p>if (i==3)</p>
<p>{</p>
<p>break;</p>
<p>}</p>
<p>&nbsp;</p>
<p>printf("%d\n ", i);</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>&nbsp;</p>
<p>1</p>
<p>2</p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>i = 1</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=1</p>
<p>The statement printf("%d\n ", i); is executed to print the output:</p>
<p>1</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 1+1 = 2</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=2</p>
<p>The statement printf("%d\n ", i); is executed to print the output:</p>
<p>2</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 2+1 = 3</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=3</p>
<p>The statement printf("%d\n ", i); <strong>is not executed</strong> to print the output:</p>
<p>&nbsp;</p>
<p>Because of the statement:</p>
<p>&nbsp;</p>
<p><em>if (i==3)</em></p>
<p><em>{</em></p>
<p><em>break;</em></p>
<p><em>}</em></p>
<p><em>&nbsp;</em></p>
<p>The for loop:</p>
<p><strong><em>for (i=1; i&lt;=5; i++)</em></strong></p>
<p>&nbsp;</p>
<p>is immediately terminated (even before the condition i&lt;=5 is achieved) and program execution stops.</p>
<p>&nbsp;</p>
<p>//---------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p><strong><em>The goto statement:</em></strong></p>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for(i=1;i&lt;=5;i++)</p>
<p>{</p>
<p>if(i==3)</p>
<p>{</p>
<p>goto HAI;</p>
<p>}</p>
<p>printf("\n %d ",i);</p>
<p>}</p>
<p>&nbsp;</p>
<p>HAI : printf("\n Linux");</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>&nbsp;</p>
<p>1</p>
<p>2</p>
<p>Linux</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>i = 1</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=1</p>
<p>The statement printf("\n %d ",i); is executed to print the output:</p>
<p>1</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 1+1 = 2</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=2</p>
<p>The statement printf("\n %d ",i); is executed to print the output:</p>
<p>2</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 2+1 = 3</p>
<p>Is the condition (i&lt;=5) is true?</p>
<p>Yes because i=3</p>
<p>The statement printf("%d\n ", i); <strong>is not executed</strong> to print the output:</p>
<p>3</p>
<p>&nbsp;</p>
<p>Rather</p>
<p>The statement printf("\n Linux"); is executed to print the output:</p>
<p>&nbsp;</p>
<p>Linux</p>
<p>Because of the statement:</p>
<p>&nbsp;</p>
<p><em>if(i==3)</em></p>
<p><em>{</em></p>
<p><em>goto HAI;</em></p>
<p><em>}</em></p>
<p><em>&nbsp;</em></p>
<p>The for loop:</p>
<p><strong><em>for (i=1; i&lt;=5; i++)</em></strong></p>
<p>&nbsp;</p>
<p>is immediately terminated (even before the condition i&lt;=5 is achieved) and program execution stops.</p>
<p>&nbsp;</p>
<p>---------------------------------------------------------------------------------------------------------------------------//</p>
<p><strong>Program 4.5</strong></p>
<p><strong>C program to convert the upper case letter to lower case letter</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'A';</p>
<p>char b = tolower(ch);</p>
<p>printf("upper case letter %c is converted to lower case letter %c", ch, b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>upper case letter A is converted to lower case letter a</p>
<p>&nbsp;</p>
<p>If you want to enter the character through the keyboard, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch;</p>
<p>printf("Enter any character:");</p>
<p>scanf("%c", &amp;ch);</p>
<p>char b = tolower(ch);</p>
<p>printf("upper case letter %c is converted to lower case letter %c", ch, b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Enter any character:</p>
<p>If you enter the character C</p>
<p>upper case letter C is converted to lower case letter c will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 4.6 </strong></p>
<p><strong>C program to convert the lower case letter to upper case letter</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'a';</p>
<p>char b = toupper(ch);</p>
<p>printf("lower case letter %c is converted to upper case letter %c", ch, b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>lower case letter a is converted to upper case letter A</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to enter the character through the keyboard, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch;</p>
<p>printf("Enter any character:");</p>
<p>scanf("%c", &amp;ch);</p>
<p>char b = toupper(ch);</p>
<p>printf("lower case letter %c is converted to upper case letter %c", ch, b);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Enter any character:</p>
<p>If you enter the character h</p>
<p>lower case letter h is converted to upper case letter H will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 4.7</strong></p>
<p><strong>C program to test whether the entered character is upper case letter or not</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'a';</p>
<p>if(isupper(ch))</p>
<p>printf("you have entered the upper case letter");</p>
<p>else</p>
<p>printf("you have entered the lower case letter");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>you have entered the lower case letter</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>char ch = 'a'; is replaced by the statement:</p>
<p>char ch = 'A';</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>you have entered the upper case letter</p>
<p>&nbsp;</p>
<p><strong>Program 4.8</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to test whether the entered character is lower case letter or not</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'a';</p>
<p>if(islower(ch))</p>
<p>printf("you have entered the lower case letter");</p>
<p>else</p>
<p>printf("you have entered the upper case letter");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>you have entered the lower case letter</p>
<p>&nbsp;</p>
<p><strong>Program 4.9</strong></p>
<p><strong>C program to print the value of tan inverse x (i.e., the value of tan<sup>-1</sup>x)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x = 20;</p>
<p>printf("the value of tan inverse x = %f", atan(x));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the value of tan inverse x = 1.520838</p>
<p>&nbsp;</p>
<p><strong>Program 5.0</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print the value of tan inverse x/y (i.e., the value of tan<sup>-1</sup>x/y)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x,y;</p>
<p>x = 20;</p>
<p>y =20;</p>
<p>printf("the value of tan inverse x/y = %f",&nbsp; atan2(x,y));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the value of tan inverse x/y = 0.785398</p>
<p>&nbsp;</p>
<p><strong>Program 5.1</strong></p>
<p><strong>C program to print the value of fmod(x, y)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float x = 20.500000;</p>
<p>float y =20.799999;</p>
<p>printf("the remainder of %f divided by %f is %f", x, y, fmod(x,y));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the remainder of 20.500000 divided by 20.799999 is 20.500000</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 5.2</strong></p>
<p><strong>C program to print the value of ~x</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y;</p>
<p>x = 205;</p>
<p>y=~x;</p>
<p>printf("the value of y is:%d", y);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the value of y is:-206</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>y=~x; is replaced by the statement:</p>
<p>y= -(~x);</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>the value of y is: 206</p>
<p>&nbsp;</p>
<p><strong>Program 5.3</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print the ASCII (American Standard Code for Information Interchange) value of the entered character</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch ='A';</p>
<p>printf("the ASCII value of ch is: %d", ch);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the ASCII value of ch is: 65</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>printf("the ASCII value of ch is: %d", ch);</p>
<p>is replaced by the statement:</p>
<p>printf("the ASCII value of ch is: %c", ch);</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>the ASCII value of ch is: A</p>
<p>&nbsp;</p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>What will be the output of the following programs:</strong></li>
</ul>
<p>&nbsp;</p>
<p>i)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>int num [5] ={16,18,19,20,21};</p>
<p>for(i=0;i&lt;5;i++)</p>
<p>printf("\n Element = %d", num[i] +1);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>Element = 17</p>
<p>Element = 19</p>
<p>Element = 20</p>
<p>Element = 21</p>
<p>Element = 22</p>
<p>&nbsp;</p>
<p>ii)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i = 54;</p>
<p>int y = i&lt;&lt;1;</p>
<p>printf("The value of y = %d", y);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>The value of y = 108</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>i&lt;&lt;1 is replaced by the statement: i&lt;&lt;2</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>The value of y = 216</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>i&lt;&lt;1 implies 54 * 2 = 108</p>
<p>i&lt;&lt;2 implies 54 * 4 = 216</p>
<p>i&lt;&lt;3 implies 54 * 6 = 324</p>
<p>i&lt;&lt;4 implies 54 * 8 = 432</p>
<p>&nbsp;</p>
<p>iii)</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i = 54;</p>
<p>int y = i&gt;&gt;1;</p>
<p>printf("The value of y = %d", y);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>The value of y = 27</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>i&gt;&gt;1 is replaced by the statement: i&gt;&gt;2</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>The value of y = 13</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>i&gt;&gt;1 implies 54 / 2 = 27</p>
<p>i&gt;&gt;2 implies 54 / 4 = 13</p>
<p>i&gt;&gt;3 implies 54 / 6 = 9</p>
<p>i&gt;&gt;4 implies 54 / 8 = 6</p>
<p>&nbsp;</p>
<p>&lt;&lt; implies: left shift operator</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &gt;&gt; implies: right shift operator</p>
<p>&nbsp;</p>
<p><strong>Program 5.4</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C program to print the length of the entered character (i.e., to print the length of the string)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;string.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>char ch[4];</p>
<p>printf("Enter any word: ");</p>
<p>scanf("%c", &amp;ch);</p>
<p>printf("The length of the string = %d", strlen(ch));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Enter any word:</p>
<p>If you enter the word dog</p>
<p>The length of the string = 3</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; will be displayed on the console screen because there are three letters in the word dog.</p>
<p>&nbsp;</p>
<p>Suppose if you enter the word tech</p>
<p>The length of the string = 4</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; will be displayed on the console screen because there are four letters in the word tech.</p>
<p>&nbsp;</p>
<p><strong>Program 5.5</strong></p>
<p><strong>C program to print the factorial of the entered number</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int i, n, fact=1 ;</p>
<p>printf("Enter any number:");</p>
<p>scanf("%d", &amp;n);</p>
<p>for(i=1; i&lt;=n; i++)</p>
<p>fact = fact *i;</p>
<p>printf("\n Entered number is: %d", n);</p>
<p>printf("\n The factorial of the entered number %d is: %d", n, fact);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Entered number is: 2</p>
<p>The factorial of the entered number 2 is: 2</p>
<p>will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>Suppose if you enter the number 4</p>
<p>Entered number is: 4</p>
<p>The factorial of the entered number 4 is: 24</p>
<p>will be displayed on the screen.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;stdio.h&gt;</p>
<p>int main()</p>
<p>{</p>
<p>printf("\nLinux \' linux ");</p>
<p>printf("\nLinux \? linux ");</p>
<p>return0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>Linux ' linux</p>
<p>Linux ? linux</p>
<p>&nbsp;</p>
<p>#include&lt;stdio.h&gt;</p>
<p>#include&lt;stdlib.h&gt;</p>
<p>int main () {</p>
<p>printf("linux\n");</p>
<p>exit (0);</p>
<p>printf("php\n");</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>linux</p>
<p>&nbsp;</p>
<p><strong>Note: </strong>exit(0) is useful for terminating a program upon having discovered some error which prevents the program from continuing to execute normally. The header file for exit (0); is <strong><em>stdlib.h.</em></strong></p>
