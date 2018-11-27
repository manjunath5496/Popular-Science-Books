
<HTML><HEAD>
<TITLE>Code Repository</TITLE>
<link rel="shortcut icon" href="images/favicon.ico" />


<style>
ul {
    list-style-image: url('images/tick-green.png');
}
</style>

</HEAD>
<P>

<BODY>
<P>
<H3 id="top"><font color="red">Contents</font></H3>
<ul>
<li><a href="#code1" style="text-decoration:none"><font color="#0074B4">Generate Alert Box if user tries to change text in text input field</font></a></li>
						

<li><a href="#code2" style="text-decoration:none"><font color="#0074B4">Show the date and time when the page loads</font></a></li>
	

<li><a href="#code3" style="text-decoration:none"><font color="#0074B4">Animate the background color of a document</font></a></li>

<li><a href="#code4" style="text-decoration:none"><font color="#0074B4">User assignment of a property and dynamic generation of a Web page</font></a></li>
		
<li><a href="#code5" style="text-decoration:none"><font color="#0074B4">Sample Script to Animate Text in Text Field</font></a></li>
		
<li><a href="#code6" style="text-decoration:none"><font color="#0074B4">Using string properties to set characteristics of text on a page</font></a></li>
		
<li><a href="#code7" style="text-decoration:none"><font color="#0074B4">Using Substrings to Generate Scrolling Banners</font></a></li>
<li><a href="#code8" style="text-decoration:none"><font color="#0074B4">What is HTML?</font></a></li>
<li><a href="#code9" style="text-decoration:none"><font color="#0074B4">HTML Fundamentals</font></a></li>
<li><a href="#code15" style="text-decoration:none"><font color="#0074B4">HTML Rules (Lines)</font></a></li>
<li><a href="#code16" style="text-decoration:none"><font color="#0074B4">SQL (Structured Query Language) </font></a></li>
<li><a href="#code17" style="text-decoration:none"><font color="#0074B4">HTML Line Breaks</font></a></li>
<li><a href="#code18" style="text-decoration:none"><font color="#0074B4">Text Formatting</font></a></li>
<li><a href="#code19" style="text-decoration:none"><font color="#0074B4">Preformatted Text</font></a></li>
<li><a href="#code20" style="text-decoration:none"><font color="#0074B4">Computer Output Tags</font></a></li>
<li><a href="#code21" style="text-decoration:none"><font color="#0074B4">Address</font></a></li>

<li><a href="#code22" style="text-decoration:none"><font color="#0074B4">Special HTML codes</font></a></li>
<li><a href="#code23" style="text-decoration:none"><font color="#0074B4">Regular HTML character codes</font></a></li>
<li><a href="#code24" style="text-decoration:none"><font color="#0074B4">Extra codes</font></a></li>
<li><a href="#code25" style="text-decoration:none"><font color="#0074B4">Symbols codes</font></a></li>
<li><a href="#code26" style="text-decoration:none"><font color="#0074B4">Currency codes</font></a></li>
<li><a href="#code27" style="text-decoration:none"><font color="#0074B4">Intellectual property codes</font></a></li>
<li><a href="#code28" style="text-decoration:none"><font color="#0074B4">Greek alphabet codes</font></a></li>
<li><a href="#code29" style="text-decoration:none"><font color="#0074B4">Abbreviations and Acronyms</font></a></li>

<li><a href="#code30" style="text-decoration:none"><font color="#0074B4">Text Direction</font></a></li>
<li><a href="#code31" style="text-decoration:none"><font color="#0074B4">Quotations</font></a></li>
<li><a href="#code32" style="text-decoration:none"><font color="#0074B4">Deleted and Inserted Text</font></a></li>
<li><a href="#code33" style="text-decoration:none"><font color="#0074B4">The HTML Style Attribute</font></a></li>
<li><a href="#code34" style="text-decoration:none"><font color="#0074B4">Background Color</font></a></li>
<li><a href="#code35" style="text-decoration:none"><font color="#0074B4">Font Family, Color, and Size</font></a></li>
<li><a href="#code36" style="text-decoration:none"><font color="#0074B4">Text Alignment</font></a></li>
<li><a href="#code37" style="text-decoration:none"><font color="#0074B4">C Programming</font></a></li>
<li><a href="#code38" style="text-decoration:none"><font color="#0074B4">C++ Programming</font></a></li>
<li><a href="#code39" style="text-decoration:none"><font color="#0074B4">Java Programming</font></a></li>
<li><a href="#code40" style="text-decoration:none"><font color="#0074B4">Linux</font></a></li>
<li><a href="#code41" style="text-decoration:none"><font color="#0074B4">Python</font></a></li>
<li><a href="#code42" style="text-decoration:none"><font color="#0074B4">PHP</font></a></li>
</ul>


		
<HR>
<div id="code1">
<H3>Generate Alert Box if user tries to change text in text input field</H3>
<H3> Code:  </H3>
<XMP><FORM>
<INPUT TYPE="text" VALUE= "dont change" NAME = "leavebutton"
onChange= "alert('Please dont change this')">
</FORM></XMP>
<P>
<H3> Output:  </H3>
<FORM>
<INPUT TYPE="text" VALUE= "dont change" NAME = "leavebutton"
onChange= "alert('Please dont change this')">
</FORM>
</div>

<a href="#top"><font color="#0074B4">Back to top</font></a>




<HR>
<div id="code2">
<H3>Show the date and time when the page loads</H3>
In this example the event handler onLoad is embedded within the <BODY> tag. OnLoad activates
whenever a new page has finished downloading. This alert code tells the browser to create an alert
box containing the value of the variable "today". Thus, it automatically prints out the date and time
when the page has finished loading and requires no special action by the user.
<P>

<XMP><SCRIPT LANGUAGE = "Javascript">
var today= new Date()
</SCRIPT>
....
<BODY onload=alert(today)></XMP>
<P>
<a href="code1.html"><button type="button">Try it Yourself!</button></a>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>


<HR>
<div id="code3">
<H3>Animate the background color of a document</H3>
Notice that the script is not just a series of document.bgColor = commands. You could write that script but the colors would change so quickly that you would not see the animated effect. We need to introduce a delay between each background color change. Javascript offers a setTimeout() method that allows creation of delays as well as serving other functions. 
<P>
The setTimeout() method requires two elements to be enclosed in its parentheses. The first element is an expression to be evaluated or acted upon. The second element is the number of milliseconds (thousandths of a second) to be waited before the first action is undertaken.
<P>
setTimeout(expression to be evaluated, milliseconds)
<P>
<XMP><SCRIPT LANGUAGE= "javascript">

setTimeout("document.bgColor='white'", 1000)
setTimeout("document.bgColor='lightpink'", 1500)
setTimeout("document.bgColor = 'pink'", 2000)
setTimeout("document.bgColor =  'deeppink'", 2500)
setTimeout("document.bgColor = 'red'", 3000)
setTimeout("document.bgColor = 'tomato'", 3500)
setTimeout("document.bgColor = 'darkred'", 4000)
</SCRIPT></XMP>
<P>
<a href="code2.html"><button type="button">Try it Yourself!</button></a>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>


<HR>
<div id="code4">
<H3>User assignment of a property and dynamic generation of a Web page</H3>

<P>

<P>
In the example, which illustrates user assigned properties, a new property is defined for the document object called firstline. Anytime Javascript encounters the expression document.firstline it will produce the assigned text. The fact that I named it "firstline" carries no special meaning to Javascript; that is, it does not know that it is to be the first line in the document. Generally, it is a good idea to name the properties with a name related to your intended use.
<P>
 The rest of the example shows how the write() method can be used to generate text that appears on a web page.  Document.open() prepares for creating a page.  The second open() forces it to appear. 

<XMP><HTML>

<HEAD>
<SCRIPT LANGUAGE = "Javascript">
document.firstline = "Welcome to this page"
</SCRIPT>
<TITLE>load demo</TITLE>
</HEAD>

<BODY>
<SCRIPT>
document.open()
document.write(document.firstline)
document.open()
</SCRIPT>

</BODY>
</HTML></XMP>
<P>
<a href="code3.html"><button type="button">Try it Yourself!</button></a>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>


<HR>
<div id="code5">
<H3>Sample Script to Animate Text in Text Field</H3>

This script will set up a form that asks for user input. It will animate text in boxes that surround it to
urge the user to provide the information. To accomplish this, we must first use standard HTML form
tags to create the input fields for user typing. We must also create text fields that we will use to create
the animation.
<P>
For the sake of illustrating methods of using Javascript to refer to different forms that appear on a
page, the examples presents the information in 3 forms. It could have also been combined into one
form. It places the fields for user input in the middle form called f2 and the fields that will animated
text placed into them into fields f1 on top and f3 on the bottom. Also it places the input elements in
form f1 and f3 into tables in order to gain more control over their placement. f1,f2, and f3 are just
arbitrary names given to the fields. In this example "Answer Soon" text appears and disappears,
moving around the fields from left to right on the top and then from left to right on the bottom. 
<P>
All the code to establish fields and tables should be famiilar to readers with HTML experience. The
new part is the code enclosed in the SCRIPT tags. The heart of these commands are expressions
that assign values to particular fields. For example the code line document.f1.ta1.value = 'Answer
Soon' tells the browser to find the document object (the Web page) and then the form that is a
subelement of it called f1 (the first one on top) and then the subelement of that form called ta.1 (the
first text entry field). Once that element is targeted, the script tells the browser to change the value
property of that text field by assigning it the text "Answer Soon". The Value attribute in standard
HTML markup is the text that a field contains (usually because a user has typed it there.). Javascript
has extended this allow the script to type values. To the user the text appears as in an animation. After
text appears the sample script makes it disappear by assinging the blank value "" to the same text field.

<P>

<XMP><HTML>
<HEAD>
<TITLE> Animated Text</TITLE>
</HEAD>
<BODY>

<FORM NAME="f1">
<TABLE>
<TR> <TD> <INPUT NAME="ta1" TYPE="text" SIZE="20"> 
<TD> <INPUT NAME="ta2" TYPE="text" SIZE="20"> 
<TD> <INPUT NAME="ta3" TYPE="text" SIZE="20">
</TABLE></FORM>



<HR>

<FORM NAME="f2" ACTION="http://netadd.com/nam.cgi" METHOD="POST">
<CENTER>
Name <INPUT NAME="pername" TYPE="text" SIZE="20"> Name<P>
Age <INPUT NAME="perage" TYPE="text" SIZE="5"> Age<P>
Occupation <INPUT NAME="perocc" TYPE="text" SIZE="20">Occupation <P>
<INPUT TYPE="Submit" VALUE="Submit">
<INPUT TYPE="Reset" VALUE="Reset">
</CENTER>
</FORM>

<HR>
<FORM NAME="f3">
<TABLE>
<TR> <TD> <INPUT NAME="ta4" TYPE="text" SIZE="20"> 
<TD> <INPUT NAME="ta5" TYPE="text" SIZE="20"> 
<TD> <INPUT NAME="ta6" TYPE="text" SIZE="20">
</TABLE></FORM>

<SCRIPT LANGUAGE= "javascript">
setTimeout("document.f1.ta1.value = 'Answer Soon'", 1000)
setTimeout("document.f1.ta1.value = ''", 1300)
setTimeout("document.f1.ta2.value = 'Answer Soon'", 1600)
setTimeout("document.f1.ta2.value = ''", 1900)
setTimeout("document.f1.ta3.value = 'Answer Soon'", 2200)
setTimeout("document.f1.ta3.value = ''", 2500)
setTimeout("document.f3.ta4.value = 'Answer Soon'", 2800)
setTimeout("document.f3.ta4.value = ''", 3100)
setTimeout("document.f3.ta5.value = 'Answer Soon'", 3400)
setTimeout("document.f3.ta5.value = ''", 3700)
setTimeout("document.f3.ta6.value = 'Answer Soon'", 4000)
setTimeout("document.f3.ta6.value = ''", 4300)
</SCRIPT> 
</BODY>
</HTML>
</XMP>
<P>

<a href="code4.html"><button type="button">Try it Yourself!</button></a>

</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code6">
<H3>Using string properties to set characteristics of text on a page</H3>
Several properties control the appearance of text on the page.  Note, however, that they cannot control the appearance of text after the page is rendered.  The document must be rewritten for the new characteristics to become visible. This example generates a series of lines, each with a different style,color, or size of text.
<P>
<H3> Code: </H3>
<XMP><SCRIPT>
//assigns value to variable
test ="What is all this?"

// opens document and uses methods to modify text characteristics
document.open()
document.write(test.bold()+"<P>")
document.write(test.fontsize(7)+"<P>")
document.write(test.fontcolor("red")+"<P>")
document.write(test.toUpperCase()+"<P>")

//assigns multiple characteristics to text
document.write(test.italics().fontsize(6).fontcolor("green")+"<P>")
document.open()
</SCRIPT></XMP>
<P>
<H3> Output: </H3>
<SCRIPT>
//assigns value to variable
test ="What is all this?"

// opens document and uses methods to modify text characteristics
document.open()
document.write(test.bold()+"<P>")
document.write(test.fontsize(7)+"<P>")
document.write(test.fontcolor("red")+"<P>")
document.write(test.toUpperCase()+"<P>")

//assigns multiple characteristics to text
document.write(test.italics().fontsize(6).fontcolor("green")+"<P>")
document.open()
</SCRIPT>

</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code7">
<P>
<H3>Using Substrings to Generate Scrolling Banners</H3>


This example uses the subString method to create a scrolling banner in a text field and on the status line of the window. Scrolling text seems to slide from left to right. You can create this effect by systematically displaying a changing section of some target text. For example, if you display character 0 to 24 of some text and next display 1 to 25 and next 2 to 26, the text will appear to be moving from right to left. The sample illustrates a method for accomplishing this effect.
<H3>Code:  </H3>
<XMP><HTML>
<HEAD><TITLE> Banner</TITLE>

<SCRIPT LANGUAGE= "javascript">
// Puts the text to scroll into variable called sent - SECTION A
// uses length propert to assess its length and put into variable slen
// initalizes a,b,n, and subsent variables
var sent = "This is a demonstration of a banner moving from the left to right. It makes use of the substring property of Javascript to make an interesting display"
var slen = sent.length
var siz = 25
var a = -3, b = 0
var subsent = "x"

// Creates a function to capture substrings of sent - SECTION B
function makeSub(a,b) {
subsent = sent.substring(a,b) ;
return subsent;
}

//Creates a function that increments the indexes of the substring - SECTION C 
//each time and calls the makeSub() function to geneate strings
//a indicates start of substring and siz indicates size of string required
function newMake() {
a = a + 3;
b = a + siz
makeSub(a,b);
return subsent
}

//function uses loop to get changing substrings of target - SECTION D
//repeatedly calls newMake to get next substring
//uses setTimeout() command to arrange for substrings to display 
// at specified times
function doIt() {
for (var i = 1; i <= slen ; i++) {
setTimeout("document.z.textdisplay.value = newMake()", i*300);
setTimeout("window.status = newMake()", i*300);
}
}

</SCRIPT> 
</HEAD>

<BODY >
<HR> <CENTER>
<FORM NAME="z">
<INPUT NAME="textdisplay" TYPE="text" SIZE=25> <P>
<INPUT NAME="doit" Type="button" value = "Run Banner" onClick = "doIt()"> 
</FORM></CENTER>

<HR>

</BODY></HTML></XMP>
<P>
<P>

<H3>Output:  </H3>

<HTML>
<HEAD><TITLE> Banner</TITLE>

<SCRIPT LANGUAGE= "javascript">
// Puts the text to scroll into variable called sent - SECTION A
// uses length propert to assess its length and put into variable slen
// initalizes a,b,n, and subsent variables
var sent = "This is a demonstration of a banner moving from the left to right. It makes use of the substring property of Javascript to make an interesting display"
var slen = sent.length
var siz = 25
var a = -3, b = 0
var subsent = "x"

// Creates a function to capture substrings of sent - SECTION B
function makeSub(a,b) {
subsent = sent.substring(a,b) ;
return subsent;
}

//Creates a function that increments the indexes of the substring - SECTION C 
//each time and calls the makeSub() function to geneate strings
//a indicates start of substring and siz indicates size of string required
function newMake() {
a = a + 3;
b = a + siz
makeSub(a,b);
return subsent
}

//function uses loop to get changing substrings of target - SECTION D
//repeatedly calls newMake to get next substring
//uses setTimeout() command to arrange for substrings to display 
// at specified times
function doIt() {
for (var i = 1; i <= slen ; i++) {
setTimeout("document.z.textdisplay.value = newMake()", i*300);
setTimeout("window.status = newMake()", i*300);
}
}

</SCRIPT> 
</HEAD>

<BODY >
<HR> <CENTER>
<FORM NAME="z">
<INPUT NAME="textdisplay" TYPE="text" SIZE=25> <P>
<INPUT NAME="doit" Type="button" value = "Run Banner" onClick = "doIt()"> 
</FORM></CENTER>

<HR>

</BODY></HTML>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code8">
<h3> What is HTML?      </h3>

<p>

Before you continue, you should have a basic understanding of how to use a browser to view pages on the Web.

If you want to study these subjects first, please read <a href="images/pdf1.pdf" style="text-decoration:none"><font color="blue">The Internet For Dummies</font></a>, 12th Edition, from Wiley Publishing.</p>


<ul>
<li> HTML is a language for describing Web pages</li>
<li>HTML stands for HyperText Markup Language </li>

</ul>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code9">
<h3> HTML Fundamentals </h3>



<ul>

<li><a href="#code11" style="text-decoration:none"><font color="blue">HTML Headings</font></a></li>

<li><a href="#code12" style="text-decoration:none"><font color="blue">HTML Paragraphs</font></a></li>

<li><a href="#code13" style="text-decoration:none"><font color="blue">HTML Links</font></a></li>

<li><a href="#code14" style="text-decoration:none"><font color="blue">HTML Images</font></a></li>


</ul>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code11">
<H3>HTML Headings</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<h1>This is Heading 1</h1> 
<h2>Heading 2 is Smaller</h2> 
<h3>Heading 3 is Smaller Still</h3>
</body>
</html>
</XMP>


<H3>Output:</H3>


<html>

<body>

<h1>This is Heading 1</h1> <h2>Heading 2 is Smaller</h2> <h3>Heading 3 is Smaller Still</h3>

</body>

</html>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>

<div id="code12">
<H3>HTML Paragraphs</H3>
<H3> Code: </H3>

<XMP>
<html>
<body>
<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
</body>
</html>
</XMP>
<H3>Output:</H3>
<html>
<body>
<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
<p>This is a paragraph.</p>
</body>
</html>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>

<div id="code13">
<H3>HTML Links</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<a href="http://www.google.com">This is a link to the google Web site.</a>
</body>
</html>
</XMP>
<H3>Output:</H3>
<html>
<body>
<a href="http://www.google.com">This is a link to the google Web site.</a>
</body>
</html>

<H3> Code: </H3>
<XMP>
<html>
<body>
<a href="http://www.google.com" style="text-decoration:none">This is a link to the google Web site.</a>
</body>
</html>
</XMP>
<H3>Output:</H3>
<html>
<body>
<a href="http://www.google.com" style="text-decoration:none">This is a link to the google Web site.</a>
</body>
</html>

<H3> Code: </H3>
<XMP>
<html>
<head>
<style type="text/css">
  a.nounderline {text-decoration: none; }
</style>
</head>
<body>
<a href="http://www.google.com" class="nounderline">This is a link to the google Web site.</a>
</body>
</html>
</XMP>
<H3>Output:</H3>
<html>
<head>
<style type="text/css">
  a.nounderline {text-decoration: none; }
</style>
</head>
<body>
<a href="http://www.google.com" class="nounderline">This is a link to the google Web site.</a>
</body>
</html>

</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code14">
<H3>HTML Images</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<img src="images/img1.jpg" width="295" height="175" />
</body>
</html>
 </XMP>


<H3>Output:</H3>

<html>
<body>
<img src="images/img1.jpg" width="295" height="175" />
</body>
</html>
</div> </br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>

<div id="code15">
<h3> HTML Rules (Lines)      </h3>


<H3> Code: </H3>
<XMP>
<html>
<body>
<p>The hr tag defines a horizontal rule:</p> <hr/>
<p>This is a paragraph</p>
<hr/>
<p>This is a paragraph</p>
<hr/>
<p>This is a paragraph</p>
</body>
</html>
 </XMP>


<H3>Output:</H3>

<html>
<body>
<p>The hr tag defines a horizontal rule:</p> <hr/>
<p>This is a paragraph</p>
<hr/>
<p>This is a paragraph</p>
<hr/>
<p>This is a paragraph</p>
</body>
</html>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code16">

<h3>  <center> SQL (Structured Query Language)</center>      </h3>

</br>
<center> <img src="images/sql.png" alt="Smiley face" height="225" width="300"> </center>
</br>


<a href="images/video.ogg"><font color="#0074B4">SQL Tutorial Video</font></a></br></br>
<a href="0ddb487e-f698-11e7-9f02-0cc47a792c0a_id_0ddb487e-f698-11e7-9f02-0cc47a792c0a.html"><font color="#0074B4">w3Schools SQL Tutorial </font></a>
<XMP>

SQL: Structured Query Language - a computer language developed by American computer scientists 
                  Donald D. Chamberlin and Raymond F. Boyce at IBM in 1974 to create database, store, manipulate, delete and retrieve data stored in database. 

                                          How to create database in MySQL
									
First you have to open MYSQL terminal and then you have to enter the command:

                                               create database data;
                                                       or
                                               CREATE DATABASE data;
											   
And press enter. Then
 
                                            Query OK, 1 row affected (0.01 sec)
											
will be displayed on the console screen indicating that database named data is created. And if you enter the command:

                                                        show databases;

And press enter. Then
 
+--------------------+                                                                                                                                        
| Database           |                                                                                                                                        
+--------------------+                                                                                                                                        
| CODINGGROUND       |                                                                                                                                        
| data               |                                                                                                                                        
| information_schema |                                                                                                                                        
| mysql              |                                                                                                                                        
| performance_schema |                                                                                                                                        
| test               

will be displayed on the console screen. And if you want to create a table in the database "data", then you have to enter the command:
                                                         use data;
And press enter. Then 
                                                     Database changed
will be displayed on the console screen stating that your active database is now "data". And if you want to create a table named "states" with three fields: id, state, and population: 

</XMP>

<center>
<table class="dtable">
		<thead>
		<tr>
			<th><XMP>id</XMP></th>
			<th><XMP>state</XMP></th>
			<th><XMP>population</XMP></th>
			
		</tr>
		</thead>
		<tr>
			<td> </br>  </td>
			<td>   </td>
			<td>   </td>
			
		</tr>
		
	</table>
	</center>

<XMP>
in your active database named "data", then you have to enter the command:

           CREATE TABLE states (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, state CHAR(25), population INT(9));
		   
And press enter. Then
 
                                                 Query OK, 0 rows affected (0.07 sec)

will be displayed on the console screen stating that the above table is created.

Note:
â€¢	The INT command will make the id field contain only numbers (i.e., integers).
â€¢	The NOT NULL command makes sure that the id field cannot be left blank / empty.
â€¢	The PRIMARY KEY designates the id field as the key field in the table.
â€¢	The AUTO_INCREMENT command will automatically assign increasing values into the id field, essentially automatically numbering each entry.
â€¢	The CHAR(characters) and INT(integers) commands designate the types of data allowed in those fields. The number next to the commands CHAR and 
INT indicate how many characters or integers can fit in the field.

Now it's time to start entering your information. Use the following command:

                 INSERT INTO states (id, state, population) VALUES (NULL, 'Karnataka', 256666); 
                 INSERT INTO states (id, state, population) VALUES (NULL, 'Assam', 2568585); 
                 INSERT INTO states (id, state, population) VALUES (NULL, 'Kashmir', 2569);

to input your entry. Then 

                                             Query OK, 1 row affected (0.03 sec)                                                                                                                           
                                                                                                                                                              
                                             Query OK, 1 row affected (0.01 sec)                                                                                                                           
                                                                                                                                                              
                                             Query OK, 1 row affected (0.00 sec)

will be displayed on the console screen stating that you have inputted your entry. And if you enter the following command: 

                                                     select*from states;

Then, your created table named "states" will be displayed on the screen as follows:

+----+-----------+------------+                                                                                                                               
| id | state     | population |                                                                                                                               
+----+-----------+------------+                                                                                                                               
|  1 | Karnataka |     256666 |                                                                                                                               
|  2 | Assam     |    2568585 |                                                                                                                               
|  3 | Kashmir   |       2569 |                                                                                                                               
+----+-----------+------------+  

And if you wish to create the following table: 

+----+-----------+------------+----------+                                                                                                                    
| id | state     | population | language |                                                                                                                    
+----+-----------+------------+----------+                                                                                                                    
|  1 | Karnataka |     256666 | Kannada  |                                                                                                                    
|  2 | Assam     |       2569 | Assami   | 

You have to use the following command:

              CREATE TABLE states (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, state CHAR (25), population INT (9), language CHAR (25));

And press enter and 

                                          Query OK, 0 rows affected (0.03 sec)

will be displayed on the console screen and then you should enter the following command:

            INSERT INTO states (id, state, population, language) VALUES (NULL, 'Karnataka', 256666, 'Kannada'); 
            INSERT INTO states (id, state, population, language) VALUES (NULL,'Assam',2569,'Assami');
			
And press enter and 

                                         Query OK, 1 row affected (0.01 sec)                                                                                                                                                   
                                         Query OK, 1 row affected (0.00 sec)   

will be displayed on the console screen and if you enter the command:

                                                select*from states;

Then the above table will be displayed on the screen.


If you enter the command:

                                      select state, population from states;

Then 

  state          | population |                                                                                                                               
+----------------+------------+                                                                                                                               
| Karnataka      |     256666 |                                                                                                                               
| assam          |       2569 | 

will be displayed on the console screen. And if you enter the command: 

                                          select state from states;

Then 

| state          |                                                                                                                                            
+----------------+                                                                                                                                            
| Karnataka      |                                                                                                                                            
| assam 

will be displayed on the console screen.


If you enter the command:

                               select*from states where language ='kannada';

Then 

+----+-----------+------------+----------+-----------+                                                                                                        
| id | state     | population | language |                                                                                                        
+----+-----------+------------+----------+-----------+                                                                                                        
|  1 | Karnataka |     256666 | kannada  

will be displayed on the console screen. Similarly, if you enter the command:

                                       select*from states where id =2; 

Then

+----+-------+------------+----------+---------+                                                                                                              
| id | state | population | language |                                                                                                             
+----+-------+------------+----------+---------+                                                                                                              
|  2 | assam |       2569 | assami 

will be displayed on the console screen.


                                                  SQL and & or Command:

If you enter the command:
    
                                 select*from states where population = 256666 or language = 'kannada';
Then 

+----+-----------+------------+----------+                                                                                                                    
| id | state     | population | language |                                                                                                                    
+----+-----------+------------+----------+                                                                                                                    
|  1 | Karnataka |     256666 | Kannada  |                                                                                                                    
+----+-----------+------------+----------+ 

will be displayed on the console screen.

If you enter the command:

                                  select *from states where population = 256666 or language ='assami';
								  
+----+-----------+------------+----------+                                                                                                                    
| id | state     | population | language |                                                                                                                    
+----+-----------+------------+----------+                                                                                                                    
|  1 | Karnataka |     256666 | Kannada  |                                                                                                                    
|  2 | assam     |       2569 | assami   |    


                                             HOW to insert information into the table 
											 
If you enter the command:
                    INSERT INTO states (id, state, population, language) VALUES (NULL, 'tamil nadu', 288,'tamil');
Then 

+----+------------+------------+----------+                                                                                                                   
| id | state      | population | language |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
|  1 | Karnataka  |     256666 | Kannada  |                                                                                                                   
|  2 | assam      |       2569 | assami   |                                                                                                                   
|  3 | tamil nadu |        288 | tamil    |                                                                                                                   
+----+------------+------------+----------+ 

will be displayed on the console screen.

                                                          UPDATE INFORMATION:

If you enter the command:
                                 update states set language =' telagu', population = 1 where state ='Karnataka';
Then 
                                        Query OK, 1 row affected (0.01 sec)                                                                                                                           
                                    Rows matched: 1  Changed: 1  Warnings: 0   

will be displayed on the console screen. And if you enter the command:

                                                select*from states;

Then 

+----+------------+------------+----------+                                                                                                                   
| id | state      | population | language |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
|  1 | Karnataka  |          1 |  telagu  |                                                                                                                   
|  2 | assam      |       2569 | assami   |                                                                                                                   
|  3 | tamil nadu |        288 | tamil    |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
3 rows in set (0.00 sec)                    

will be displayed on the console screen.


                                                           DELETE information:
 
If you enter the command:

                                          delete from states where language ='assami' and state ='assam';  
Then
                                                       Query OK, 1 row affected (0.00 sec)
will be displayed on the console screen. And if you enter the command:
                                                                   select*from states;
Then
+----+------------+------------+----------+                                                                                                                   
| id | state      | population | language |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
|  1 | Karnataka  |     256666 | kannada  |                                                                                                                   
|  3 | tamil nadu |        288 | tamil    |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
2 rows in set (0.00 sec)  

will be displayed on the console screen.

                                                        How to delete database in MYSQL:
 
Note: If want to delete database "dbtest" from MySQL.Then you have to enter the command:
                                         drop database dbtest;
Then
                                     Query OK, 1 row affected (0.00 sec)
will be displayed on the console screen stating that database "dbtest" is deleted from MySQL.

If want to delete table "states" from database "dbtest." Then you have to enter the command:

                                                 drop table states;

Then
                                        Query OK, 1 row affected (0.00 sec)
										
will be displayed on the console screen stating that table "states" is deleted from database "dbtest".

                                    Limit Data Selection From MySQL Database:

If enter the command:
                                             select*from states limit 1;
Then

  id | state      | population | language |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
|  1 | Karnataka  |     256666 | Kannada  |                                                                                                                   

will be displayed on the console screen.
 
If enter the command:
                                             select*from states limit 2;
Then

  id | state      | population | language |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
|  1 | Karnataka  |     256666 | Kannada  |                                                                                                                   
|  2 | assam      |       2569 | assami   |                                                                                                                   


will be displayed on the console screen. 

If you enter the following command:
                                               select*from states limit 3;
Then

+----+------------+------------+----------+                                                                                                                   
| id | state      | population | language |                                                                                                                   
+----+------------+------------+----------+                                                                                                                   
|  1 | Karnataka  |     256666 | Kannada  |                                                                                                                   
|  2 | assam      |       2569 | assami   |                                                                                                                   
|  3 | tamil nadu |        288 | tamil    |                                                                                                                   
+----+------------+------------+----------+ 

And if you enter the command:
                                                      truncate states;

Then
                                          Query OK, 0 rows affected (0.06 sec)
will be displayed on the console screen stating that all the rows are removed from the table "states". And you can confirm it by entering the command:
                                                     select*from states;
Then: 
                                                    Empty set (0.01 sec)
will be displayed on the console screen.
                                    

</XMP>

</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>SQL: The Complete Reference</xmp></center></td>
                <td><center><xmp>Paul Weinberg</xmp></center></td>
                <td><a href="img/pdf1.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>Sams Teach Yourself SQL in 24 Hours</xmp></center></td>
                <td><center><xmp>Ryan Stephens</xmp></center></td>
                <td><a href="img/pdf2.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>SQL Cookbook </xmp></center></td>
                <td><center><xmp>Graeme Birchall </xmp></center></td>
                <td><a href="img/pdf3.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>SQL For Dummies</xmp></center></td>
                <td><center><xmp>Allen G. Taylor</xmp></center></td>
                <td><a href="img/pdf4.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Head First SQL</xmp></center></td>
                <td><center><xmp>Lynn Beighley</xmp></center></td>
                <td><a href="img/pdf5.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>SQL in a Nutshell</xmp></center></td>
                <td><center><xmp> Kevin Kline</xmp></center></td>
                <td><a href="img/pdf6.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>The Art of SQL</xmp></center></td>
                <td><center><xmp>Stephane Faroult</xmp></center></td>
                <td><a href="img/pdf7.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>SQL: structured query language</xmp></center></td>
                <td><center><xmp> TutorialsPoint</xmp></center></td>
                <td><a href="img/pdf8.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Learning SQL</xmp></center></td>
                <td><center><xmp>Alan Beaulieu</xmp></center></td>
                <td><a href="img/pdf9.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>SQL Pocket Guide</xmp></center></td>
                <td><center><xmp>Jonathan Gennick</xmp></center></td>
                <td><a href="img/pdf10.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Structured Query Language</xmp></center></td>
                <td><center><xmp>Hans-Petter Halvorsen</xmp></center></td>
                <td><a href="img/pdf11.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>



</br>



</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>


<div id="code17">
<h3> HTML Line Breaks      </h3>


<H3> Code: </H3>

<XMP>
<html>
<body>
<p>This is<br/>a para-<br/>graph with line breaks</p>
</body>
</html>
</XMP>

<H3>Output:</H3>

<html>
<body>
<p>This is<br/>a para-<br/>graph with line breaks</p>
</body>
</html>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>
<div id="code18">
<h3> Text Formatting      </h3>


<H3> Code: </H3>

<XMP>
<html>
<body>
<p><b>This text is bold</b></p> 
<p><strong>This text is strong</strong></p> 
<p><big>This text is big</big></p> 
<p><em>This text is emphasized</em></p> 
<p><i>This text is italic</i></p> 
<p><small>This text is small</small></p>
<p>This is<sub> subscript</sub> and <sup>superscript</sup></ p>
</body>
</html>
</XMP>

<H3>Output:</H3>

<html>
<body>
<p><b>This text is bold</b></p> 
<p><strong>This text is strong</strong></p> 
<p><big>This text is big</big></p> 
<p><em>This text is emphasized</em></p> 
<p><i>This text is italic</i></p> 
<p><small>This text is small</small></p>
<p>This is<sub> subscript</sub> and <sup>superscript</sup></ p>
</body>
</html>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<HR>

<div id="code19">
<h3>Preformatted Text</h3>


<H3> Code: </H3>
<XMP>
<html>
<body>
<pre>
This is
preformatted text.
It preserves	both spaces
and line breaks and shows the text in a monospace font. </pre>
<p>The pre tag is good for displaying computer code:</p>
<pre>
for i = 1 to 10
print i
next i
</pre>
</body>
</html></XMP>

<H3> Output: </H3>

<html>

<body>
<pre>

This is

preformatted text.

It preserves	both spaces

and line breaks and shows the text in a monospace font. </pre>
<p>The pre tag is good for displaying computer code:</p>
<pre>

for i = 1 to 10

print i

next i

</pre>
</body>

</html>
</div>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>

<div id="code20">
<h3>Computer Output Tags</h3>


<H3> Code: </H3>
<XMP>
<html>
<body>
<code>Computer code</code>
<br/>
<kbd>Keyboard input</kbd>
<br/>
<tt>Teletype text</tt>
<br/>
<samp>Sample text</samp>
<br/>
<var>Computer variable</var>
<br/>
<p>
<b>Note:</b> These tags are often used to display computer/ programming code on the page.
</p>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>
<body>
<code>Computer code</code>
<br/>
<kbd>Keyboard input</kbd>
<br/>
<tt>Teletype text</tt>
<br/>
<samp>Sample text</samp>
<br/>
<var>Computer variable</var>
<br/>
<p>
<b>Note:</b> These tags are often used to display computer/ programming code on the page.
</p>
</body>
</html>
</div> </br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code21">
<H3> Address </H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<address>
Donald Duck<br>
BOX 555<br>
Disneyland<br>
USA
</address>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>

<body>

<address>

Donald Duck<br>

BOX 555<br>

Disneyland<br>

USA

</address>

</body>

</html>

</div> </br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>

<br/>

<a href="img/htmlcodes.html" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Character Entity Reference Chart</xmp></center></font> </a>


<br/>



<a href="img/html_codes.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>HTML Character set & entity references pdf</xmp></center></font> </a>


<br/>



<style>
table {
    width:40%;
}
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>
<div id="code22" style="font-family: Corbel">
<h2>Special HTML codes</h2>
	<table class="dtable">
		<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
		</thead>
		<tr>
			<td>&nbsp;</td>
			<td>&amp;#09;</td>
			<td>&nbsp;</td>
			<td>horizontal tab</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&amp;#10;</td>
			<td>&nbsp;</td>
			<td>line feed</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&amp;#13;</td>
			<td>&nbsp;</td>
			<td>carriage return / enter</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&amp;#160;</td>
			<td>&amp;nbsp;</td>
			<td>non-breaking space</td>
		</tr>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
	<div id="code23" style="font-family: Corbel">
	<h3>Regular HTML character codes</h3>
	<table class="dtable">
	<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>&nbsp;</td>
			<td><a id="space"></a>&amp;#32;</td>
			<td>&nbsp;</td>
			<td>space</td>
		</tr>
		<tr>
			<td>!</td>
			<td>&amp;#33;</td>
			<td>&nbsp;</td>
			<td>exclamation mark</td>
		</tr>
		<tr>
			<td>&quot;</td>
			<td>&amp;#34;</td>
			<td>&amp;quot;</td>
			<td>double quote</td>
		</tr>
		<tr>
			<td>#</td>
			<td>&amp;#35;</td>
			<td>&nbsp;</td>
			<td>number</td>
		</tr>
		<tr>
			<td>$</td>
			<td>&amp;#36;</td>
			<td>&nbsp;</td>
			<td>dollar</td>
		</tr>
		<tr>
			<td>%</td>
			<td>&amp;#37;</td>
			<td>&nbsp;</td>
			<td>percent</td>
		</tr>
		<tr>
			<td>&amp;</td>
			<td>&amp;#38;</td>
			<td>&amp;amp;</td>
			<td>ampersand</td>
		</tr>
		<tr>
			<td>'</td>
			<td>&amp;#39;</td>
			<td>&amp;apos;</td>
			<td>single quote</td>
		</tr>
		<tr>
			<td>(</td>
			<td>&amp;#40;</td>
			<td>&nbsp;</td>
			<td>left parenthesis</td>
		</tr>
		<tr>
			<td>)</td>
			<td>&amp;#41;</td>
			<td>&nbsp;</td>
			<td>right parenthesis</td>
		</tr>
		<tr>
			<td>*</td>
			<td>&amp;#42;</td>
			<td>&nbsp;</td>
			<td>asterisk</td>
		</tr>
		<tr>
			<td>+</td>
			<td>&amp;#43;</td>
			<td>&nbsp;</td>
			<td>plus</td>
		</tr>
		<tr>
			<td>,</td>
			<td>&amp;#44;</td>
			<td>&nbsp;</td>
			<td>comma</td>
		</tr>
		<tr>
			<td>-</td>
			<td>&amp;#45;</td>
			<td>&nbsp;</td>
			<td>minus</td>
		</tr>
		<tr>
			<td>.</td>
			<td>&amp;#46;</td>
			<td>&nbsp;</td>
			<td>period</td>
		</tr>
		<tr>
			<td>/</td>
			<td>&amp;#47;</td>
			<td>&nbsp;</td>
			<td>slash</td>
		</tr>
		<tr>
			<td>0</td>
			<td><a id="number"></a> &amp;#48;</td>
			<td>&nbsp;</td>
			<td>zero</td>
		</tr>
		<tr>
			<td>1</td>
			<td>&amp;#49;</td>
			<td>&nbsp;</td>
			<td>one</td>
		</tr>
		<tr>
			<td>2</td>
			<td>&amp;#50;</td>
			<td>&nbsp;</td>
			<td>two</td>
		</tr>
		<tr>
			<td>3</td>
			<td>&amp;#51;</td>
			<td>&nbsp;</td>
			<td>three</td>
		</tr>
		<tr>
			<td>4</td>
			<td>&amp;#52;</td>
			<td>&nbsp;</td>
			<td>four</td>
		</tr>
		<tr>
			<td>5</td>
			<td>&amp;#53;</td>
			<td>&nbsp;</td>
			<td>five</td>
		</tr>
		<tr>
			<td>6</td>
			<td>&amp;#54;</td>
			<td>&nbsp;</td>
			<td>six</td>
		</tr>
		<tr>
			<td>7</td>
			<td>&amp;#55;</td>
			<td>&nbsp;</td>
			<td>seven</td>
		</tr>
		<tr>
			<td>8</td>
			<td>&amp;#56;</td>
			<td>&nbsp;</td>
			<td>eight</td>
		</tr>
		<tr>
			<td>9</td>
			<td>&amp;#57;</td>
			<td>&nbsp;</td>
			<td>nine</td>
		</tr>
		<tr>
			<td>:</td>
			<td>&amp;#58;</td>
			<td>&nbsp;</td>
			<td>colon</td>
		</tr>
		<tr>
			<td>;</td>
			<td>&amp;#59;</td>
			<td>&nbsp;</td>
			<td>semicolon</td>
		</tr>
		<tr>
			<td>&lt;</td>
			<td>&amp;#60;</td>
			<td>&amp;lt;</td>
			<td>less than</td>
		</tr>
		<tr>
			<td>=</td>
			<td>&amp;#61;</td>
			<td>&nbsp;</td>
			<td>equality sign</td>
		</tr>
		<tr>
			<td>&gt;</td>
			<td>&amp;#62;</td>
			<td>&amp;gt;</td>
			<td>greater than</td>
		</tr>
		<tr>
			<td>?</td>
			<td>&amp;#63;</td>
			<td>&nbsp;</td>
			<td>question mark</td>
		</tr>
		<tr>
			<td>@</td>
			<td>&amp;#64;</td>
			<td>&nbsp;</td>
			<td>at sign</td>
		</tr>
		<tr>
			<td>A</td>
			<td>
			<a id="letter"></a>&amp;#65;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>B</td>
			<td>&amp;#66;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>C</td>
			<td>&amp;#67;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>D</td>
			<td>&amp;#68;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>E</td>
			<td>&amp;#69;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>F</td>
			<td>&amp;#70;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>G</td>
			<td>&amp;#71;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>H</td>
			<td>&amp;#72;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>I</td>
			<td>&amp;#73;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>J</td>
			<td>&amp;#74;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>K</td>
			<td>&amp;#75;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>L</td>
			<td>&amp;#76;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>M</td>
			<td>&amp;#77;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>N</td>
			<td>&amp;#78;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>O</td>
			<td>&amp;#79;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>P</td>
			<td>&amp;#80;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Q</td>
			<td>&amp;#81;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>R</td>
			<td>&amp;#82;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>S</td>
			<td>&amp;#83;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>T</td>
			<td>&amp;#84;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>U</td>
			<td>&amp;#85;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>V</td>
			<td>&amp;#86;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>W</td>
			<td>&amp;#87;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>X</td>
			<td>&amp;#88;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Y</td>
			<td>&amp;#89;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>Z</td>
			<td>&amp;#90;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>[</td>
			<td>&amp;#91;</td>
			<td>&nbsp;</td>
			<td>left square bracket</td>
		</tr>
		<tr>
			<td>\</td>
			<td>&amp;#92;</td>
			<td>&nbsp;</td>
			<td>backslash</td>
		</tr>
		<tr>
			<td>]</td>
			<td>&amp;#93;</td>
			<td>&nbsp;</td>
			<td>right square bracket</td>
		</tr>
		<tr>
			<td>^</td>
			<td>&amp;#94;</td>
			<td>&nbsp;</td>
			<td>caret / circumflex</td>
		</tr>
		<tr>
			<td>_</td>
			<td>&amp;#95;</td>
			<td>&nbsp;</td>
			<td>underscore</td>
		</tr>
		<tr>
			<td>`</td>
			<td>&amp;#96;</td>
			<td>&nbsp;</td>
			<td>grave / accent</td>
		</tr>
		<tr>
			<td>a</td>
			<td>&amp;#97;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>b</td>
			<td>&amp;#98;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>c</td>
			<td>&amp;#99;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>d</td>
			<td>&amp;#100;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>e</td>
			<td>&amp;#101;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>f</td>
			<td>&amp;#102;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>g</td>
			<td>&amp;#103;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>h</td>
			<td>&amp;#104;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>i</td>
			<td>&amp;#105;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>j</td>
			<td>&amp;#106;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>k</td>
			<td>&amp;#107;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>l</td>
			<td>&amp;#108;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>m</td>
			<td>&amp;#109;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>n</td>
			<td>&amp;#110;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>o</td>
			<td>&amp;#111;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>p</td>
			<td>&amp;#112;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>q</td>
			<td>&amp;#113;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>r</td>
			<td>&amp;#114;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>s</td>
			<td>&amp;#115;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>t</td>
			<td>&amp;#116;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>u</td>
			<td>&amp;#117</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>v</td>
			<td>&amp;#118;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>w</td>
			<td>&amp;#119;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>x</td>
			<td>&amp;#120;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>y</td>
			<td>&amp;#121;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>z</td>
			<td>&amp;#122;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>{</td>
			<td>&amp;#123;</td>
			<td>&nbsp;</td>
			<td>left curly bracket</td>
		</tr>
		<tr>
			<td>|</td>
			<td>&amp;#124;</td>
			<td>&nbsp;</td>
			<td>vertical bar</td>
		</tr>
		<tr>
			<td>}</td>
			<td>&amp;#125;</td>
			<td>&nbsp;</td>
			<td>right curly bracket</td>
		</tr>
		<tr>
			<td>~</td>
			<td>&amp;#126;</td>
			<td>&nbsp;</td>
			<td>tilde</td>
		</tr>
	</tbody>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
	<div id="code24" style="font-family: Corbel">
	<h2>Extra codes</h2>
	<table class="dtable">
		<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
		</thead>
		<tr>
			<td>&nbsp;</td>
			<td>&amp;#160;</td>
			<td>&amp;nbsp;</td>
			<td>non-breaking space</td>
		</tr>
		<tr>
			<td>&#161;</td>
			<td>&amp;#161;</td>
			<td>&amp;iexcl;</td>
			<td>inverted exclamation mark</td>
		</tr>
		<tr>
			<td>&#162;</td>
			<td>&amp;#162;</td>
			<td>&amp;cent;</td>
			<td>cent sign</td>
		</tr>
		<tr>
			<td>&#163;</td>
			<td>&amp;#163;</td>
			<td>&amp;pound;</td>
			<td>pound sign</td>
		</tr>
		<tr>
			<td>&#164;</td>
			<td>&amp;#164;</td>
			<td>&amp;curren;</td>
			<td>currency sign</td>
		</tr>
		<tr>
			<td>&#165;</td>
			<td>&amp;#165;</td>
			<td>&amp;yen;</td>
			<td>yen sign</td>
		</tr>
		<tr>
			<td>&#166;</td>
			<td>&amp;#166;</td>
			<td>&amp;brvbar;</td>
			<td>broken bar</td>
		</tr>
		<tr>
			<td>&#167;</td>
			<td>&amp;#167;</td>
			<td>&amp;sect;</td>
			<td>section sign</td>
		</tr>
		<tr>
			<td>&#168;</td>
			<td>&amp;#168;</td>
			<td>&amp;uml;</td>
			<td>diaeresis</td>
		</tr>
		<tr>
			<td>&#169;</td>
			<td>&amp;#169;</td>
			<td>&amp;copy;</td>
			<td>copyright sign</td>
		</tr>
		<tr>
			<td>&#170;</td>
			<td>&amp;#170;</td>
			<td>&amp;ordf;</td>
			<td>feminine ordinal indicator</td>
		</tr>
		<tr>
			<td>&#171;</td>
			<td>&amp;#171;</td>
			<td>&amp;laquo;</td>
			<td>left pointing guillemet</td>
		</tr>
		<tr>
			<td>&#172;</td>
			<td>&amp;#172;</td>
			<td>&amp;not;</td>
			<td>not sign</td>
		</tr>
		<tr>
			<td>&#173;</td>
			<td>&amp;#173;</td>
			<td>&amp;shy;</td>
			<td>soft hyphen</td>
		</tr>
		<tr>
			<td>&#174;</td>
			<td>&amp;#174;</td>
			<td>&amp;reg;</td>
			<td>registered sign</td>
		</tr>
		<tr>
			<td>&#175;</td>
			<td>&amp;#175;</td>
			<td>&amp;macr;</td>
			<td>macron</td>
		</tr>
		<tr>
			<td>&#176;</td>
			<td>&amp;#176;</td>
			<td>&amp;deg;</td>
			<td>degree sign</td>
		</tr>
		<tr>
			<td>&#177;</td>
			<td>&amp;#177;</td>
			<td>&amp;plusmn;</td>
			<td>plus-minus sign</td>
		</tr>
		<tr>
			<td>&#178;</td>
			<td>&amp;#178;</td>
			<td>&amp;sup2;</td>
			<td>superscript two</td>
		</tr>
		<tr>
			<td>&#179;</td>
			<td>&amp;#179;</td>
			<td>&amp;sup3;</td>
			<td>superscript three</td>
		</tr>
		<tr>
			<td>&#180;</td>
			<td>&amp;#180;</td>
			<td>&amp;acute;</td>
			<td>acute accent</td>
		</tr>
		<tr>
			<td>&#181;</td>
			<td>&amp;#181;</td>
			<td>&amp;micro;</td>
			<td>micro sign</td>
		</tr>
		<tr>
			<td>&#182;</td>
			<td>&amp;#182;</td>
			<td>&amp;para;</td>
			<td>paragraph sign</td>
		</tr>
		<tr>
			<td>&#183;</td>
			<td>&amp;#183;</td>
			<td>&amp;middot;</td>
			<td>middle dot</td>
		</tr>
		<tr>
			<td>&#184;</td>
			<td>&amp;#184;</td>
			<td>&amp;cedil;</td>
			<td>spacing cedilla</td>
		</tr>
		<tr>
			<td>&#185;</td>
			<td>&amp;#185;</td>
			<td>&amp;sup1;</td>
			<td>superscript one</td>
		</tr>
		<tr>
			<td>&#186;</td>
			<td>&amp;#186;</td>
			<td>&amp;ordm;</td>
			<td>masculine ordinal indicator</td>
		</tr>
		<tr>
			<td>&#187;</td>
			<td>&amp;#187;</td>
			<td>&amp;raquo;</td>
			<td>right pointing guillemet</td>
		</tr>
		<tr>
			<td>&#188;</td>
			<td>&amp;#188;</td>
			<td>&amp;frac14;</td>
			<td>fraction one quarter</td>
		</tr>
		<tr>
			<td>&#189;</td>
			<td>&amp;#189;</td>
			<td>&amp;frac12;</td>
			<td>fraction one half</td>
		</tr>
		<tr>
			<td>&#190;</td>
			<td>&amp;#190;</td>
			<td>&amp;frac34;</td>
			<td>fraction three quarters</td>
		</tr>
		<tr>
			<td>&#191;</td>
			<td>&amp;#191;</td>
			<td>&amp;iquest;</td>
			<td>inverted question mark</td>
		</tr>
		<tr>
			<td>&#192;</td>
			<td>&amp;#192;</td>
			<td>&amp;Agrave;</td>
			<td>&nbsp;capital&nbsp; A with grave</td>
		</tr>
		<tr>
			<td>&#193;</td>
			<td>&amp;#193;</td>
			<td>&amp;Aacute;</td>
			<td>&nbsp;capital&nbsp; A with acute</td>
		</tr>
		<tr>
			<td>&#194;</td>
			<td>&amp;#194;</td>
			<td>&amp;Acirc;</td>
			<td>&nbsp;capital&nbsp; A with circumflex</td>
		</tr>
		<tr>
			<td>&#195;</td>
			<td>&amp;#195;</td>
			<td>&amp;Atilde;</td>
			<td>&nbsp;capital&nbsp; A with tilde</td>
		</tr>
		<tr>
			<td>&#196;</td>
			<td>&amp;#196;</td>
			<td>&amp;Auml;</td>
			<td>&nbsp;capital&nbsp; A with diaeresis</td>
		</tr>
		<tr>
			<td>&#197;</td>
			<td>&amp;#197;</td>
			<td>&amp;Aring;</td>
			<td>&nbsp;capital&nbsp; A with ring</td>
		</tr>
		<tr>
			<td>&#198;</td>
			<td>&amp;#198;</td>
			<td>&amp;AElig;</td>
			<td>&nbsp;capital&nbsp; AE</td>
		</tr>
		<tr>
			<td>&#199;</td>
			<td>&amp;#199;</td>
			<td>&amp;Ccedil;</td>
			<td>&nbsp;capital&nbsp; C with cedilla</td>
		</tr>
		<tr>
			<td>&#200;</td>
			<td>&amp;#200;</td>
			<td>&amp;Egrave;</td>
			<td>&nbsp;capital&nbsp; E with grave</td>
		</tr>
		<tr>
			<td>&#201;</td>
			<td>&amp;#201;</td>
			<td>&amp;Eacute;</td>
			<td>&nbsp;capital&nbsp; E with acute</td>
		</tr>
		<tr>
			<td>&#202;</td>
			<td>&amp;#202;</td>
			<td>&amp;Ecirc;</td>
			<td>&nbsp;capital&nbsp; E with circumflex</td>
		</tr>
		<tr>
			<td>&#203;</td>
			<td>&amp;#203;</td>
			<td>&amp;Euml;</td>
			<td>&nbsp;capital&nbsp; E with diaeresis</td>
		</tr>
		<tr>
			<td>&#204;</td>
			<td>&amp;#204;</td>
			<td>&amp;Igrave;</td>
			<td>&nbsp;capital&nbsp; I with grave</td>
		</tr>
		<tr>
			<td>&#205;</td>
			<td>&amp;#205;</td>
			<td>&amp;Iacute;</td>
			<td>&nbsp;capital&nbsp; I with acute</td>
		</tr>
		<tr>
			<td>&#206;</td>
			<td>&amp;#206;</td>
			<td>&amp;Icirc;</td>
			<td>&nbsp;capital&nbsp; I with circumflex</td>
		</tr>
		<tr>
			<td>&#207;</td>
			<td>&amp;#207;</td>
			<td>&amp;Iuml;</td>
			<td>&nbsp;capital&nbsp; I with diaeresis</td>
		</tr>
		<tr>
			<td>&#208;</td>
			<td>&amp;#208;</td>
			<td>&amp;ETH;</td>
			<td>&nbsp;capital&nbsp; ETH</td>
		</tr>
		<tr>
			<td>&#209;</td>
			<td>&amp;#209;</td>
			<td>&amp;Ntilde;</td>
			<td>&nbsp;capital&nbsp; N with tilde</td>
		</tr>
		<tr>
			<td>&#210;</td>
			<td>&amp;#210;</td>
			<td>&amp;Ograve;</td>
			<td>&nbsp;capital&nbsp; O with grave</td>
		</tr>
		<tr>
			<td>&#211;</td>
			<td>&amp;#211;</td>
			<td>&amp;Oacute;</td>
			<td>&nbsp;capital&nbsp; O with acute</td>
		</tr>
		<tr>
			<td>&#212;</td>
			<td>&amp;#212;</td>
			<td>&amp;Ocirc;</td>
			<td>&nbsp;capital&nbsp; O with circumflex</td>
		</tr>
		<tr>
			<td>&#213;</td>
			<td>&amp;#213;</td>
			<td>&amp;Otilde;</td>
			<td>&nbsp;capital&nbsp; O with tilde</td>
		</tr>
		<tr>
			<td>&#214;</td>
			<td>&amp;#214;</td>
			<td>&amp;Ouml;</td>
			<td>&nbsp;capital&nbsp; O with diaeresis</td>
		</tr>
		<tr>
			<td>&#215;</td>
			<td>&amp;#215;</td>
			<td>&amp;times;</td>
			<td>multiplication sign</td>
		</tr>
		<tr>
			<td>&#216;</td>
			<td>&amp;#216;</td>
			<td>&amp;Oslash;</td>
			<td>&nbsp;capital&nbsp; O with stroke</td>
		</tr>
		<tr>
			<td>&#217;</td>
			<td>&amp;#217;</td>
			<td>&amp;Ugrave;</td>
			<td>&nbsp;capital&nbsp; U with grave</td>
		</tr>
		<tr>
			<td>&#218;</td>
			<td>&amp;#218;</td>
			<td>&amp;Uacute;</td>
			<td>&nbsp;capital&nbsp; U with acute</td>
		</tr>
		<tr>
			<td>&#219;</td>
			<td>&amp;#219;</td>
			<td>&amp;Ucirc;</td>
			<td>&nbsp;capital&nbsp; U with circumflex</td>
		</tr>
		<tr>
			<td>&#220;</td>
			<td>&amp;#220;</td>
			<td>&amp;Uuml;</td>
			<td>&nbsp;capital&nbsp; U with diaeresis</td>
		</tr>
		<tr>
			<td>&#221;</td>
			<td>&amp;#221;</td>
			<td>&amp;Yacute;</td>
			<td>&nbsp;capital&nbsp; Y with acute</td>
		</tr>
		<tr>
			<td>&#222;</td>
			<td>&amp;#222;</td>
			<td>&amp;THORN;</td>
			<td>&nbsp;capital&nbsp; THORN</td>
		</tr>
		<tr>
			<td>&#223;</td>
			<td>&amp;#223;</td>
			<td>&amp;szlig;</td>
			<td>&nbsp;small&nbsp; sharp s</td>
		</tr>
		<tr>
			<td>&#224;</td>
			<td>&amp;#224;</td>
			<td>&amp;agrave;</td>
			<td>&nbsp;small&nbsp; a with grave</td>
		</tr>
		<tr>
			<td>&#225;</td>
			<td>&amp;#225;</td>
			<td>&amp;aacute;</td>
			<td>&nbsp;small&nbsp; a with acute</td>
		</tr>
		<tr>
			<td>&#226;</td>
			<td>&amp;#226;</td>
			<td>&amp;;</td>
			<td>&nbsp;small&nbsp; a with circumflex</td>
		</tr>
		<tr>
			<td>&#227;</td>
			<td>&amp;#227;</td>
			<td>&amp;atilde;</td>
			<td>&nbsp;small&nbsp; a with tilde</td>
		</tr>
		<tr>
			<td>&#228;</td>
			<td>&amp;#228;</td>
			<td>&amp;auml;</td>
			<td>&nbsp;small&nbsp; a with diaeresis</td>
		</tr>
		<tr>
			<td>&#229;</td>
			<td>&amp;#229;</td>
			<td>&amp;aring;</td>
			<td>&nbsp;small&nbsp; a with ring above</td>
		</tr>
		<tr>
			<td>&#230;</td>
			<td>&amp;#230;</td>
			<td>&amp;aelig;</td>
			<td>&nbsp;small&nbsp; ae</td>
		</tr>
		<tr>
			<td>&#231;</td>
			<td>&amp;#231;</td>
			<td>&amp;ccedil;</td>
			<td>&nbsp;small&nbsp; c with cedilla</td>
		</tr>
		<tr>
			<td>&#232;</td>
			<td>&amp;#232;</td>
			<td>&amp;egrave;</td>
			<td>&nbsp;small&nbsp; e with grave</td>
		</tr>
		<tr>
			<td>&#233;</td>
			<td>&amp;#233;</td>
			<td>&amp;eacute;</td>
			<td>&nbsp;small&nbsp; e with acute</td>
		</tr>
		<tr>
			<td>&#234;</td>
			<td>&amp;#234;</td>
			<td>&amp;ecirc;</td>
			<td>&nbsp;small&nbsp; e with circumflex</td>
		</tr>
		<tr>
			<td>&#235;</td>
			<td>&amp;#235;</td>
			<td>&amp;euml;</td>
			<td>&nbsp;small&nbsp; e with diaeresis</td>
		</tr>
		<tr>
			<td>&#236;</td>
			<td>&amp;#236;</td>
			<td>&amp;igrave;</td>
			<td>&nbsp;small&nbsp; i with grave</td>
		</tr>
		<tr>
			<td>&#237;</td>
			<td>&amp;#237;</td>
			<td>&amp;iacute;</td>
			<td>&nbsp;small&nbsp; i with acute</td>
		</tr>
		<tr>
			<td>&#238;</td>
			<td>&amp;#238;</td>
			<td>&amp;icirc;</td>
			<td>&nbsp;small&nbsp; i with circumflex</td>
		</tr>
		<tr>
			<td>&#239;</td>
			<td>&amp;#239;</td>
			<td>&amp;iuml;</td>
			<td>&nbsp;small&nbsp; i with diaeresis</td>
		</tr>
		<tr>
			<td>&#240;</td>
			<td>&amp;#240;</td>
			<td>&amp;eth;</td>
			<td>&nbsp;small&nbsp; eth</td>
		</tr>
		<tr>
			<td>&#241;</td>
			<td>&amp;#241;</td>
			<td>&amp;ntilde;</td>
			<td>&nbsp;small&nbsp; n with tilde</td>
		</tr>
		<tr>
			<td>&#242;</td>
			<td>&amp;#242;</td>
			<td>&amp;ograve;</td>
			<td>&nbsp;small&nbsp; o with grave</td>
		</tr>
		<tr>
			<td>&#243;</td>
			<td>&amp;#243;</td>
			<td>&amp;oacute;</td>
			<td>&nbsp;small&nbsp; o with acute</td>
		</tr>
		<tr>
			<td>&#244;</td>
			<td>&amp;#244;</td>
			<td>&amp;ocirc;</td>
			<td>&nbsp;small&nbsp; o with circumflex</td>
		</tr>
		<tr>
			<td>&#245;</td>
			<td>&amp;#245;</td>
			<td>&amp;otilde;</td>
			<td>&nbsp;small&nbsp; o with tilde</td>
		</tr>
		<tr>
			<td>&#246;</td>
			<td>&amp;#246;</td>
			<td>&amp;ouml;</td>
			<td>&nbsp;small&nbsp; o with diaeresis</td>
		</tr>
		<tr>
			<td>&#247;</td>
			<td>&amp;#247;</td>
			<td>&amp;divide;</td>
			<td>division sign</td>
		</tr>
		<tr>
			<td>&#248;</td>
			<td>&amp;#248;</td>
			<td>&amp;oslash;</td>
			<td>&nbsp;small&nbsp; o with stroke</td>
		</tr>
		<tr>
			<td>&#249;</td>
			<td>&amp;#249;</td>
			<td>&amp;ugrave;</td>
			<td>&nbsp;small&nbsp; u with grave</td>
		</tr>
		<tr>
			<td>&#250;</td>
			<td>&amp;#250;</td>
			<td>&amp;uacute;</td>
			<td>&nbsp;small&nbsp; u with acute</td>
		</tr>
		<tr>
			<td>&#251;</td>
			<td>&amp;#251;</td>
			<td>&amp;ucirc;</td>
			<td>&nbsp;small&nbsp; u with circumflex</td>
		</tr>
		<tr>
			<td>&#252;</td>
			<td>&amp;#252;</td>
			<td>&amp;uuml;</td>
			<td>&nbsp;small&nbsp; u with diaeresis</td>
		</tr>
		<tr>
			<td>&#253;</td>
			<td>&amp;#253;</td>
			<td>&amp;yacute;</td>
			<td>&nbsp;small&nbsp; y with acute</td>
		</tr>
		<tr>
			<td>&#254;</td>
			<td>&amp;#254;</td>
			<td>&amp;thorn;</td>
			<td>&nbsp;small&nbsp; thorn</td>
		</tr>
		<tr>
			<td>&#255;</td>
			<td>&amp;#255;</td>
			<td>&amp;yuml;</td>
			<td>&nbsp;small&nbsp; y with diaeresis</td>
		</tr>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
	<div id="code25" style="font-family: Corbel">
	<h2>Symbols codes</h2>
	<table class="dtable">
		<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
		</thead>
		<tr>
			<td>&amp;</td>
			<td>&amp;#38;</td>
			<td>&amp;amp;</td>
			<td>ampersand</td>
		</tr>
		<tr>
			<td>&bull;</td>
			<td>&amp;#8226;</td>
			<td>&amp;bull;</td>
			<td>bullet</td>
		</tr>
		<tr>
			<td>&#9702;</td>
			<td>&amp;#9702;</td>
			<td>&nbsp;</td>
			<td>white bullet</td>
		</tr>
		<tr>
			<td>&#8729;</td>
			<td>&amp;#8729;</td>
			<td>&nbsp;</td>
			<td>bullet operator</td>
		</tr>
		<tr>
			<td>&#8227;</td>
			<td>&amp;#8227;</td>
			<td>&nbsp;</td>
			<td>triangular bullet</td>
		</tr>
		<tr>
			<td>&#8259;</td>
			<td>&amp;#8259;</td>
			<td>&nbsp;</td>
			<td>hyphen bullet</td>
		</tr>
		<tr>
			<td>&deg;</td>
			<td>&amp;#176;</td>
			<td>&amp;deg;</td>
			<td>degree</td>
		</tr>
		<tr>
			<td>&#8734;</td>
			<td>&amp;#8734;</td>
			<td>&amp;infin;</td>
			<td>infinity</td>
		</tr>
		<tr>
			<td>&permil;</td>
			<td>&amp;#8240;</td>
			<td>&amp;permil;</td>
			<td>per-mille</td>
		</tr>
		<tr>
			<td>&sdot;</td>
			<td>&amp;#8901;</td>
			<td>&amp;sdot;</td>
			<td>multiplication dot</td>
		</tr>
		<tr>
			<td>&plusmn;</td>
			<td>&amp;#177;</td>
			<td>&amp;plusmn;</td>
			<td>plus-minus</td>
		</tr>
		<tr>
			<td>&dagger;</td>
			<td>&amp;#8224;</td>
			<td>&amp;dagger;</td>
			<td>hermitian</td>
		</tr>
		<tr>
			<td>&mdash;</td>
			<td>&amp;#8212;</td>
			<td>&amp;mdash;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&not;</td>
			<td>&amp;#172;</td>
			<td>&amp;not;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&micro;</td>
			<td>&nbsp;</td>
			<td>&amp;micro;</td>
			<td>&nbsp;</td>
		</tr>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
	<div id="code26" style="font-family: Corbel">
	<h2>Currency codes</h2>
	<table class="dtable">
		<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
		</thead>
		<tr>
			<td>$</td>
			<td>&amp;#36;</td>
			<td>&nbsp;</td>
			<td>dollar</td>
		</tr>
		<tr>
			<td>&euro;</td>
			<td>&amp;#8364;</td>
			<td>&amp;euro;</td>
			<td>euro</td>
		</tr>
		<tr>
			<td>&pound;</td>
			<td>&amp;#163;</td>
			<td>&amp;pound;</td>
			<td>pound</td>
		</tr>
		<tr>
			<td>&yen;</td>
			<td>&amp;#165;</td>
			<td>&amp;yen;</td>
			<td>yen / yuan</td>
		</tr>
		<tr>
			<td>&cent;</td>
			<td>&amp;#162;</td>
			<td>&amp;cent;</td>
			<td>cent</td>
		</tr>
		<tr>
			<td>&#8377;</td>
			<td>&amp;#8377;</td>
			<td>&nbsp;</td>
			<td>indean Rupee</td>
		</tr>
		<tr>
			<td>&#8360;</td>
			<td>&amp;#8360;</td>
			<td>&nbsp;</td>
			<td>rupee</td>
		</tr>
		<tr>
			<td>&#8369;</td>
			<td>&amp;#8369;</td>
			<td>&nbsp;</td>
			<td>peso</td>
		</tr>
		<tr>
			<td>&#8361;</td>
			<td>&amp;#8361;</td>
			<td>&nbsp;</td>
			<td>korean won</td>
		</tr>
		<tr>
			<td>&#3647;</td>
			<td>&amp;#3647;</td>
			<td>&nbsp;</td>
			<td>thai baht</td>
		</tr>
		<tr>
			<td>&#8363;</td>
			<td>&amp;#8363;</td>
			<td>&nbsp;</td>
			<td>dong</td>
		</tr>
		<tr>
			<td>&#8362;</td>
			<td>&amp;#8362;</td>
			<td>&nbsp;</td>
			<td>shekel</td>
		</tr>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
	<div id="code27" style="font-family: Corbel">
	<h2>Intellectual property codes</h2>
	<table class="dtable">
		<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
		</thead>
		<tr>
			<td>&copy;</td>
			<td>&amp;#169;</td>
			<td>&amp;copy;</td>
			<td>copyright</td>
		</tr>
		<tr>
			<td>&reg;</td>
			<td>&amp;#174;</td>
			<td>&amp;reg;</td>
			<td>registered trademark</td>
		</tr>
		<tr>
			<td>&#8471;</td>
			<td>&amp;#8471;</td>
			<td>&nbsp;</td>
			<td>sound recording copyright</td>
		</tr>
		<tr>
			<td>&trade;</td>
			<td>&amp;#8482;</td>
			<td>&amp;trade;</td>
			<td>trademark</td>
		</tr>
		<tr>
			<td>&#8480;</td>
			<td>&amp;#8480;</td>
			<td>&nbsp;</td>
			<td>service mark</td>
		</tr>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
	<div id="code28" style="font-family: Corbel" >
	<h2>Greek alphabet codes</h2>
	<table class="dtable">
		<thead>
		<tr>
			<th>Char</th>
			<th>Numeric code</th>
			<th>Named code</th>
			<th>Description</th>
		</tr>
		</thead>
		<tr>
			<td>&#945;</td>
			<td>&amp;#945;</td>
			<td>&amp;alpha;</td>
			<td>small alpha</td>
		</tr>
		<tr>
			<td>&#946;</td>
			<td>&amp;#946;</td>
			<td>&amp;beta;</td>
			<td>small beta</td>
		</tr>
		<tr>
			<td>&#947;</td>
			<td>&amp;#947;</td>
			<td>&amp;gamma;</td>
			<td>small gamma</td>
		</tr>
		<tr>
			<td>&#948;</td>
			<td>&amp;#948;</td>
			<td>&amp;delta;</td>
			<td>small delta</td>
		</tr>
		<tr>
			<td>&#949;</td>
			<td>&amp;#949;</td>
			<td>&amp;epsilon;</td>
			<td>small epsilon</td>
		</tr>
		<tr>
			<td>&#950;</td>
			<td>&amp;#950;</td>
			<td>&amp;zeta;</td>
			<td>small zeta</td>
		</tr>
		<tr>
			<td>&#951;</td>
			<td>&amp;#951;</td>
			<td>&amp;eta;</td>
			<td>small eta</td>
		</tr>
		<tr>
			<td>&#952;</td>
			<td>&amp;#952;</td>
			<td>&amp;theta;</td>
			<td>small theta</td>
		</tr>
		<tr>
			<td>&#953;</td>
			<td>&amp;#953;</td>
			<td>&amp;iota;</td>
			<td>small iota</td>
		</tr>
		<tr>
			<td>&#954;</td>
			<td>&amp;#954;</td>
			<td>&amp;kappa;</td>
			<td>small kappa</td>
		</tr>
		<tr>
			<td>&#955;</td>
			<td>&amp;#955;</td>
			<td>&amp;lambda;</td>
			<td>small lambda</td>
		</tr>
		<tr>
			<td>&#956;</td>
			<td>&amp;#956;</td>
			<td>&amp;mu;</td>
			<td>small mu</td>
		</tr>
		<tr>
			<td>&#957;</td>
			<td>&amp;#957;</td>
			<td>&amp;nu;</td>
			<td>small nu</td>
		</tr>
		<tr>
			<td>&#958;</td>
			<td>&amp;#958;</td>
			<td>&amp;xi;</td>
			<td>small xi</td>
		</tr>
		<tr>
			<td>&#959;</td>
			<td>&amp;#959;</td>
			<td>&amp;omicron;</td>
			<td>small omicron</td>
		</tr>
		<tr>
			<td>&#960;</td>
			<td>&amp;#960;</td>
			<td>&amp;pi;</td>
			<td>small pi</td>
		</tr>
		<tr>
			<td>&#961;</td>
			<td>&amp;#961;</td>
			<td>&amp;rho;</td>
			<td>small rho</td>
		</tr>
		<tr>
			<td>&#963;</td>
			<td>&amp;#963;</td>
			<td>&amp;sigma;</td>
			<td>small sigma</td>
		</tr>
		<tr>
			<td>&#964;</td>
			<td>&amp;#964;</td>
			<td>&amp;tau;</td>
			<td>small tau</td>
		</tr>
		<tr>
			<td>&#965;</td>
			<td>&amp;#965;</td>
			<td>&amp;upsilon;</td>
			<td>small upsilon</td>
		</tr>
		<tr>
			<td>&#966;</td>
			<td>&amp;#966;</td>
			<td>&amp;phi;</td>
			<td>small phi</td>
		</tr>
		<tr>
			<td>&#967;</td>
			<td>&amp;#967;</td>
			<td>&amp;chi;</td>
			<td>small chi</td>
		</tr>
		<tr>
			<td>&#968;</td>
			<td>&amp;#968;</td>
			<td>&amp;psi;</td>
			<td>small psi</td>
		</tr>
		<tr>
			<td>&#969;</td>
			<td>&amp;#969;</td>
			<td>&amp;omega;</td>
			<td>small omega</td>
		</tr>
		<tr>
			<td>&#913;</td>
			<td>&amp;#913;</td>
			<td>&amp;Alpha;</td>
			<td>capital alpha</td>
		</tr>
		<tr>
			<td>&#914;</td>
			<td>&amp;#914;</td>
			<td>&amp;Beta;</td>
			<td>capital beta</td>
		</tr>
		<tr>
			<td>&#915;</td>
			<td>&amp;#915;</td>
			<td>&amp;Gamma;</td>
			<td>capital gamma</td>
		</tr>
		<tr>
			<td>&#916;</td>
			<td>&amp;#916;</td>
			<td>&amp;Delta;</td>
			<td>capital delta</td>
		</tr>
		<tr>
			<td>&#917;</td>
			<td>&amp;#917;</td>
			<td>&amp;Epsilon;</td>
			<td>capital epsilon</td>
		</tr>
		<tr>
			<td>&#918;</td>
			<td>&amp;#918;</td>
			<td>&amp;Zeta;</td>
			<td>capital zeta</td>
		</tr>
		<tr>
			<td>&#919;</td>
			<td>&amp;#919;</td>
			<td>&amp;Eta;</td>
			<td>capital eta</td>
		</tr>
		<tr>
			<td>&#920;</td>
			<td>&amp;#920;</td>
			<td>&amp;Theta;</td>
			<td>capital theta</td>
		</tr>
		<tr>
			<td>&#921;</td>
			<td>&amp;#921;</td>
			<td>&amp;Iota;</td>
			<td>capital iota</td>
		</tr>
		<tr>
			<td>&#922;</td>
			<td>&amp;#922;</td>
			<td>&amp;Kappa;</td>
			<td>capital kappa</td>
		</tr>
		<tr>
			<td>&#923;</td>
			<td>&amp;#923;</td>
			<td>&amp;Lambda;</td>
			<td>capital lambda</td>
		</tr>
		<tr>
			<td>&#924;</td>
			<td>&amp;#924;</td>
			<td>&amp;Mu;</td>
			<td>capital mu</td>
		</tr>
		<tr>
			<td>&#925;</td>
			<td>&amp;#925;</td>
			<td>&amp;Nu;</td>
			<td>capital nu</td>
		</tr>
		<tr>
			<td>&#926;</td>
			<td>&amp;#926;</td>
			<td>&amp;Xi;</td>
			<td>capital xi</td>
		</tr>
		<tr>
			<td>&#927;</td>
			<td>&amp;#927;</td>
			<td>&amp;Omicron;</td>
			<td>capital omicron</td>
		</tr>
		<tr>
			<td>&#928;</td>
			<td>&amp;#928;</td>
			<td>&amp;Pi;</td>
			<td>capital pi</td>
		</tr>
		<tr>
			<td>&#929;</td>
			<td>&amp;#929;</td>
			<td>&amp;Rho;</td>
			<td>capital rho</td>
		</tr>
		<tr>
			<td>&#931;</td>
			<td>&amp;#931;</td>
			<td>&amp;Sigma;</td>
			<td>capital sigma</td>
		</tr>
		<tr>
			<td>&#932;</td>
			<td>&amp;#932;</td>
			<td>&amp;Tau;</td>
			<td>capital tau</td>
		</tr>
		<tr>
			<td>&#933;</td>
			<td>&amp;#933;</td>
			<td>&amp;Upsilon;</td>
			<td>capital upsilon</td>
		</tr>
		<tr>
			<td>&#934;</td>
			<td>&amp;#934;</td>
			<td>&amp;Phi;</td>
			<td>capital phi</td>
		</tr>
		<tr>
			<td>&#935;</td>
			<td>&amp;#935;</td>
			<td>&amp;Chi;</td>
			<td>capital chi</td>
		</tr>
		<tr>
			<td>&#936;</td>
			<td>&amp;#936;</td>
			<td>&amp;Psi;</td>
			<td>capital psi</td>
		</tr>
		<tr>
			<td>&#937;</td>
			<td>&amp;#937;</td>
			<td>&amp;Omega;</td>
			<td>capital omega</td>
		</tr>
	</table>
	</div>
	</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code29">
<H3> Abbreviations and Acronyms </H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<abbr title="United Nations">UN</abbr>
<br/>
<acronym title="World Wide Web">WWW</acronym>
<p>The title attribute is used to show the spelled-out version when holding the mouse pointer over the acronym or abbreviation.</p>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>
<body>
<abbr title="United Nations">UN</abbr>
<br/><br/>
<acronym title="World Wide Web">WWW</acronym>
<p>The title attribute is used to show the spelled-out version when holding the mouse pointer over the acronym or abbreviation.</p>
</body>
</html>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code30">
<H3> Text Direction </H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<p>
If your browser supports bidirectional override (bdo), the next line will be written from the right to the left (rtl):
</p>
<bdo dir="rtl">
Here is some backward text
</bdo>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>
<body>
<p>
If your browser supports bidirectional override (bdo), the next line will be written from the right to the left (rtl):
</p>
<bdo dir="rtl">
Here is some backward text
</bdo>
</body>
</html>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code31">
<H3> Quotations</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
A blockquote quotation:
<blockquote>
This is a long quotation. This is a long quotation. This is a long quotation. This is a long quotation. This is a long quotation.
</blockquote>
<p><b>The browser inserts line breaks and margins for a blockquote element.</b></p>
A short quotation:
<q>This is a short quotation</q>
<p><b>The q element does not render as anything special.</ b></p>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>

<body>

A blockquote quotation:

<blockquote>

This is a long quotation. This is a long quotation. This is a long quotation. This is a long quotation. This is a long quotation.

</blockquote>

<p><b>The browser inserts line breaks and margins for a blockquote element.</b></p>

A short quotation:

<q>This is a short quotation</q>

<p><b>The q element does not render as anything special.</b></p>

</body>

</html>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code32">
<H3> Deleted and Inserted Text</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<p>
a dozen is
<del>twenty</del>
<ins>twelve</ins>
pieces
</p>
<p>
Most browsers will <del>overstrike</del> deleted text and <ins>underscore</ins> inserted text.
</p>
<p>
Some older browsers will display deleted or inserted text as plain text.
</p>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>

<body>

<p>

a dozen is

<del>twenty</del>

<ins>twelve</ins>

pieces

</p>

<p>

Most browsers will <del>overstrike</del> deleted text and <ins>underscore</ins> inserted text.

</p>

<p>

Some older browsers will display deleted or inserted text as plain text.

</p>

</body>

</html>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>


<div id="code33">
<H3> The HTML Style Attribute</H3>
<H3> Code: </H3>
<XMP>
<html>
<body style="background-color:Gray;">
<h1>Look! Styles and colors</h1>
<p style="font-family:verdana;color:red"> This text is in Verdana and red</p>
<p style="font-family:times;color:green">
This text is in Times and green</p>
<p style="font-size:30px">This text is 30 pixels high</p>
</body>
</html>
</XMP>

<a href="code5.html"><button type="button">Try it Yourself!</button></a>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code34">
<H3> Background Color</H3>
<H3> Code: </H3>
<XMP>
<html>
<body style="background-color:gray"> <h2>Look: Colored Background!</h2>
</body>
</html>
</XMP>

<a href="code6.html"><button type="button">Try it Yourself!</button></a>
</br>
<H3> Code: </H3>
<XMP>
<html>
<body bgcolor="gray">
<h2>Look: Colored Background!</h2>
<p>For future-proof HTML, use HTML styles instead:</p> <p>style="background-color:gray"</p>
</body>
</html>
</XMP>

<a href="code7.html"><button type="button">Try it Yourself!</button></a>

</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code35">
<H3> Font Family, Color, and Size</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<h1 style="font-family:verdana">A heading</h1>
<p style="font-family:courier new; color:red; font-size:20px;">A paragraph</p>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>
<body>
<h1 style="font-family:verdana">A heading</h1>
<p style="font-family:courier new; color:red; font-size:20px;">A paragraph</p>
</body>
</html>


<H3> Code: </H3>
<XMP>
<html>
<body>
<p><font size="2" face="Verdana">
This is a paragraph.
</font></p>
<p><font size="5" face="Times" color="red"> This is another paragraph.</font></p>
</body>
</html>
</XMP>
<a href="code8.html"><button type="button">Try it Yourself!</button></a>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>
<div id="code36">
<H3> Text Alignment</H3>
<H3> Code: </H3>
<XMP>
<html>
<body>
<h1 style="text-align:center">This is heading 1</h1>
<p>The heading above is aligned to the center of this page. The heading above is aligned to the center of this page. The heading above is aligned to the center of this page. </p>
</body>
</html>
</XMP>

<H3> Output: </H3>

<html>

<body>

<h1 style="text-align:center">This is heading 1</h1>

<p>The heading above is aligned to the center of this page. The heading above is aligned to the center of this page. The heading above is aligned to the center of this page. </p>

</body>

</html>

<H3> Code: </H3>
<XMP>
<html>
<body>
<h1 align="center">This is heading 1</h1>
<p>The heading above is aligned to the center of this page. The heading above is aligned to the center of this page. The heading above is aligned to the center of this page.</ p>
</body>
</html>
</XMP>

<a href="code9.html"><button type="button">Try it Yourself!</button></a>
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>
<hr>

<div id="code37"  style ="font-family: Georgia, Serif;">
<center> <h3>  <font color="black" size="6" face="calibri"> C Programming </font>            </h3> </center>
 </br>
 
 
 <ul>
<li>A High Level Programming Language (which uses alphabets, digits, punctuations and some special symbols and cannot be executed directly without being converted into machine level language (the language which uses only 0 and 1))</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>developed by a man named Dennis Ritchie</li>
</ul>

</br>
<center> <img src="images/d1.jpg" alt="Smiley face" height="255" width="197"> </center>
</br>



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
<center>
<p><strong>*</strong></p>
<p><strong>*****</strong></p>
<p><strong>*****</strong></p>
<p><strong>*****</strong></p>
<p><strong>*****</strong></p>
</center>
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
<center>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
</center>
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
<center>
<p>*</p>
<p>****</p>
<p>*******</p>
<p>****</p>
<p>*</p>
</center>
<p>(b)</p>
<center>
<p>&nbsp;</p>
<p>****************</p>
<p>* *</p>
<p>* Hello World! *</p>
<p>* *</p>
<p>****************</p>
<p>&nbsp;</p>
</center>
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
<center>
<h4>- Donald Knuth</h4></center>
<h2>&nbsp;</h2>
<h4>You might have an algorithm for getting from office home , for making a chunk of code that calculates the terms of the Fibonacci sequence , or for finding what you're looking for in a retail store . Algorithms are the building blocks of computer programs or a sequence of a sequence of unambiguous instructions ( the term 'unambiguous ' indicates that there is no room for subjective interpretation ) that tells how the problem can be addressed and solved - - which is definitely overblown in their importance like road maps for accomplishing a given , well-defined automated reasoning task - - which always have a clear stopping point . Long division and column addition are examples that everyone is familiar with- even a simple function for adding two numbers is an implementation of a particular algorithm. Online grammar checking uses algorithms . Financial computations use algorithms . A search engine like Google uses search engine algorithms (for example , takes search strings of keywords as input , searches its associated database for relevant web pages , and returns results ) . In fact , it is difficult to think of a task performed by your computer that does not use computer procedures that are a lot like a recipes (called algorithms ) .</h4>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<ul>
<li>The algorithm <strong>to add two numbers entered by user</strong>would look something like this:</li>
<li>Step 1: Start</li>
<li>Step 2: Declare variables num1, num2 and sum.</li>
<li>Step 3: Read values num1 and num2.</li>
<li>Step 4: Add num1 and num2 and assign the result to sum.</li>
</ul>
<center> <p>sum&larr;num1+num2</p></center>
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

</br>
<center> <img src="images/binary_search_0.jpg" alt="Smiley face" height="72" width="483"> </center>
</br>


<p>First, we shall determine half of the array by using this formula &minus;</p>



<p>mid = low + (high - low) / 2</p>


</br>
<center> <img src="images/binary_search_1.jpg" alt="Smiley face" height="105" width="483"> </center>
</br>




<p>Here it is, 0 + (9 - 0 ) / 2 = 4 (integer value of 4.5). So, 4 is the mid of the array.</p>




<p>Now we compare the value stored at location 4, with the value being searched, i.e. 31. We find that the value at location 4 is 27, which is not a match. As the value is greater than 27 and we have a sorted array, so we also know that the target value must be in the upper portion of the array.</p>



</br>
<center> <img src="images/binary_search_2.jpg" alt="Smiley face" height="72" width="482"> </center>
</br>

<p>We change our low to mid + 1 and find the new mid value again.</p>
<p>low = mid + 1</p>
<p>mid = low + (high - low) / 2</p>
<p>Our new mid is 7 now. We compare the value stored at location 7 with our target value 31.</p>


</br>
<center> <img src="images/binary_search_3.jpg" alt="Smiley face" height="106" width="483"> </center>
</br>


<p>The value stored at location 7 is not a match, rather it is more than what we are looking for. So, the value must be in the lower part from this location.</p>


</br>
<center> <img src="images/binary_search_4.jpg" alt="Smiley face" height="74" width="482"> </center>
</br>


<p>Hence, we calculate the mid again. This time it is 5.</p>


</br>
<center> <img src="images/binary_search_5.jpg" alt="Smiley face" height="104" width="483"> </center>
</br>



<p>We compare the value stored at location 5 with our target value. We find that it is a match.</p>



</br>
<center> <img src="images/binary_search_6.jpg" alt="Smiley face" height="75" width="483"> </center>
</br>



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
<p>&nbsp;</p>
 
</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>The C Programming Language </xmp></center></td>
                <td><center><xmp>Brian W. Kernighan</xmp></center></td>
                <td><a href="img/pdf12.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>Let Us C</xmp></center></td>
                <td><center><xmp>Yashavant P. Kanetkar</xmp></center></td>
                <td><a href="img/pdf13.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>A Book on C </xmp></center></td>
                <td><center><xmp>AI Kelley </xmp></center></td>
                <td><a href="img/pdf14.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Head First C</xmp></center></td>
                <td><center><xmp>David Griffiths</xmp></center></td>
                <td><a href="img/pdf15.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C For Dummies</xmp></center></td>
                <td><center><xmp>Dan Gookin</xmp></center></td>
                <td><a href="img/pdf16.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C in a Nutshell</xmp></center></td>
                <td><center><xmp> Peter Prinz</xmp></center></td>
                <td><a href="img/pdf17.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C: The Complete Reference</xmp></center></td>
                <td><center><xmp>Herbert Schildt</xmp></center></td>
                <td><a href="img/pdf18.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp> Learning C programming </xmp></center></td>
                <td><center><xmp> TutorialsPoint</xmp></center></td>
                <td><a href="img/pdf19.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C Programming Tutorial</xmp></center></td>
                <td><center><xmp>Mark Burgess</xmp></center></td>
                <td><a href="img/pdf20.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>Programming in C</xmp></center></td>
                <td><center><xmp>Stephen G. Kochan</xmp></center></td>
                <td><a href="img/pdf21.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Practical C Programming</xmp></center></td>
                <td><center><xmp>Steve Oualline</xmp></center></td>
                <td><a href="img/pdf22.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>



</br>


										  
												  									
</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>



<div id="code38" style ="font-family: Georgia, Serif;">
<center> <h3>  <font color="black" size="6" face="calibri"> C++ Programming </font>            </h3> </center>
 </br>
 
 <ul>
<li>An Object-oriented (Programming methodology that views a computer program as a combination of variables, functions, and data structures called objects) high level language (which uses alphabets, digits, punctuations and some special symbols and cannot be executed directly without being converted into machine level language (the language which uses only 0 and 1))</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>developed by a Danish computer scientist</li>
</ul>
</br>
<center> <img src="images/d2.jpg" alt="Smiley face" height="335" width="500"> </center>
</br>

<p><strong>Bjarne Stroustrup</strong> (in 1979 at AT &amp; T Bell laboratories, USA) as an extension of the C language</p>
<p>&nbsp;</p>
<ul>
<li>initially named C with classes which later named C ++ in 1983.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>As a successor of C language, C++ has been certified as a 99.9 percent pure standard and possesses exceptional performance, efficiency and flexibility of use compared to C language.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>Advantage:</strong> Has the power and extensibility to write large-scale programs and runs on a variety of platforms, such as Windows, Mac OS, and the various versions of UNIX.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>Uses:</strong> Used in the development of Apple Macintosh, PC running Windows, operating systems and Adobe Systems (like Photoshop, Acrobat etc).</li>
<li><strong>C++</strong> fully supports most important features of <strong>object-oriented programming</strong> including the four pillars of object-oriented development:</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>Encapsulation</li>
<li>Data hiding</li>
<li>Inheritance</li>
<li>Polymorphism</li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>Inheritance</strong></li>
</ul>
<p>&nbsp;</p>
<p>The ability of a class (<strong>sub class</strong>) to derive properties and characteristics from another class (<strong>super class</strong>) is called Inheritance. Inheritance is one of the most important feature of Object Oriented Programming.</p>
<p>The capability of a class to derive properties and characteristics from another class is called&nbsp;<strong>Inheritance</strong>. Inheritance is one of the most important feature of Object Oriented Programming.</p>
<p>&nbsp;</p>
<p><strong>Sub Class:</strong>&nbsp;The class that inherits properties from another class is called Sub class or Derived Class.<br /> <strong>Super Class:</strong>The class whose properties are inherited by sub class is called Base Class or Super class.</p>
<p>&nbsp;</p>
<p><strong>Why and when to use inheritance?</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Consider a group of vehicles. You need to create classes for Bus, Car and Truck. The methods fuelAmount(), capacity(), applyBrakes() will be same for all of the three classes. If we create these classes avoiding inheritance then we have to write all of these functions in each of the three classes as shown in below figure:</p>
<p>&nbsp;</p>
<p><strong>Process of C++ program execution: A C++ program:</strong>&nbsp;</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>int main()</p>
<p>{</p>
<p>std::cout&lt;&lt;"Hello, crazy world!";</p>
<p>return 0;</p>
<p>}&nbsp;</p>
<p>&nbsp;</p>
<p>is written using Text Editor , such as [ Notepad++, Notepad ] and saved with [.ccp] Extension.</p>
<p>File Saved with [.ccp] extension is called Source Program or Source Code.</p>
<p>C++ Source code with [.ccp] Extension is sent to preprocessor first.</p>
<p>The preprocessor generates an expanded source code:</p>
<p>&nbsp;</p>
<p>// ------------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>The contents of &lt;iostream&gt;would be pasted at the location of #include&lt;iostream&gt;</p>
<p>int main()</p>
<p>{</p>
<p>std::cout&lt;&lt;"Hello, crazy world!";</p>
<p>return 0;</p>
<p>}&nbsp;</p>
<p>&nbsp;</p>
<p>--------------------------------------------------------------------------------------------------------------------------------&nbsp; //</p>
<p>&nbsp;</p>
<ul>
<li>Expanded source code is given as input to compiler where the expanded source program is compiled (i.e., the program is entirely read and translated to instructions the computer can understand i.e., machine understandable / readable language i.e., to machine code sequence of 0s and 1s).</li>
<li>If the C++ compiler finds any error during compilation, it provides information about the error to the programmer.</li>
<li>The programmer has to review code and re-edit the program. After re-editing program, Compiler again check for any error.</li>
<li>If program is error-free then it is sent to assembler (where the code is assembled and converted into object code. Now a simple.obj file is generated).</li>
<li>The object code is sent to linker (where the object code is linked with included header files (such as iostream) and appropriate libraries).</li>
<li>Then it is converted into executable code. A simple.exe file is generated.</li>
<li>The executable code is sent to loader (where the executable code is loaded into memory and then it is executed).</li>
<li>After execution, output</li>
</ul>
<p>Hello,world!</p>
<p>is displayed on the console screen.</p>
<p>&nbsp;</p>
<p>Like C</p>
<p>C++ is case sensitive language: only lower case letters (or small letters) must be used.&nbsp;</p>
<p>Capital letters (or upper case letters) must be avoided to prevent the display of error on the screen</p>
<p>(For example: If the statement STD::COUT&lt;&lt;"Hello, crazy world!"; is written instead of</p>
<p>std::cout&lt;&lt;"Hello, crazy world!";</p>
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
<p>i.e., int main(&nbsp; )</p>
<p>&nbsp;</p>
<p>to prevent the display of compilation error on the screen.</p>
<p>&nbsp;</p>
<p>As we know C++ is Platform dependent language. So the Operating system needs to know when the program execution ends.</p>
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
<p>The statement <strong>#include&lt;iostream&gt;</strong> tells the compiler to include the text from the file iostream (which is already present in the operating system) before it translates or compiles the program into a sequence of 0s and 1s.</p>
<p>&nbsp;</p>
<p><strong>#include &lt;iostream&gt;</strong> is to C++ what #include&lt;iostream&gt; is to C (note one thing: there is no .h extension to the name iostream. The reason is that &lt;iostream&gt; is one of the modern&nbsp; style headers)</p>
<p>&nbsp;</p>
<p>iostream means input output screen (i&rarr; input,&nbsp; o &rarr; output,&nbsp; stream &rarr; screen) and iostream comprises input output functions like cout, cin etc. -- note: cin is a input function (cin means console input) and cout is a output function (cout means console output) and it is included into the C ++ program by writing the statement #include &lt;iostream&gt;). The statement #include tell the compiler to include the contents of the file iostream before compilation. If a program is written without the statement <strong>#include&lt;iostream&gt;</strong>, then the C++ compiler can&rsquo;t compile and a compilation error will be displayed on the screen (because C++ compiler fails&nbsp; to recognize the functions such as cin and cout).</p>
<p>int main() &rarr;&nbsp; The program begins its execution with the function main() -- which is called the user defined function (because this function is defined by the user) - the main function -- the entry point of the program execution i.e., the point from where the execution of C++ program begins and the point at which the operating system passes control of the computer over to that program.</p>
<p>&nbsp;</p>
<p>int main() {</p>
<p>} &rarr; implies body of the main function within which the sequence of instructions in the form of statements</p>
<p>i.e., the program&nbsp; is written and executed. The left curly brace</p>
<p>{</p>
<p>implies: the beginning of the main function</p>
<p>and the right curly brace</p>
<p>}</p>
<p>implies: the end of the main function.</p>
<p>&nbsp;</p>
<p>return 0; &rarr; implies the exit status of execution of the program i.e., at this point,</p>
<p>main function returns back the control of the computer to the operating system since</p>
<p>the execution is terminated at this point and once a return statement</p>
<p>i.e., return 0; is executed, no further instructions within the main function are executed</p>
<p>&nbsp;</p>
<p><strong>For example:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>int main()</p>
<p>{</p>
<p>std::cout&lt;&lt;"Hello, crazy world!";</p>
<p>return 0;</p>
<p>std::cout&lt;&lt;"Hello, crazy world!";</p>
<p>}</p>
<p>&nbsp;</p>
<p>Or</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"Hello, crazy world!";</p>
<p>return 0;</p>
<p>cout&lt;&lt;"Hello, crazy world!";</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Hello,world!</p>
<p>&nbsp;</p>
<p>; &rarr; implies semicolon --&gt; A program is a well-defined set of instructions and each well-defined instruction (in the form of a statement)</p>
<p>is ended by a semicolon (which is C++ language punctuation --</p>
<p>like a period in English i.e., in an English paragraph each sentence is ended by a full stop which tells that one sentence ends and another begins,</p>
<p>semicolon implies that one instruction (or statement) ends and another begins).</p>
<p>&nbsp;</p>
<p>cout&rarr; implies the output function of the C++ language which makes provision to print the output:</p>
<p>Hello, crazy world!</p>
<p>on the console screen.</p>
<p>In the statement:</p>
<p>std::cout</p>
<p>std &rarr; standard</p>
<p>:: &rarr; scope resolution operator</p>
<p>cout &rarr; console output</p>
<p>std::cout basically means: look in standard library and get cout function. The text</p>
<p>Hello, crazy world! should be enclosed by the double quotation marks ("") and if the statement:</p>
<p>using std::cout;</p>
<p>is added below the statement:</p>
<p>#include&lt;iostream&gt;</p>
<p>then the program takes the form:</p>
<p>#include&lt;iostream&gt;</p>
<p>using std::cout;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"Hello, crazy world!";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>i.e., no need to include std:: in the statement:</p>
<p>std::cout&lt;&lt;"Hello, crazy world!";</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> The symbol &lt;&lt; implies: output the text:</li>
</ul>
<p>Hello, crazy world!</p>
<p>on the console screen using the cout function.</p>
<p>&nbsp;</p>
<p><strong>Program 1.1</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to print the word "hello Bill Gates" on screen</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using std::cout;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"hello Bill Gates";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>hello Bill Gates</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 1.2</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to print </strong></p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p><strong>on screen</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using std::cout;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp; ***** ";</p>
<p>cout&lt;&lt;"\n&nbsp; ***** ";</p>
<p>cout&lt;&lt;"\n&nbsp; ***** ";</p>
<p>cout&lt;&lt;"\n&nbsp; ***** ";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>&nbsp;</p>
<p>If new line \n is not included in the above program then the output on the screen is:</p>
<p>&nbsp;</p>
<p>*********************</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>endl</p>
<p>can be used instead of \n:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using std::cout;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen :</strong></p>
<p><strong>&nbsp;</strong></p>
<p>// The error:</p>
<p>endl was not declared in this scope //</p>
<p>will be displayed on the screen.</p>
<p>If the above program is rewritten:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using std::cout;</p>
<p>using std::endl;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen :</strong></p>
<p>&nbsp;</p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>&nbsp;</p>
<p>The single statement:</p>
<p>using namespace std;</p>
<p>can be used instead of the statements:</p>
<p>&nbsp;</p>
<p>using std::cout;</p>
<p>using std::endl;</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>cout&lt;&lt;"&nbsp;&nbsp;&nbsp;&nbsp; ***** "&lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen :</strong></p>
<p>&nbsp;</p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>&nbsp;</p>
<p>//----------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>cout &lt;&lt;"Hello world."&lt;&lt; endl;&nbsp; // Here it is necessary to put 'using namespace std' on the top of code.</p>
<p>std::cout &lt;&lt;"Hello world."&lt;&lt; std::endl; // Here there is no need to put 'using namespace std' on the top of code.</p>
<p>&nbsp;</p>
<p>-----------------------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
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
<p>C++ is done mostly in lowercase. It's a case-sensitive language</p>
<p>&nbsp;</p>
<p><strong>Answers:</strong></p>
<p>&nbsp;</p>
<p>(a)</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ******* ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****&nbsp;&nbsp;&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>(b)</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****************&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * Hello World! *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ";&nbsp;&nbsp;&nbsp;</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>cout&lt;&lt;"\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****************&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>(c)</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"\n Braces come in pairs!";</p>
<p>cout&lt;&lt;"\n Comments come in pairs!";</p>
<p>cout&lt;&lt;"\n&nbsp; All statements end with a semicolon!";</p>
<p>cout&lt;&lt;"\n&nbsp; Spaces are optional!";</p>
<p>cout&lt;&lt;"\n Must have a main function!";</p>
<p>cout&lt;&lt;"\n C++ is done mostly in lowercase. It's a case-sensitive language";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 1.3</strong></p>
<p><strong>C++&nbsp; program to find the area of a circle </strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>main()</p>
<p>{</p>
<p>int r, area;</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>cout&lt;&lt;"The area of the circle = "&lt;&lt; area;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>The area of the circle = 50</p>
<p>&nbsp;</p>
<p>int means the data type is integer.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> An integer is a whole number -- no fractions, decimal parts, or funny stuff.</li>
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
<p>cout&lt;&lt;"The area of the circle = "&lt;&lt; area;</p>
<p>make provision to print the output:</p>
<p>The area of the circle = 50</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>The area of the circle is 50. 24 (for r = 2) but The area of the circle = 50 is displayed on the screen</p>
<p>because data type int is used instead of float.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>float r, area; is used instead of int r, area;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>int main()</p>
<p>{</p>
<p>float r, area;</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>cout&lt;&lt;"The area of the circle = "&lt;&lt; area;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong>:</p>
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
<p>data type float is used instead of int because if the data type int is used instead of float then the result will not be clearly outputted i.e., instead of 50.24 the computer displays only 50.</p>
<p>&nbsp;</p>
<p>If you want to supply the value for r through the key board, then the statement</p>
<p>&nbsp;</p>
<p>float r = 2;</p>
<p>should be replaced by the statements</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;r;</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float r, area;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;r;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>cout&lt;&lt;"The area of the circle = "&lt;&lt; area;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you the number 2</p>
<p>The area of the circle = 50.24 will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>As told earlier:</strong> cout is an output function and cin is an input function.</li>
</ul>
<p>&nbsp;</p>
<p>The statement:</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>make provision to print the text</p>
<p>Enter any number:</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>cin&gt;&gt; r; is to C++ what scanf("%d", &amp;r); is to C</p>
<p>&nbsp;</p>
<p>If you write the statement:</p>
<p>area = 4 * 3.14 * r ^ 2;</p>
<p>instead of</p>
<p>area = 4 * 3.14 * r * r;&nbsp;</p>
<p>&nbsp;</p>
<p>Then compilation error will be displayed on the console screen because like in C Language &ndash; there is no operator for performing exponentiation operation -- so the statement&nbsp;</p>
<p>area = 4 * 3.14 * r ^ 2; is invalid.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>cout and cin are not part of C++ language but they are part of iostream file</p>
<p>Hence the statement #include&lt;iostream&gt; should be included in the C++ program otherwise cout and cin&nbsp; will not work and the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>Right shift operator &gt;&gt; denote stream extraction operator (extract data entered through the keyboard)</p>
<p>Left shift operator &lt;&lt; denote stream insertion operator (insert data into an output screen)</p>
<p>&nbsp;</p>
<p>&lt;&lt; and &gt;&gt; are termed overloaded operators and the file iostream defines these operators.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> As told earlier: when you enter an integer for x through the keyboard, this integer will be stored in the computer memory.</li>
</ul>
<p>&nbsp;</p>
<p>If you yearn to know the storage size of the integer in computer memory</p>
<p>(i.e., space occupied by the entered integer in the computer memory), you need to appeal to the following program:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x;</p>
<p>x=10;</p>
<p>cout&lt;&lt;"size of r =&nbsp; "&lt;&lt; sizeof(r);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>size of x = 4</p>
<p>i.e., integer entered for r i.e., 10 has occupied a space of 4 bytes in the computer memory.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the circumference of the circle (given r = 2.5)</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float r, area;</p>
<p>r = 2.5;</p>
<p>circumference = 3.14 * r * r;</p>
<p>cout&lt;&lt;"The circumference of the circle =&nbsp; "&lt;&lt; circumference;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the area of the rectangle (given l = 2.5 and b = 3)</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float l, b, area;</p>
<p>l = 2.5;</p>
<p>b = 3;</p>
<p>area = 1*b;</p>
<p>cout&lt;&lt;"The area of the rectangle =&nbsp; "&lt;&lt; area;</p>
<p>return 0;</p>
<p>}</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Format Specifiers in C++ </strong></p>
<p>&nbsp;</p>
<table width="204">
<tbody>
<tr>
<td width="77">
<p><strong>Data Type</strong></p>
</td>
<td width="126">
<p><strong>Format Specifier</strong></p>
</td>
</tr>
<tr>
<td width="77">
<p>int</p>
</td>
<td width="126">
<p>%d</p>
</td>
</tr>
<tr>
<td width="77">
<p>float</p>
</td>
<td width="126">
<p>%f or %e</p>
</td>
</tr>
<tr>
<td width="77">
<p>char</p>
</td>
<td width="126">
<p>%c</p>
</td>
</tr>
<tr>
<td width="77">
<p>double</p>
</td>
<td width="126">
<p>%lf or %le</p>
</td>
</tr>
<tr>
<td width="77">
<p>long int</p>
</td>
<td width="126">
<p>%ld</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 4.6</strong></p>
<p><strong>C++ program to find the sum of two numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, sum;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>sum = a + b;</p>
<p>cout&lt;&lt;"the sum of a and b = "&lt;&lt; sum;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the sum of a and b = 3</p>
<p>If you assign the floating point values 1.5 &amp; 2.6 for a &amp; b, then the statement:</p>
<p>int a, b, sum; should be replaced by the statement float a, b, sum;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float a, b, sum;</p>
<p>a=1.5;</p>
<p>b=2.6;</p>
<p>sum = a + b;</p>
<p>cout&lt;&lt;"the sum of a and b = "&lt;&lt; sum;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the sum of a and b = 4.1</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>cout&lt;&lt;"the sum of a and b = "&lt;&lt; sum;</p>
<p>make provision to print the output:</p>
<p>the sum of a and b = 4.1</p>
<p>&nbsp;</p>
<p>on the console screen. And if the statement:</p>
<p>cout&lt;&lt;"the sum of a and b = "&lt;&lt; sum;</p>
<p>is omitted from the C ++ program, then the program will be successfully executed but there will be no display of the output on the console screen.</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then the statements:</p>
<p>a=1.5;</p>
<p>b=2.6;</p>
<p>should be replaced by the statements:</p>
<p>cout&lt;&lt;"Enter any two numbers:";</p>
<p>cin&gt;&gt;a;</p>
<p>cin&gt;&gt;b;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float a, b, sum;</p>
<p>cout&lt;&lt;"Enter any two numbers:";</p>
<p>cin&gt;&gt;a;</p>
<p>cin&gt;&gt;b;</p>
<p>sum = a+ b;</p>
<p>cout&lt;&lt;"the sum of a and b = "&lt;&lt; sum;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two numbers:</p>
<p>If you enter two numbers 2.9 &amp; 3.6</p>
<p>the sum of a and b = 6.5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>cout&lt;&lt;"Enter any two numbers:";</p>
<p>make provision to print</p>
<p>Enter any two numbers:</p>
<p>on the screen and the statements:</p>
<p>cin&gt;&gt;a;</p>
<p>cin&gt;&gt;b;</p>
<p>make provision to read the two numbers 2.9 and 3.6 entered through the keyboard and store them in the computer memory.</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>cout&lt;&lt;"Enter any two numbers:";</p>
<p>cin&gt;&gt;a;</p>
<p>cin&gt;&gt;b;</p>
<p>are replaced by the statements:</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;b;</p>
<p>Then the output on the screen is:</p>
<p>Enter any number:</p>
<p>If you enter the number 2.9</p>
<p>Enter any number:</p>
<p>If you enter the number 3.6</p>
<p>the sum of a and b = 6.5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>cout&lt;&lt;"the sum of a and b = "&lt;&lt; sum;</p>
<p>is replaced by the statement:</p>
<p>cout&lt;&lt; a &lt;&lt;" + "&lt;&lt; b &lt;&lt;" = "&lt;&lt; sum;</p>
<p>Then the output:</p>
<p>2.9 + 3.6 = 6.5</p>
<p>will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int a = 5;</p>
<p>int main()</p>
<p>{</p>
<p>int a =2;</p>
<p>cout&lt;&lt; a;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong> 2</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>2 is a local variable (variable declared within the body of the main function)</p>
<p>The statement:</p>
<p>int a = 2;</p>
<p>imply: local variable declaration.</p>
<p>5 is a global variable (variable declared outside the body of the main function)</p>
<p>The statement:</p>
<p>int a = 5;</p>
<p>imply: global variable declaration.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>cout&lt;&lt; a;</p>
<p>is replaced by the statement:</p>
<p>cout&lt;&lt; :: a; (where :: denote scope resolution operator)</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int a = 5;</p>
<p>int main()</p>
<p>{</p>
<p>int a =2;</p>
<p>cout&lt;&lt; ::a;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>5</p>
<p>i.e., global variable will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the same program is written in C language</p>
<p>i.e.,</p>
<p>#include&lt;stdio.h&gt;</p>
<p>int a = 5;</p>
<p>int main()</p>
<p>{</p>
<p>int a =2;</p>
<p>print("%d", ::a);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the compilation error will be outputted on the screen because</p>
<p>scope resolution operator is not defined in the C language (i.e., C does not hold scope resolution operator).</p>
<p>&nbsp;</p>
<ul>
<li><strong>Whether the following program will be successfully outputted or not:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>a=3;</p>
<p>b=2;</p>
<p>c= a+b;</p>
<p>cout&lt;&lt;" sum of two numbers = 6"&lt;&lt; c;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>Yes, the output on the screen is:</p>
<p>sum of two numbers = 65</p>
<p>&nbsp;</p>
<p><strong>Program 4.7</strong></p>
<p><strong>C ++ program to convert the temperature in Celsius to Fahrenheit</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float C, F;</p>
<p>C=38.5;</p>
<p>F = 9*C/5 +32;</p>
<p>cout&lt;&lt;"temperature in Fahrenheit= "&lt;&lt; F;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>temperature in Fahrenheit = 101.3</p>
<p>&nbsp;</p>
<p><strong>As said Earlier: </strong></p>
<p>If&nbsp; &times;&nbsp; is used instead of *</p>
<p>and F = 9C/5 +32 is used of F = 9*C/5 +32, the compilation error will be displayed on the screen.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to supply a value 16 digits after decimal point i.e., 36.5555555555555555 for C, then the statement:</p>
<p>double C, F;</p>
<p>should be used instead of the statement:</p>
<p>float C, F;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>double C, F;</p>
<p>C=38.5555555555555555;</p>
<p>F = 9*C/5 +32;</p>
<p>cout&lt;&lt;"temperature in Fahrenheit= "&lt;&lt; F;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>If you want to supply the value for C through the key board, then the statement:</p>
<p>C=38.5;</p>
<p>should be replaced by the statements:</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;C;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float C, F;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;C;</p>
<p>F = 9*C/5 +32;</p>
<p>cout&lt;&lt;"temperature in Fahrenheit= "&lt;&lt; F;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 23.6</p>
<p>temperature in Fahrenheit = 74.48</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 4.8</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to find the product of two numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, product;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>product = a * b;</p>
<p>cout&lt;&lt;"the product of a and b = "&lt;&lt; product;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of a and b = 2</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you insert a value 2^3 for a and 3^2 for b, then as said earlier wrong result or compilation error will be flagged on the screen.</p>
<p>&nbsp;</p>
<p>a=2^3;</p>
<p>b=3^2; ---&gt; ERROR</p>
<p>a=2* 2*2</p>
<p>b=3*3; ---&gt; Result will be outputted on the screen i.e.,</p>
<p>the product of a and b = 72</p>
<p>&nbsp;</p>
<p>If you want to insert a 10 digit number for a and b i.e.,</p>
<p>a=1000000000</p>
<p>b=3000000000, then the statement:</p>
<p>int a, b, product;</p>
<p>should be replaced by the statement:</p>
<p>long int a, b, product;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>long int a, b, product;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>product = a * b;</p>
<p>cout&lt;&lt;"the product of a and b = "&lt;&lt; product;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of a and b = 3000000000000000000</p>
<p>&nbsp;</p>
<p>If you want to supply the integer values for a and b through the key board, then the statements:</p>
<p>a=1;</p>
<p>b=2; should be replaced by the statements:</p>
<p>cout&lt;&lt;"Enter any two numbers:";</p>
<p>cin &gt;&gt; a;</p>
<p>cin &gt;&gt; b;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main ()</p>
<p>{</p>
<p>int a, b, product;</p>
<p>cout&lt;&lt;"Enter any two numbers:";</p>
<p>cin&gt;&gt;a;</p>
<p>cin&gt;&gt;b;</p>
<p>product = a* b;</p>
<p>cout&lt;&lt;"the product of a and b = "&lt;&lt; product;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two numbers:</p>
<p>If you enter two numbers 2 &amp; 3</p>
<p>the product of a and b = 6</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>cout&lt;&lt;the product of a and b = &lt;&lt; product;</p>
<p>is written instead of the statement:</p>
<p>cout&lt;&lt;"the product of a and b = "&lt;&lt; product;</p>
<p>i.e., the statement the product of a and b =&nbsp; is not enclosed by the double quotation marks</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p><strong>Program 4.9</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to find the square of a number</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b = a * a;</p>
<p>cout&lt;&lt;"the square of a = "&lt;&lt; b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the square of a = 4</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to supply the integer value for a through the key board, then the statement:</p>
<p>a=2;</p>
<p>should be replaced by the statements:</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>b = a * a;</p>
<p>cout&lt;&lt;"the square of a = "&lt;&lt; b;</p>
<p>return 0;</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter a number 3</p>
<p>the square of a = 9</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>If the statement:</p>
<p>int main();</p>
<p>is written instead of int main() then the error will be displayed on the screen</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the cube of a number</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>b = a * a*a;</p>
<p>cout&lt;&lt;"the cube of a = "&lt;&lt; b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the force applied to the mass m.</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int m, a, F;</p>
<p>cout&lt;&lt;"Enter the mass:";</p>
<p>cin&gt;&gt;m;</p>
<p>cout&lt;&lt;"Enter acceleration:";</p>
<p>cin&gt;&gt;a;</p>
<p>F = m * a;</p>
<p>cout&lt;&lt;"the force applied to the mass =&nbsp; "&lt;&lt; F;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 5.0</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C ++ program to find the greatest of two numbers using if - else statement</strong></p>
<p>&nbsp;</p>
<p>The syntax of&nbsp; if - else statement is:</p>
<p>&nbsp;</p>
<p><strong>if (this condition is true)</strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>else </strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement;</strong></p>
<p><strong>}</strong></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a = 2;</p>
<p>b = 3;</p>
<p>if(a&gt;b)</p>
<p>{</p>
<p>cout&lt;&lt;"a is greater than b";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"b is greater than a";</p>
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
<p>if the condition (a&gt;b) is true, then the statement</p>
<p>{</p>
<p>cout&lt;&lt;"a is greater than b";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>a is greater than b</p>
<p>else the statement</p>
<p>{</p>
<p>cout&lt;&lt;"b is greater than a";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>b is greater than a</p>
<p>&nbsp;</p>
<p>If you want to supply the integer values for a and b through the key board, then the statements:</p>
<p>a=2;</p>
<p>b=3; should be replaced by the statements</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>scanf("%d", &amp;a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>scanf("%d", &amp;b;</p>
<p>&nbsp;</p>
<p>i.e., the program should be rewritten as:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>scanf("%d", &amp;a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>scanf("%d", &amp;b;</p>
<p>if(a&gt;b)</p>
<p>{</p>
<p>cout&lt;&lt;"a is greater than b";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"b is greater than a";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 6</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>a is greater than b</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 5.1</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to find the greatest of three numbers using if &ndash; else if &ndash; else&nbsp; statement</strong></p>
<p>&nbsp;</p>
<p>The syntax of if - else&nbsp; if - else statement:</p>
<p>&nbsp;</p>
<p><strong>if (this condition is true)</strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>else if (this condition is true)</strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>else&nbsp; </strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>&nbsp;</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;b;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;c;</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>{</p>
<p>cout&lt;&lt; a&lt;&lt;" is greater than"&lt;&lt; b&lt;&lt;" and "&lt;&lt;c;</p>
<p>}</p>
<p>else if (b&gt;a&amp;&amp;b&gt;c)</p>
<p>{</p>
<p>cout&lt;&lt; b&lt;&lt;" is greater than"&lt;&lt; a &lt;&lt;" and "&lt;&lt;c;</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt; c&lt;&lt;" is greater than"&lt;&lt; b&lt;&lt;" and "&lt;&lt; a;</p>
<p>}</p>
<p>&nbsp;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 4</p>
<p>4 is greater than 3 and 2 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>double ampersand "&amp;&ampamp;" imply:</p>
<p>and</p>
<p>(a&gt;b&amp;&amp;a&gt;c)</p>
<p>(b&gt;a&amp;&amp;b&gt;c)</p>
<p>denote conditions.</p>
<p>i.e., the condition</p>
<p>(a&gt;b&amp;&amp;a&gt;c) imply:</p>
<p>a is greater than b and a is greater than c</p>
<p>and if this condition is true, then the statement:</p>
<p>{</p>
<p>cout&lt;&lt; a&lt;&lt;" is greater than"&lt;&lt; b&lt;&lt;" and "&lt;&lt;c;</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>a is greater than b and c</p>
<p>and if the condition (a&gt;b&amp;&amp;a&gt;c) is not true</p>
<p>the statement</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt; a&lt;&lt;" is greater than"&lt;&lt; b&lt;&lt;" and "&lt;&lt;c;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is not executed; instead the execution skips and pass to the condition (b&gt;a&amp;&amp;b&gt;c)</p>
<p>and if this condition is true, then the statement:</p>
<p>{</p>
<p>cout&lt;&lt; b&lt;&lt;" is greater than"&lt;&lt; a &lt;&lt;" and "&lt;&lt;c;</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>b is greater than a and c</p>
<p>and if the condition (b&gt;a&amp;&amp;b&gt;c) is not true, then the statement:</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt; b&lt;&lt;" is greater than"&lt;&lt; a &lt;&lt;" and "&lt;&lt;c;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is not executed; instead the execution skips and the statement:</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt; c&lt;&lt;" is greater than"&lt;&lt; b&lt;&lt;" and "&lt;&lt; a;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>c is greater than b and a</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program?</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include &lt;iostream&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b=2;</p>
<p>if(a&gt;b || a= = b)</p>
<p>cout&lt;&lt;"a is greater than or equal to b";</p>
<p>else</p>
<p>cout&lt;&lt;"b is greater than a";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>a is greater than or equal to b</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>Note:</strong> symbol || denote OR i.e., a&gt;b || a = = b denote a is greater than or a is equal to b.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 5.2</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C ++&nbsp; program to find the average of 10 numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int N1, N2, N3, N4, N5, N6, N7, N8, N9, N10, X;</p>
<p>cout&lt;&lt;"Enter any 10 numbers:";</p>
<p>cin&gt;&gt;N1;</p>
<p>cin&gt;&gt;N2;</p>
<p>cin&gt;&gt;N3;</p>
<p>cin&gt;&gt;N4;</p>
<p>cin&gt;&gt;N5;</p>
<p>cin&gt;&gt;N6;</p>
<p>cin&gt;&gt;N7;</p>
<p>cin&gt;&gt;N8;</p>
<p>cin&gt;&gt;N9;</p>
<p>cin&gt;&gt;N10;</p>
<p>X = (N1 + N2 + N3 + N4 + N5 + N6 + N7 + N8 + N9 + N10) /10;</p>
<p>cout&lt;&lt;"the average of 10 numbers = "&lt;&lt; X;</p>
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
<li><strong>Note:</strong> The average of 10 numbers is 5.5, the output on the screen is 5 because int is used instead of float.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>Like in C language, any mathematical expression should be written in C ++ equivalent expression to prevent the display of compilation error on the screen because C ++ language also does not accept the general mathematical expressions.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> C++ equivalent mathematical expression is same as C equivalent mathematical expression</li>
</ul>
<p>&nbsp;</p>
<p><strong>For example:</strong></p>
<p>&nbsp;</p>
<table width="414">
<tbody>
<tr>
<td width="143">
<p><strong>Mathematical expression:</strong></p>
</td>
<td width="131">
<p><strong>C equivalent expression:</strong></p>
</td>
<td width="140">
<p><strong>C++ equivalent expression:</strong></p>
</td>
</tr>
<tr>
<td width="143">
<p>log<sub>10</sub>x + bx</p>
</td>
<td width="131">
<p>log10 (x) + b * x</p>
</td>
<td width="140">
<p>log10 (x) + b * x</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 5.3</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C ++ program to find the square root of a number</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;cmath&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt; a;</p>
<p>b = sqrt (a);</p>
<p>cout&lt;&lt;"the square root of a number = "&lt;&lt;&nbsp; b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 16</p>
<p>the square root of a number = 4</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>This program can also be written as:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;cmath&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"the square root of a number =&nbsp; "&lt;&lt; sqrt (4);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Suppose if you enter the number 8,</p>
<p>the square root of a number = 2</p>
<p>will be outputted instead of</p>
<p>the square root of a number = 2.82</p>
<p>on the screen because int is used instead of float.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> Since b = sqrt (a) is written</li>
</ul>
<p>the statement:</p>
<p>&nbsp;</p>
<p>#include&lt;cmath&gt; must be included in the above program because cmath file defines the mathematical functions like sqrt().</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>&nbsp;</p>
<p>#include&lt;cmath&gt; is not included in the above program:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt; a;</p>
<p>b = sqrt (a);</p>
<p>cout&lt;&lt;"the square root of a number = "&lt;&lt;&nbsp; b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;math.h&gt; is used in C</p>
<p>whereas #include&lt;cmath&gt; is used in C ++</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the cube root of a number:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer: </strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;cmath&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;"the cube root of a number =&nbsp; "&lt;&lt; cbrt (8);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 5.4</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to find the simple interest</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int P,T, R, SI;</p>
<p>P = 1000;</p>
<p>T = 2;</p>
<p>R = 3;</p>
<p>SI = P*T*R/100;</p>
<p>cout&lt;&lt;"the simple interest = "&lt;&lt; SI;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the simple interest = 60</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>If you write:</p>
<p>SI = PTR/100;</p>
<p>instead of:</p>
<p>SI = P*T*R/100;</p>
<p>Then the compilation error is displayed on the screen because (like C) C ++ language does not accept the general expressions.</p>
<p>&nbsp;</p>
<p>If you want to supply the integer values for P, T and R through the key board, then the statements:</p>
<p>P = 1000;</p>
<p>T = 2;</p>
<p>R = 3;</p>
<p>should be replaced by the statements:</p>
<p>cout&lt;&lt;"Enter principal amount:";</p>
<p>cin&gt;&gt;P;</p>
<p>cout&lt;&lt;"Enter time:";</p>
<p>cin&gt;&gt;T;</p>
<p>cout&lt;&lt;"Enter rate of interest:";</p>
<p>cin&gt;&gt;R;</p>
<p>i.e., the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int P,T, R, SI;</p>
<p>cout&lt;&lt;"Enter principal amount:";</p>
<p>cin&gt;&gt;P;</p>
<p>cout&lt;&lt;"Enter time:";</p>
<p>cin&gt;&gt;T;</p>
<p>cout&lt;&lt;"Enter rate of interest:";</p>
<p>cin&gt;&gt;R;</p>
<p>SI = P*T*R/100;</p>
<p>cout&lt;&lt;"the simple interest = "&lt;&lt;SI;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter principal amount:</p>
<p>If you enter the principal amount 1000</p>
<p>Enter time:</p>
<p>If you enter the time 2</p>
<p>Enter rate of interest:</p>
<p>If you enter the rate of interest 3</p>
<p>the simple interest = 60</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 5.5</strong></p>
<p><strong>C++ program to find the senior citizen</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int age;</p>
<p>age=20;</p>
<p>if(age &gt; = 60)</p>
<p>{</p>
<p>cout&lt;&lt;"senior citizen";</p>
<p>}</p>
<p>if(age&lt;60)</p>
<p>{</p>
<p>cout&lt;&lt;"not a senior citizen";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>not a senior citizen</p>
<p>(age &gt; = 60) means: age greater than or equal to 60.</p>
<p>&nbsp;</p>
<p>If you want to supply the value for age through the key board, then the statement:</p>
<p>age = 20;</p>
<p>should be replaced by the statements:</p>
<p>cout&lt;&lt;"Enter age:";</p>
<p>cin&gt;&gt;age;</p>
<p>i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int age;</p>
<p>cout&lt;&lt;"Enter age:";</p>
<p>cin&gt;&gt;age;</p>
<p>if(age&gt;60)</p>
<p>{</p>
<p>cout&lt;&lt;"senior citizen";</p>
<p>}</p>
<p>if(age&lt;60)</p>
<p>{</p>
<p>cout&lt;&lt;"not a senior citizen";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter age:</p>
<p>If you enter the age 60</p>
<p>senior citizen</p>
<p>will be outputted on the screen.</p>
<p>Suppose if you enter the age 31</p>
<p>not a senior citizen</p>
<p>will be outputted on the screen</p>
<p>&nbsp;</p>
<p><strong>Program 5.6</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C ++ program to get marks for 3 subjects and declare the result.</strong></p>
<p><strong>If the marks &gt;= 35 in all the subjects the student passes else fails.</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int M1, M2, M3;</p>
<p>M1 = 38;</p>
<p>M2= 45;</p>
<p>M3 = 67;</p>
<p>if(M1 &gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35)</p>
<p>{</p>
<p>cout&lt;&lt;"candidate is passed";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"candidate is failed";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>candidate is passed</p>
<p>&nbsp;</p>
<p>&gt;= imply: greater than or equal to and double ampersand imply: and</p>
<p>(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35) denote the condition and this condition imply M1 is greater than or equal to 35</p>
<p>and M2 is greater than or equal to 35 and M3 is greater than or equal to 35. And if this condition is TRUE, then the statement</p>
<p>{</p>
<p>cout&lt;&lt;"candidate is passed";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>candidate is passed</p>
<p>else the statement:</p>
<p>{</p>
<p>cout&lt;&lt;"candidate is failed";</p>
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
<p>cout&lt;&lt;"Enter any three marks:";</p>
<p>cin&gt;&gt; M1;</p>
<p>cin&gt;&gt; M2;</p>
<p>cin&gt;&gt; M3;</p>
<p>&nbsp;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>int main()</p>
<p>{</p>
<p>int M1, M2, M3;</p>
<p>cout&lt;&lt;"Enter any three marks:";</p>
<p>cin&gt;&gt; M1;</p>
<p>cin&gt;&gt; M2;</p>
<p>cin&gt;&gt; M3;</p>
<p>if(M1 &gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35)</p>
<p>{</p>
<p>cout&lt;&lt;"candidate is passed";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"candidate is failed";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any three numbers:</p>
<p>If you enter three numbers 26, 28, 39</p>
<p>candidate is failed</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p><strong>Program 5.7</strong></p>
<p><strong>C ++ program to find profit or loss</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int CP, SP, loss, profit;</p>
<p>cout&lt;&lt;"Enter cost price:";</p>
<p>cin &gt;&gt; CP;</p>
<p>cout&lt;&lt;"Enter selling price:";</p>
<p>cin&gt;&gt;SP;</p>
<p>if ( SP &gt; CP )</p>
<p>{</p>
<p>cout&lt;&lt;"profit= "&lt;&lt; SP-CP;</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"loss = "&lt;&lt; CP-SP;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter cost price:</p>
<p>If you enter the cost price 25</p>
<p>Enter selling price:</p>
<p>If you enter the selling price 26</p>
<p>profit = 1</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the condition (SP&gt;CP) is true, then the statement:</p>
<p>{</p>
<p>cout&lt;&lt;"profit= "&lt;&lt; SP-CP;</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>profit = SP-CP (in this case profit = 26-25 =1)</p>
<p>else the statement:</p>
<p>{</p>
<p>cout&lt;&lt;"loss = "&lt;&lt; CP-SP;</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>loss = CP-SP</p>
<p>&nbsp;</p>
<p><strong>Program 5.8</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to convert inches into centimeter</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float I, C;</p>
<p>I=3.5;</p>
<p>C = 2.54*I;</p>
<p>cout&lt;&lt;"length in centimeters = "&lt;&lt; C;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>length in centimeters = 8.89</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> float is used instead of int because I = 3.5 if int is used instead of float then the result will not be clearly outputted i.e., instead of 8.89 the computer displays only 8.</li>
</ul>
<p>&nbsp;</p>
<p>If you want to supply the value for I through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float I, C;</p>
<p>cout&lt;&lt;"Enter the length in inches:";</p>
<p>cin &gt;&gt; I;</p>
<p>C = 2.54*I;</p>
<p>cout&lt;&lt;"length in centimeters= "&lt;&lt; C;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter the length in inches:</p>
<p>If you enter the value for I i.e., 25.5</p>
<p>length in centimeters = 64.9 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Suppose</p>
<p>If you enter the value 25</p>
<p><strong>The output on the screen:</strong></p>
<p>length in centimeters = 63.5</p>
<p>Even if you enter the value 25 instead of 25.5, float should be used instead of int because if float is not used then</p>
<p>C = 63 will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 5.9</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to find the incremented and decremented values of two numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c, d, e, f;</p>
<p>a = 10;</p>
<p>b=12;</p>
<p>c=a+1;</p>
<p>d=b+1;</p>
<p>e=a-1;</p>
<p>f=b-1;</p>
<p>cout&lt;&lt;"the incremented value of a = "&lt;&lt; c;</p>
<p>cout&lt;&lt;"the incremented value of b = "&lt;&lt; d;</p>
<p>cout&lt;&lt;"the decremented value of a = "&lt;&lt; e;</p>
<p>cout&lt;&lt;"the decremented value of b = "&lt;&lt; f;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the incremented value of a = 11 the incremented value of b = 13 the decremented value of a = 9 the decremented value of b = 11</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>cout&lt;&lt;"the incremented value of a = "&lt;&lt; c;</p>
<p>cout&lt;&lt;"the incremented value of b = "&lt;&lt; d;</p>
<p>cout&lt;&lt;"the decremented value of a = "&lt;&lt; e;</p>
<p>cout&lt;&lt;"the decremented value of b = "&lt;&lt; f;</p>
<p>are replaced by the statements:</p>
<p>cout&lt;&lt;"\n the incremented value of a = "&lt;&lt; c;</p>
<p>cout&lt;&lt;"\n the incremented value of b = "&lt;&lt; d;</p>
<p>cout&lt;&lt;"\n the decremented value of a = "&lt;&lt; e;</p>
<p>cout&lt;&lt;"\n the decremented value of b = "&lt;&lt; f;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>the incremented value of a = 11</p>
<p>the incremented value of b = 13</p>
<p>the decremented value of a = 9</p>
<p>the decremented value of b = 11</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>&nbsp;</p>
<p>cout&lt;&lt;"the incremented value of a = "&lt;&lt; c;</p>
<p>cout&lt;&lt;"the incremented value of b = "&lt;&lt; d;</p>
<p>cout&lt;&lt;"the decremented value of a = "&lt;&lt; e;</p>
<p>cout&lt;&lt;"the decremented value of b = "&lt;&lt; f;</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>cout&lt;&lt;"the incremented value of a = "&lt;&lt; c &lt;&lt; endl ;</p>
<p>cout&lt;&lt;"the incremented value of b = "&lt;&lt; d &lt;&lt; endl;</p>
<p>cout&lt;&lt;"the decremented value of a = "&lt;&lt; e &lt;&lt; endl;</p>
<p>cout&lt;&lt;"the decremented value of b = "&lt;&lt; f &lt;&lt; endl;</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong>:</p>
<p>&nbsp;</p>
<p>the incremented value of a = 11</p>
<p>the incremented value of b = 13</p>
<p>the decremented value of a = 9</p>
<p>the decremented value of b = 11</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board,</p>
<p>then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c, d, e, f;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt; a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt; b;</p>
<p>c=a+1;</p>
<p>d=b+1;</p>
<p>e=a-1;</p>
<p>f=b-1;</p>
<p>cout&lt;&lt;"\n the incremented value of a = "&lt;&lt; c;</p>
<p>cout&lt;&lt;"\n the incremented value of b = "&lt;&lt; d;</p>
<p>cout&lt;&lt;"\n the decremented value of a = "&lt;&lt; e;</p>
<p>cout&lt;&lt;"\n the decremented value of b = "&lt;&lt; f;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>the incremented value of a = 3</p>
<p>the incremented value of b = 4</p>
<p>the decremented value of a = 1</p>
<p>the decremented value of b = 2</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>b++ is same as b+1 and b-- is same as b-1</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float T1, T2, A;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin &gt;&gt;T1;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin &gt;&gt;T2;</p>
<p>A = (T1 + T2) / 2;</p>
<p>cout&lt;&lt;"the average temperature of the day = "&lt;&lt; A;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>Enter any number:</p>
<p>If you enter the number:</p>
<p>2</p>
<p>Enter any number:</p>
<p>If you enter the number:</p>
<p>3</p>
<p>the average temperature of the day = 2.5</p>
<p>will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p><strong>Program 6.0</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>The percentage marks are entered and the grades are allotted as follows:</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>percentage &gt;= 60 First Class</p>
<p>percentage &gt;=50 and per &lt;= 60 Second Class</p>
<p>percentage &gt;= 40 and per &lt;= 50 Pass Class</p>
<p>percentage &lt; 40 Fail</p>
<p><strong>Write a C++ program for the above:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>main()</p>
<p>{</p>
<p>int P;</p>
<p>cout&lt;&lt;"Enter the percentage:";</p>
<p>cin&gt;&gt;P;</p>
<p>if(P &gt;= 60)</p>
<p>{</p>
<p>cout&lt;&lt;"first class";</p>
<p>}</p>
<p>if(P&gt;=50&amp;&amp;P &lt;60)</p>
<p>{</p>
<p>cout&lt;&lt;"second class";</p>
<p>}</p>
<p>if(P&gt;=40&amp;&amp;P&lt;=50 )</p>
<p>{</p>
<p>cout&lt;&lt;"pass class";</p>
<p>}</p>
<p>if(P&lt;40)</p>
<p>{</p>
<p>cout&lt;&lt;"fail";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter the percentage:</p>
<p>If you enter the percentage 35</p>
<p>fail</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 6.1</strong></p>
<p><strong>C++ program to calculate the discounted price and the total price after discount</strong></p>
<p><strong>Given:</strong></p>
<p>If purchase value is greater than 1000, 10% discount</p>
<p>If purchase value is greater than 5000, 20% discount</p>
<p>If purchase value is greater than 10000, 30% discount</p>
<p>&nbsp;</p>
<ul>
<li><strong>discounted price</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>double PV, dis;</p>
<p>cout&lt;&lt;"Enter purchased value:";</p>
<p>cin&gt;&gt;PV;</p>
<p>if(PV&gt;1000)</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.1;</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.2;</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.3;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 6500</p>
<p>dis = 1300.000000</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>(PV&gt;1000), (PV&gt;5000) denote the conditions and if the condition (PV&gt;1000) is true i.e., purchased value is greater than 1000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.1;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 10% = PV* 10 /100 = PV* 0.1</p>
<p>and if the condition (PV&gt;1000) is false and if the condition (PV&gt;5000) is true i.e., purchased value is greater than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.2;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 20% = PV* 20 /100 = PV* 0.2</p>
<p>and if the condition (PV&gt;5000) is not true i.e., purchased value is less than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.3;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 30% = PV* 30 /100 = PV* 0.3</p>
<p>&nbsp;</p>
<ul>
<li><strong>total price </strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>double PV, total;</p>
<p>cout&lt;&lt;"Enter purchased value:";</p>
<p>scanf("%lf", &amp;PV;</p>
<p>if(PV&lt;1000)</p>
<p>{</p>
<p>cout&lt;&lt;"total= "&lt;&lt; PV - PV* 0.1;</p>
<p>}</p>
<p>else if(PV&lt;5000)</p>
<p>{</p>
<p>cout&lt;&lt;"total = "&lt;&lt; PV- PV* 0.2;</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"total= "&lt;&lt; PV- PV* 0.3;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 650</p>
<p>total = 585.000000</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If the condition (PV&gt;1000) is true i.e., purchased value is greater than 1000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt;"total = %d", PV - PV* 0.1;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*10% = PV- PV* 10 /100 = PV - PV * 0.1</p>
<p>and if the condition (PV&gt;1000) is false and if the condition (PV&gt;5000) is true i.e., purchased value is greater than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt;"total = %d", PV - PV* 0.2;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*20% = PV- PV* 20 /100 = PV - PV * 0.2</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>and if the condition (PV&gt; 5000) is not true i.e., purchased value is less than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>cout&lt;&lt;"total = %d", PV - PV* 0.3;</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>&nbsp;</p>
<p>total =PV- dis = PV- PV*30% = PV- PV* 30 /100 = PV - PV * 0.3</p>
<p>&nbsp;</p>
<ul>
<li><strong>Now, Combing both the programs (above), we can write:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>double PV, dis, total;</p>
<p>cout&lt;&lt;"Enter purchased value:";</p>
<p>cin&gt;&gt;PV;</p>
<p>if(PV&gt;1000)</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.1;</p>
<p>cout&lt;&lt;"total= "&lt;&lt; PV - PV* 0.1;</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>cout&lt;&lt;"dis = "&lt;&lt; PV* 0.2;</p>
<p>cout&lt;&lt;"total= "&lt;&lt; PV - PV* 0.1;</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"dis= "&lt;&lt; PV* 0.3;</p>
<p>cout&lt;&lt;"total= "&lt;&lt; PV - PV* 0.1;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 850</p>
<p>dis = 85.000000</p>
<p>total = 765.000000</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 6.2</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to print the first ten natural numbers using for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i=1; i&lt;=10; i++)</p>
<p>cout&lt;&lt;"value of i = "&lt;&lt; i;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>value of i = 1 value of i = 2&nbsp; value of i = 3&nbsp; value of i = 4&nbsp; value of i= 5&nbsp; value of i= 6 value of i = 7 value of i= 8&nbsp; value of i= 9&nbsp; value of i= 10</p>
<p>&nbsp;</p>
<p>for (i=1; i&lt;=10; i++) denote the</p>
<p>for loop statement and the syntax of the</p>
<p>for loop statement is:</p>
<p>for (initialization; condition; increment)</p>
<p>Here:</p>
<p>i=1 denote initialization (i.e., from where to start)</p>
<p>i&lt;=10 denote the condition (i.e., stop when 10 is reached)</p>
<p>i++ implies increment (which tells the value of i to increase by 1 each time the loop is executed) and i++ is the same as i+1.</p>
<p>&nbsp;</p>
<ul>
<li><strong>When for loop executes, the following occurs:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>i = 1</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=1</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 1</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 1+1 = 2</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=2</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 2</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 2+1 = 3</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=3</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 3</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 3+1 = 4</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=4</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 4</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 4+1 = 5</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=5</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 5</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 5+1 = 6</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=6</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 6</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 6+1 = 7</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=7</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 7</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 7+1 = 8</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=8</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 8</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 8+1 = 9</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=9</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 9</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 9+1 = 10</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=10</p>
<p>The statement cout&lt;&lt;"value of i = "&lt;&lt; i; is executed to print the output:</p>
<p>value of i = 10</p>
<p>and stop because the condition i&lt;=10 is achieved.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>cout&lt;&lt;"value of i = "&lt;&lt; i;</p>
<p>is replaced by the statement:</p>
<p>cout&lt;&lt;"\n value of i = "&lt;&lt; i;</p>
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
<p>cout&lt;&lt;"value of i = "&lt;&lt; i; is replaced by the statement:</p>
<p>cout&lt;&lt;"\n "&lt;&lt; i;</p>
<p>&nbsp;</p>
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
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i =1; i&lt;=5; i ++)</p>
<p>cout&lt;&lt;"\n Linux is not portable";</p>
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
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the first ten natural numbers using for while loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>The syntax of while loop statement is:</p>
<p>&nbsp;</p>
<p><strong>while (this is the condition)</strong></p>
<p><strong>{</strong></p>
<p><strong>execute this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i = 1;</p>
<p>while (i&lt;=10)</p>
<p>{</p>
<p>cout&lt;&lt;"\n "&lt;&lt; i++;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
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
<p>cout&lt;&lt;"\n "&lt;&lt; i++;</p>
<p>&nbsp;</p>
<p>is repeatedly executed as long as a given condition (i&lt;=10) is true.</p>
<p>&nbsp;</p>
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
<p>Then the <strong>output on the screen</strong> is:</p>
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
<p>Then the <strong>output on the screen</strong> is:</p>
<p>7</p>
<p>8</p>
<p>9</p>
<p>10</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print first 10 numbers using do while loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>The syntax of do while loop statement is:</p>
<p>&nbsp;</p>
<p><strong>do</strong></p>
<p><strong>{</strong></p>
<p><strong>execute this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>while(this is the condition;</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i =1;</p>
<p>do</p>
<p>{</p>
<p>cout&lt;&lt;" \n i= "&lt;&lt; i++;</p>
<p>} while (i&lt;=10);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>The <strong>output on the screen</strong> is:</p>
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
<p>cout&lt;&lt;" \ni= "&lt;&lt; i++;</p>
<p>is executed and then condition (i&lt;=10) is checked. If condition (i&lt;=10) is true then</p>
<p>The statement:</p>
<p>cout&lt;&lt;" \ni= "&lt;&lt; i++;</p>
<p>is executed again. This process repeats until the given condition (i&lt;=10) becomes false.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print </strong></li>
</ul>
<p>When in doubt use brute force</p>
<p><strong>100 times using for loop statement.</strong></p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for(i=0; i&lt;=99; i++)</p>
<p>cout&lt;&lt;"\n When in doubt use brute force";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 6.3</strong></p>
<p><strong>C++ program to print the characters from A to Z using for loop, do while loop and while loop statement.</strong></p>
<p>&nbsp;</p>
<ul>
<li><strong>C ++ program to print the characters from A to Z using for loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char a;</p>
<p>for( a='A'; a&lt;='Z'; a++)</p>
<p>cout&lt;&lt;" \n"&lt;&lt; a;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
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
<p>char means the data type is character.</p>
<p>The statement:</p>
<p>char a;</p>
<p>imply that we are creating the character a.</p>
<p>If the statement:</p>
<p>for( a=A; a&lt;=Z; a++) is written instead of the statement for( a='A'; a&lt;='Z'; a++)</p>
<p>i.e., A is used instead of 'A' and Z is used instead of 'Z', then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C ++ program to print the characters from A to Z using while loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char a = 'A';</p>
<p>while (a&lt;='Z')</p>
<p>{</p>
<p>cout&lt;&lt;" \n"&lt;&lt; a++;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>C ++ program to print the characters from A to Z using do while loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char a = 'A';</p>
<p>do</p>
<p>{</p>
<p>cout&lt;&lt;" \n"&lt;&lt; a++;</p>
<p>} while (a&lt;='Z');</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 6.4</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to print the given number is even or odd.</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>if(a%2 = = 0)</p>
<p>{</p>
<p>cout&lt;&lt;"the number is even";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"the number is odd";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 6</p>
<p>the number is even</p>
<p>will be outputted on the screen.</p>
<p>(a%2 = = 0) is the condition and this condition imply: a divided by 2 yields reminder = 0.</p>
<p>For example: if you enter the number 2</p>
<p>Then a = 2</p>
<p>Then 2 divided by 2 yields the remainder = 0</p>
<p>Then the statement</p>
<p>{</p>
<p>cout&lt;&lt;"the number is even";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>the number is even</p>
<p>(<strong>Note:</strong>(like in C) in C ++ language = = implies: equal to)</p>
<p>If you enter the number 3</p>
<p>Then a = 3</p>
<p>Then 3 divided by 2 yields the remainder = 1</p>
<p>Then the statement</p>
<p>{</p>
<p>cout&lt;&lt;"the number is odd";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>the number is odd</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 6.5</strong></p>
<p><strong>C++ program to print the remainder of two numbers </strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;b;</p>
<p>c = a % b;</p>
<p>cout&lt;&lt;"the remainder of a and b = "&lt;&lt; c;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>the remainder of a and b = 1</p>
<p>will be outputted on the screen.</p>
<p>Since (a =3 and b =2). Therefore:</p>
<p>3 divided by 2 (i.e., a divided by b) yields the remainder equal to 1</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>cout&lt;&lt;"the remainder of a and b = "&lt;&lt; c; is replaced by the statement:</p>
<p>cout &lt;&lt;" the remainder of "&lt;&lt;a &lt;&lt;"and"&lt;&lt; b &lt;&lt;"=&nbsp; "&lt;&lt; c;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b, c;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;b;</p>
<p>c = a % b;</p>
<p>cout &lt;&lt;" the remainder of "&lt;&lt;a &lt;&lt;"and"&lt;&lt; b &lt;&lt;"=&nbsp; "&lt;&lt; c;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>the remainder of 3 and 2 = 1</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 6.6</strong></p>
<p><strong>C++ program to check equivalence of two numbers</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;x;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;y;</p>
<p>if(x-y==0)</p>
<p>{</p>
<p>cout&lt;&lt;"the two numbers are equivalent";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"the number are not equivalent";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>Enter any number:</p>
<p>If you enter the number 2</p>
<p>the two numbers are equivalent</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Since 2-2 is equal to 0 (i.e., x-y = = 0). Therefore: the statement</p>
<p>{</p>
<p>cout&lt;&lt;"the two numbers are equivalent";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>two numbers are equivalent</p>
<p>If you enter the numbers 3 and 2</p>
<p>The output on the screen:</p>
<p>the two numbers are not equivalent</p>
<p>Since 3-2 is not equal to 0 (i.e., x-y!= 0). Therefore: the statement</p>
<p>{</p>
<p>cout&lt;&lt;"the two numbers are not equivalent";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>two numbers are not equivalent</p>
<p>(<strong>Note:</strong> (like in C) in C ++ language != implies not equal to)</p>
<p>&nbsp;</p>
<p><strong>Program 6.7</strong></p>
<p><strong>C ++ program to print whether the given number is positive or negative</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a;</p>
<p>a = -35;</p>
<p>if(a&gt;0)</p>
<p>{</p>
<p>cout&lt;&lt;"number is positive";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;" number entered is negative";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>number entered is negative</p>
<p>Since a = -35. Therefore:</p>
<p>a is less than 0 i.e., a &lt; 0 because any negative number is always less than zero.</p>
<p>The statement:</p>
<p>{</p>
<p>cout&lt;&lt;"number is negative";</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>number entered is negative</p>
<p>&nbsp;</p>
<p><strong>Program 6.8</strong></p>
<p><strong>C++ program to print the sum of the first 10 numbers using for loop statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>cout&lt;&lt;"sum of the first10 numbers = "&lt;&lt; sum;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 digits = 55</p>
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
<p>cout&lt;&lt;"sum of the first 10 digits = "&lt;&lt; sum;</p>
<p>is executed to print the output:</p>
<p>sum of the first 10 digits = 55</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>int i, sum = 0;</p>
<p>is replaced by int i, sum = 1;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>sum of the first10 digits = 56</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output if the for loop statement</strong> for(i =1; i&lt;=10; i++) <strong>is replaced by the statement</strong> for(i =2; i&lt;10; i++)?</li>
</ul>
<p><strong>Answer:</strong>&nbsp; sum of 10 digits = 44</p>
<p>&nbsp;</p>
<p>If the statement int i, sum, sum = 0; is written instead of int i, sum = 0;</p>
<p>Then the compilation error message will be displayed on the screen (stating that sum is twice declared).</p>
<p>&nbsp;</p>
<p>If the for loop is ended with a semicolon i.e.,</p>
<p>for( i=1; i&lt;=10; i++;</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p>//--------------------------------------------------------------------------------------</p>
<p>sum = sum + a; is the same as sum + = a;</p>
<p>sub = sub - a; is the same as sub - = a;</p>
<p>product = product* a; is the same as product * = a;</p>
<p>div = div / a; is the same as div /= a;</p>
<p>a = a% b; is the same as a % = b;</p>
<p>----------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<p><strong>Program 6.9</strong></p>
<p><strong>C++ program to print the average of the first 10 numbers using for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i, avg, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>avg = sum/10;</p>
<p>cout&lt;&lt;"sum of the first 10 numbers = "&lt;&lt; sum;</p>
<p>cout&lt;&lt;"average of the first 10 numbers = "&lt;&lt; avg;</p>
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
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float i, avg, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>avg = sum/10;</p>
<p>cout&lt;&lt;"sum of the first 10 numbers = "&lt;&lt; sum;</p>
<p>cout&lt;&lt;"average of the first 10 numbers = "&lt;&lt; avg;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 numbers = 55</p>
<p>average of the first 10 numbers = 5.5</p>
<p>&nbsp;</p>
<p><strong>Program 7.0</strong></p>
<p><strong>C++ program to print the product of the first 10 digits using for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i, product = 1;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>product = product * i;</p>
<p>cout&lt;&lt;"the product of the first 10 digits =%d", product;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of the first 10 digits = 3628800</p>
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
<p>cout&lt;&lt;"the product of the first 10 digits = "&lt;&lt; product; is executed to display the output:</p>
<p>the product of the first 10 digits = 3628800</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int i, product = 1; is replaced by int i, product = 0;</p>
<p>Then the output on the screen is:</p>
<p>the product of the first 10 digits = 0</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>for(i=1; i&lt;=10; i++) is replaced by for(i=5; i&lt;=8; i++)</p>
<p>Then the output on the screen is:</p>
<p>the product of the first 10 digits = 1680</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 7.1</strong></p>
<p><strong>C++ Program to print the table of a number using the for loop statement</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int n, i;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;n;</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>cout&lt;&lt; n &lt;&lt;"&nbsp; *&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt; n*i;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
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
<p><strong>&nbsp;</strong></p>
<p>Since you entered the number 2, therefore: n=2.</p>
<p>i=1</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 1 = 2</p>
<p>using the statement cout&lt;&lt; n &lt;&lt;"&nbsp; *&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt; n*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 2 = 4</p>
<p>using the statement cout&lt;&lt; n &lt;&lt;"&nbsp; *&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt; n*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 3 = 6</p>
<p>using the statement cout&lt;&lt; n &lt;&lt;"&nbsp; *&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt; n*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 4 = 8</p>
<p>using the statement cout&lt;&lt; n &lt;&lt;"&nbsp; *&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt; n*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=5</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 5 = 10</p>
<p>using the statement cout&lt;&lt; n &lt;&lt;"&nbsp; *&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt; n*i;</p>
<p>&nbsp;</p>
<p>stop Now because the condition i&lt;=5 is achieved.</p>
<p>&nbsp;</p>
<p>If the symbol * is replaced by +</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int n, a;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;n;</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>cout&lt;&lt; n &lt;&lt;"&nbsp; +&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"&nbsp; =&nbsp; "&lt;&lt;&nbsp; n + i &lt;&lt;endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
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
<p>&nbsp;</p>
<p><strong>Program 7.2 </strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program:&nbsp; </strong></p>
<p>If you enter a character M</p>
<p><strong>Output must be:</strong> ch = M</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
<p>cin&gt;&gt;M;</p>
<p>cout&lt;&lt;"ch= "&lt;&lt; M;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen: </strong></p>
<p>Enter any character:</p>
<p>If you enter the character M</p>
<p>ch = M</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>If we replace the statement:</p>
<p>cin&gt;&gt;M; by the statement:</p>
<p>M = getchar();</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
<p>M = getchar();</p>
<p>cout&lt;&lt;"ch= "&lt;&lt; M;</p>
<p>return 0;</p>
<p>}</p>
<p>There will be no change in the output on the screen i.e., <strong>The output on the screen</strong> is:</p>
<p>Enter any character:</p>
<p>If you enter the character K</p>
<p>ch = K</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If we replace the statement:</p>
<p>cout&lt;&lt;"ch= "&lt;&lt; M; by the statement:</p>
<p>putchar (M); i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
<p>cin&gt;&gt;M;</p>
<p>putchar (M);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>There will be no change in the output on the screen i.e., The <strong>output on the screen</strong> is:</p>
<p>Enter any character:</p>
<p>If you enter the character M</p>
<p>M will be outputted on the console screen.</p>
<p>&nbsp;</p>
<p>If we replace the statement:</p>
<p>cin&gt;&gt;M; by the statement:</p>
<p>M = getchar();</p>
<p>and the statement:</p>
<p>cout&lt;&lt;"ch= "&lt;&lt; M; by the statement:</p>
<p>putchar (M);&nbsp; i.e.,</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char M;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
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
<ul>
<li><strong>Write a program to print the absolute value of a number</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;cmath&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int a, b;</p>
<p>a= - 2;</p>
<p>b= abs(a);</p>
<p>cout&lt;&lt;" absolute value of a = "&lt;&lt; b&lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>absolute value of a = 2</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p><strong>Program 7.2</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C ++ program to print the first 5 numbers starting from one together with their squares</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square =&nbsp; "&lt;&lt; i*i;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>number=1 its square=1</p>
<p>number=2 its square=4</p>
<p>number=3 its square=9</p>
<p>number=4 its square=16</p>
<p>number=5 its square=25</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>How the execution takes its way through the for loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>i=1</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=1 its square=1</p>
<p>using the statement cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square =&nbsp; "&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=2 its square=4</p>
<p>using the statement cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square =&nbsp; "&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=3 its square=9</p>
<p>using the statement cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square =&nbsp; "&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=4 its square=16</p>
<p>using the statement cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square =&nbsp; "&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=5</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>number=5 its square=25</p>
<p>using the statement cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square = &nbsp;"&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>stop Now because the condition (i&lt;=5) is achieved.</p>
<p>&nbsp;</p>
<p>Note:</p>
<p>&nbsp;</p>
<p>If the statement cout&lt;&lt;"\n number = "&lt;&lt; i &lt;&lt;"its square = "&lt;&lt; i*i; is replaced by the statement:</p>
<p>cout&lt;&lt;"\n number =&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"\t its square =&nbsp; "&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>&nbsp;</p>
<p>number=1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; its square=1</p>
<p>number=2&nbsp;&nbsp;&nbsp;&nbsp; its square=4</p>
<p>number=3&nbsp;&nbsp;&nbsp;&nbsp; its square=9</p>
<p>number=4&nbsp;&nbsp;&nbsp;&nbsp; its square=16</p>
<p>number=5&nbsp;&nbsp;&nbsp;&nbsp; its square=25</p>
<p>&nbsp;</p>
<p>tab /t is included because to leave space between</p>
<p>number=1&nbsp;&nbsp; and&nbsp;&nbsp; its square=1</p>
<p>&nbsp;</p>
<p>Suppose cout&lt;&lt;"\n number =&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"\t its square =&nbsp; "&lt;&lt; i*i; is replaced by the statement</p>
<p>cout&lt;&lt;"\n number =&nbsp;&nbsp; "&lt;&lt; i &lt;&lt;"\n its square =&nbsp; "&lt;&lt; i*i;</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>&nbsp;</p>
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
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the first 10 numbers starting from one together with their squares and cubes?</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>cout&lt;&lt;"number =&nbsp; "&lt;&lt; i &lt;&lt;" its square =&nbsp; "&lt;&lt; i*i &lt;&lt;" its cube =&nbsp; "&lt;&lt; i*i*i&lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 7.3 </strong></p>
<p><strong>C++ program to print the sum of two numbers using pointers</strong></p>
<p>&nbsp;</p>
<p>If we create an integer variable x by declaring the statement:</p>
<p>int x;</p>
<p>within the body of the main function "main()" -- this variable is stored in the computer memory i.e.,</p>
<p>this variable occupies a specific location in the space of computer memory.</p>
<p>And this integer variable x is assigned an address (i.e., &amp;x) to locate its position in the computer memory</p>
<p>(like a house in the street is assigned an address to locate its position in the street).</p>
<p>Pointers are the variables that represent the address of x in the computer memory i.e., p = &amp;x,</p>
<p>where &amp;x imply the address of x in the computer memory and</p>
<p>p is the pointer variable (which is the variable that represent the address of x in the computer memory).</p>
<p>And further if you assign a value to the variable x by declaring the statement x=1; within the body of the</p>
<p>main function&mdash;this value is stored in the address of x in the computer memory. "*" denote pointer operator and *p denote the pointer</p>
<p>(which&nbsp; represent the value stored in the address of x in the computer memory).</p>
<p>&nbsp;</p>
<ul>
<li><strong>C ++ program to print the address of x and the value assigned to x</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, *p;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>p = &amp;x;</p>
<p>cout&lt;&lt;"The address of the variable x = "&lt;&lt; p;</p>
<p>cout&lt;&lt;"The value of the variable x = "&lt;&lt; *p;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 1</p>
<p>The address of the variable x = 0x7fffc60478a4</p>
<p>The value of the variable x = 1</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>The value of the variable x = 1 because you have assigned the value 1 to the variable x by entering 1 through the keyboard.</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>cout&lt;&lt;"The address of the variable x = "&lt;&lt; p;</p>
<p>cout&lt;&lt;"The value of the variable x = "&lt;&lt; *p;</p>
<p>are replaced by the statement:</p>
<p>cout&lt;&lt;"The address of the variable x = "&lt;&lt; p &lt;&lt;"its value = "&lt;&lt; *p;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, *p;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin &gt;&gt; x;</p>
<p>p = &amp;x;</p>
<p>cout&lt;&lt;"The address of the variable x = "&lt;&lt; p &lt;&lt;"its value = "&lt;&lt; *p;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>The address of the variable x = 0x7fff78508cc4 its value = 2</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y, *p, *q, sum;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin &gt;&gt; x;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin &gt;&gt; y;</p>
<p>p = &amp;x;</p>
<p>q = &amp;y;</p>
<p>sum = *p + *q;</p>
<p>cout&lt;&lt;"\n sum of entered numbers =&nbsp; "&lt;&lt; sum;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 4</p>
<p>Enter any number:</p>
<p>If you enter the number 3</p>
<p>sum of entered numbers = 7</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Since *p imply the value assigned to the variable x (i.e., 4) by entering 4 through the keyboard</p>
<p>and *q imply the value assigned to the variable y (i.e., 3) by entering 3 through the keyboard. Therefore:</p>
<p>sum = *p + *q = 4 + 3 = 7 (which is outputted on the screen).</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the product, subtraction and division of two numbers using pointers</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y, *p, *q, product, subtract, div;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt; x;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt; y;</p>
<p>p = &amp;x;</p>
<p>q = &amp;y;</p>
<p>product = *p * *q;</p>
<p>subtract = *p - *q;</p>
<p>div= *p / *q;</p>
<p>cout&lt;&lt;"\n product of entered numbers =&nbsp; "&lt;&lt; product;</p>
<p>cout&lt;&lt;"\n subtract of entered numbers =&nbsp; "&lt;&lt; subtract;</p>
<p>cout&lt;&lt;"\n division of entered numbers =&nbsp; "&lt;&lt; div;</p>
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
<p>will be displayed on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to find the greatest of two numbers using pointers</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y, *p, *q;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt; x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt; y;</p>
<p>p = &amp;x;</p>
<p>q = &amp;y;</p>
<p>if(*p&gt;*q)</p>
<p>{</p>
<p>cout&lt;&lt;"x is greater than y";</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>cout&lt;&lt;"y is greater than x";</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 10</p>
<p>Enter any integer:</p>
<p>If you enter the integer 16</p>
<p>y is greater than x</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the output of the following programs:</strong></li>
</ul>
<p>A)</p>
<p>&nbsp;</p>
<p>#include &lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x;</p>
<p>x=12;</p>
<p>cout&lt;&lt;"per = "&lt;&lt; x;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>per=12</p>
<p>B)</p>
<p>&nbsp;</p>
<p>#include &lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, t, c;</p>
<p>x=12;</p>
<p>t=2;</p>
<p>c = x/t;</p>
<p>cout&lt;&lt;"velocity =&nbsp; "&lt;&lt; c &lt;&lt;"m/s";</p>
<p>return 0;</p>
<p>}</p>
<p><strong>Answer:</strong></p>
<p>velocity = 6 m/s</p>
<p><strong>Program 7.4</strong></p>
<ul>
<li><strong>C++ program to print the sum of two numbers using functions</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int addition();</p>
<p>int main()</p>
<p>{&nbsp;&nbsp;</p>
<p>int answer;</p>
<p>answer = addition();</p>
<p>cout&lt;&lt;"The sum of two numbers is: "&lt;&lt;answer;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>int addition()</p>
<p>{</p>
<p>int x, y;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;y;</p>
<p>return x+y;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Enter any integer:</p>
<p>If you enter the integer 3</p>
<p>Enter any integer:</p>
<p>If you enter the integer 5</p>
<p>sum of two numbers = 8</p>
<p>will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>int addition(); // the statement implies function declaration</p>
<p>&nbsp;</p>
<p>int means integer and int addition() implies: addition() should return integer value.</p>
<p>&nbsp;</p>
<p>int addition()// implies: the function to add the entered values (i.e., 3 and 5) and return the result (i.e., 3 + 5 i.e., 8) to the statement:</p>
<p>cout&lt;&lt;"The sum of two numbers is: "&lt;&lt;answer; to</p>
<p>make provision to display the output:</p>
<p>sum of two numbers = 8</p>
<p>{</p>
<p>int x, y;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;y;</p>
<p>return x+y;</p>
<p>}// implies: the body of the function int addition()</p>
<p>&nbsp;</p>
<p>answer = addition(); // implies: the function call i.e., calls the function:</p>
<p>addition()</p>
<p>to add the entered values (i.e., 3 and 5) and return the result (i.e., 3 + 5 i.e., 8)</p>
<p>to the statement:</p>
<p>cout&lt;&lt;"The sum of two numbers is: "&lt;&lt;answer;</p>
<p>to make provision to display the output:</p>
<p>sum of two numbers = 8</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the product of two numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int multiplication();</p>
<p>int main()</p>
<p>{&nbsp;&nbsp;</p>
<p>int answer;</p>
<p>answer = multiplication();</p>
<p>cout&lt;&lt;"The product of two numbers is: "&lt;&lt;answer;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>int multiplication()</p>
<p>{</p>
<p>int x, y;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;y;</p>
<p>return x*y;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter the integer 3</p>
<p>Enter any integer:</p>
<p>If you enter the integer 5</p>
<p>product of two numbers = 15</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the greatest of two numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int largest();</p>
<p>int main()</p>
<p>{&nbsp;&nbsp;</p>
<p>int answer;</p>
<p>answer = largest();</p>
<p>cout&lt;&lt;"The largest of two numbers is: "&lt;&lt;answer;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>int largest()</p>
<p>{</p>
<p>int x, y;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;y;</p>
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
<p>largest of two numbers= 5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the greatest of three numbers using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int largest();</p>
<p>int main()</p>
<p>{</p>
<p>int answer;</p>
<p>answer = largest();&nbsp;</p>
<p>cout&lt;&lt;"largest of three numbers= "&lt;&lt; answer;</p>
<p>return 0;</p>
<p>}</p>
<p>int largest()</p>
<p>{</p>
<p>int x, y, z;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;y;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;z;</p>
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
<p>largest of three numbers = 10</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the square of the number using functions</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int square(;</p>
<p>int main()</p>
<p>{</p>
<p>int answer;</p>
<p>answer = square();&nbsp;</p>
<p>cout&lt;&lt;"square of the given number = "&lt;&lt; answer;</p>
<p>return 0;</p>
<p>}</p>
<p>int square()</p>
<p>{</p>
<p>int x;</p>
<p>cout&lt;&lt;"Enter any integer:";</p>
<p>cin&gt;&gt;x;</p>
<p>return x*x;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any integer:</p>
<p>If you enter an integer 5</p>
<p>square of the number = 25</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x;</p>
<p>x=6;</p>
<p>cout&lt;&lt;"The address of x = "&lt;&lt;&amp;x;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>The address of x = 0x7ffd80d2c06c</p>
<p><strong>Program 7.5</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Switch (case)</strong> allows to make decision from the number of choices i.e., from the number of cases</p>
<p>&nbsp;</p>
<p><strong>For example:</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
<p>cin&gt;&gt;ch;</p>
<p>switch(ch)</p>
<p>{</p>
<p>case 'R':</p>
<p>cout&lt;&lt;"Red";</p>
<p>break;</p>
<p>case 'W':</p>
<p>cout&lt;&lt;"White";</p>
<p>break;</p>
<p>case 'Y':</p>
<p>cout&lt;&lt;"Yellow";</p>
<p>break;</p>
<p>case 'G':</p>
<p>cout&lt;&lt;"Green";</p>
<p>break;</p>
<p>default:</p>
<p>cout&lt;&lt;"Error";</p>
<p>break;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any character:</p>
<p>If you enter a character R</p>
<p>Red</p>
<p>will be outputted on the screen.</p>
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
<p>cout&lt;&lt;"Red";</p>
<p>is executed to display the output:</p>
<p>Red</p>
<p>on the screen.</p>
<p>Suppose you enter a character K</p>
<p>Then the output on the screen is:</p>
<p>Error</p>
<p>&nbsp;</p>
<p>(Entered character K does not correspond to any of the cases:</p>
<p>case 'R':</p>
<p>case 'W':</p>
<p>case 'Y':</p>
<p>case 'G':</p>
<p>Therefore the statement:</p>
<p>cout&lt;&lt;"Error";</p>
<p>is executed to display the output:</p>
<p>Error</p>
<p>on the console screen).</p>
<p>If the statements:</p>
<p>&nbsp;</p>
<p>case 'R':</p>
<p>cout&lt;&lt;"Red";</p>
<p>break;</p>
<p>case 'W':</p>
<p>cout&lt;&lt;"White";</p>
<p>break;</p>
<p>case 'Y':</p>
<p>cout&lt;&lt;"Yellow";</p>
<p>break;</p>
<p>case 'G':</p>
<p>cout&lt;&lt;"Green";</p>
<p>break;</p>
<p>default:</p>
<p>cout&lt;&lt;"Error";</p>
<p>break;</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>case 'R':</p>
<p>cout&lt;&lt;"Red";</p>
<p>case 'W':</p>
<p>cout&lt;&lt;"White";</p>
<p>case 'Y':</p>
<p>cout&lt;&lt;"Yellow";</p>
<p>break;</p>
<p>case 'G':</p>
<p>cout&lt;&lt;"Green";</p>
<p>break;</p>
<p>default:</p>
<p>cout&lt;&lt;"Error";</p>
<p>break;</p>
<p>&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>Red</p>
<p>White</p>
<p>Yellow</p>
<p>i.e., the output will be printed till yellow even though you have entered the character R.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 7.6</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to print the output:</strong></p>
<p>&nbsp;</p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>&nbsp;</p>
<p><strong>using arrays: </strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>main()</p>
<p>{</p>
<p>int i;</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl;</p>
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
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl;</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=0) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[0] i.e., 16).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=1</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [1] = 18</p>
<p>using the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl;</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=1) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[1] i.e., 18).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [2] = 20</p>
<p>using the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl;</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=2) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[2] i.e., 20).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [3] = 25</p>
<p>using the statement:&nbsp;</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl;</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=3) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[3] i.e., 25).</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [4] = 36</p>
<p>using the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl;</p>
<p>Stop because the condition i&lt;5 is achieved.</p>
<p>format string %d in the square brackets indicates that the value to be displayed at that point in the string i.e., with the square brackets [ ] needs to be taken from a variable (which is i i.e., i=4) and the format string %d after the statement (\n Element [%d] = ) indicates that the value to be displayed at that point in the string i.e., after the statement (\n Element [%d] = ) needs to be taken from a variable (which is stored in num[i] i.e., num[4] i.e., 36).</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl; is replaced by the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[0] &lt;&lt; endl;</p>
<p>Then the <strong>output on the screen</strong>:</p>
<p>Element [0] = 16</p>
<p>Element [1] = 16</p>
<p>Element [2] = 16</p>
<p>Element [3] = 16</p>
<p>Element [4] = 16</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl; is replaced by the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[1] &lt;&lt; endl;</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 18</p>
<p>Element [1] = 18</p>
<p>Element [2] = 18</p>
<p>Element [3] = 18</p>
<p>Element [4] = 18</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl; is replaced by the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[2] &lt;&lt; endl;</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 20</p>
<p>Element [1] = 20</p>
<p>Element [2] = 20</p>
<p>Element [3] = 20</p>
<p>Element [4] = 20</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl; is replaced by the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[3] &lt;&lt; endl;</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 25</p>
<p>Element [1] = 25</p>
<p>Element [2] = 25</p>
<p>Element [3] = 25</p>
<p>Element [4] = 25</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[i] &lt;&lt; endl; is replaced by the statement:</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt;&nbsp; num[4] &lt;&lt; endl;</p>
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
<p>int num [i] = {16, 18, 20, 25, 36};</p>
<p>Then the compilation will be displayed on the screen because there are 5 elements within the braces {} not i elements.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>C++ program to print the sum of the elements in array.</strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i, sum = 0;</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>sum = sum + num[i];</p>
<p>cout&lt;&lt;"Sum of the Elements in the array = "&lt;&lt; sum;</p>
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
<p>cout&lt;&lt;"Sum of the Elements in the array&nbsp; = "&lt;&lt; sum; is executed to display the output:</p>
<p>Sum of the Elements in the array = 115</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int i, sum = 0;</p>
<p>is replaced by int i, sum = 1;</p>
<p>Then The output on the screen:</p>
<p>Sum of the Elements in the array = 116</p>
<p>&nbsp;</p>
<ul>
<li><strong>C++ program to print the average of the elements in array </strong></li>
</ul>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i, avg, sum = 0;</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>sum = sum + num [i];</p>
<p>avg = sum/5;</p>
<p>cout&lt;&lt;"Sum of the Elements in the array = "&lt;&lt; sum;</p>
<p>cout&lt;&lt;"average of the elements in the array= "&lt;&lt; avg;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Sum of the Elements in the array = 115</p>
<p>average of the elements in the array = 23</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print: </strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>Einstein [0] = E</p>
<p>Einstein [1] = I</p>
<p>Einstein [2] = N</p>
<p>Einstein [3] = S</p>
<p>Einstein [4] = T</p>
<p>Einstein [5] = E</p>
<p>Einstein [6] = I</p>
<p>Einstein [7] = N</p>
<p><strong>using arrays</strong></p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>char name [8] = {'E' , 'I', 'N', 'S', 'T', 'E', 'I', 'N'};</p>
<p>for(i=0; i&lt;8; i++)</p>
<p>cout&lt;&lt;"Element ["&lt;&lt; i &lt;&lt;" ] = "&lt;&lt; name[i] &lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following programs?</strong></li>
</ul>
<p>i)</p>
<p>#include &lt;iostream&gt;</p>
<p>#include &lt;math.h&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>cout&lt;&lt;""&lt;&lt; cbrt(27);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>3</p>
<p>ii)</p>
<p>#include &lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char i;&nbsp;</p>
<p>char body [4] = {'b', 'o', 'd', 'y'};</p>
<p>for(i=0; i&lt;4; i++)</p>
<p>cout&lt;&lt;"\n body ["&lt;&lt;body[i] &lt;&lt;" ] = "&lt;&lt; body[i] &lt;&lt; endl;</p>
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
<p>&nbsp;</p>
<p>iii)</p>
<p>&nbsp;</p>
<p>#include &lt;iostream&gt;</p>
<p>#include &lt;malloc.h&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x=2;&nbsp;</p>
<p>cout&lt;&lt;""&lt;&lt; malloc (200*sizeof(x));</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>8183824</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 7.7</strong></p>
<p><strong>C++ program to print the output:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Name of the book = B</p>
<p>Price of the book = 135.00</p>
<p>Number of pages = 300</p>
<p>Edition = 8</p>
<p>&nbsp;</p>
<p><strong>using structures </strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>struct book {</p>
<p>char name;</p>
<p>float price;</p>
<p>int pages;</p>
<p>int edition;</p>
<p>};</p>
<p>struct book b1= {'B', 135.00, 300, 8};</p>
<p>cout&lt;&lt;"Name of the book =&nbsp; "&lt;&lt; b1.name&lt;&lt; endl;</p>
<p>cout&lt;&lt;"Price of the book = "&lt;&lt; b1.price&lt;&lt;endl;</p>
<p>cout&lt;&lt;"Number of pages = "&lt;&lt; b1.pages&lt;&lt;endl;</p>
<p>cout&lt;&lt;"Edition of the book = "&lt;&lt; b1.edition&lt;&lt; endl;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
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
<p>For example: name is the element which must be linked with structure variable b1 with dot operator to assign a value B to the element "name".</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>cout&lt;&lt;"Name of the book =&nbsp; "&lt;&lt; b1.name&lt;&lt; endl;</p>
<p>is executed to print the output:</p>
<p>Name of the book = B</p>
<p>on the screen.</p>
<p>The statement:</p>
<p>cout&lt;&lt;"Price of the book = "&lt;&lt; b1.price&lt;&lt;endl;</p>
<p>is executed to print the output:</p>
<p>Price of the book = 135.00</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>cout&lt;&lt;"Number of pages = "&lt;&lt; b1.pages&lt;&lt;endl;</p>
<p>is executed to print the output:</p>
<p>Number of pages = 300</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>cout&lt;&lt;"Edition of the book = "&lt;&lt; b1.edition&lt;&lt; endl;</p>
<p>is executed to print the output:</p>
<p>Edition of the book = 8</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be output of the following programs?</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>A)</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>struct book {</p>
<p>char name;</p>
<p>float price;</p>
<p>int pages;</p>
<p>int edition;</p>
<p>};</p>
<p>int main()</p>
<p>{</p>
<p>struct book b1;</p>
<p>b1.name = 'C';</p>
<p>b1.price = 135.00;</p>
<p>b1.pages = 300;</p>
<p>b1.edition = 8;</p>
<p>cout&lt;&lt;"Name of the book = bulgarian "&lt;&lt;&nbsp; b1.name &lt;&lt; endl;</p>
<p>cout&lt;&lt;"\n Price of the book = "&lt;&lt; b1.price;</p>
<p>cout&lt;&lt;"\n Number of pages = "&lt;&lt; b1.pages&lt;&lt;endl;</p>
<p>cout&lt;&lt;"\n Edition of the book = "&lt;&lt; b1.edition;</p>
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
<p>#include &lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>&nbsp;</p>
<p>for( ; ; ) {</p>
<p>cout&lt;&lt;"This loop will run forever.\n";</p>
<p>}</p>
<p>&nbsp;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever.</p>
<p>This loop will run forever. ......... continues</p>
<p>&nbsp;</p>
<p><strong>Program 7.8</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Continue and break statements: </strong></p>
<p>&nbsp;</p>
<ol>
<li>i)</li>
</ol>
<p>&nbsp;</p>
<p>#include &lt;iostream&gt;</p>
<p>using namespace std;</p>
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
<p>cout&lt;&lt;"\n "&lt;&lt; i;</p>
<p>}</p>
<p>return 0;</p>
<p>&nbsp;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>1</p>
<p>2</p>
<p>4</p>
<p>5</p>
<p>&nbsp;</p>
<ol>
<li>ii)</li>
</ol>
<p>&nbsp;</p>
<p>#include &lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i;</p>
<p>for (i=1; i&lt;=5; i++)</p>
<p>{</p>
<p>if (i==3)</p>
<p>{</p>
<p>break;</p>
<p>}</p>
<p>cout&lt;&lt;"\n "&lt;&lt; i;</p>
<p>}</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Output on the screen:</p>
<p>&nbsp;</p>
<p>1</p>
<p>2</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 7.9</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>C++ program to convert the upper case letter to lower case letter</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'A';</p>
<p>char b = tolower(ch);</p>
<p>cout&lt;&lt;" upper case letter "&lt;&lt; ch &lt;&lt;" is converted to lower case letter "&lt;&lt; b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>upper case letter A is converted to lower case letter a</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to enter the character through the keyboard, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
<p>cin&gt;&gt;ch;</p>
<p>char b = tolower(ch);</p>
<p>cout&lt;&lt;" upper case letter "&lt;&lt; ch &lt;&lt;" is converted to lower case letter "&lt;&lt; b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Enter any character:</p>
<p>If you enter the character C</p>
<p>upper case letter C is converted to lower case letter c will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 8.0</strong></p>
<p><strong>C++ program to convert the lower case letter to upper case letter</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'a';</p>
<p>char b = toupper(ch);</p>
<p>cout&lt;&lt;" lower case letter "&lt;&lt;ch&lt;&lt;" is converted to upper case letter "&lt;&lt;b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>Output on the screen:</p>
<p>lower case letter a is converted to upper case letter A</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to enter the character through the keyboard, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch;</p>
<p>cout&lt;&lt;"Enter any character:";</p>
<p>cin&gt;&gt;ch;</p>
<p>char b = toupper(ch);</p>
<p>cout&lt;&lt;" lower case letter "&lt;&lt;ch&lt;&lt;" is converted to upper case letter "&lt;&lt;b;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Enter any character:</p>
<p>If you enter the character h</p>
<p>lower case letter h is converted to upper case letter H</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 8.1</strong></p>
<p><strong>C++ program to test whether the entered character is upper case letter or not</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'a';</p>
<p>if(isupper(ch))</p>
<p>cout&lt;&lt;"you have entered the upper case letter";</p>
<p>else</p>
<p>cout&lt;&lt;"you have entered the lower case letter";</p>
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
<p><strong>Program 8.2</strong></p>
<p><strong>C++ program to test whether the entered character is lower case letter or not</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch = 'a';</p>
<p>if(islower(ch))</p>
<p>cout&lt;&lt;"you have entered the lower case letter";</p>
<p>else</p>
<p>cout&lt;&lt;"you have entered the upper case letter";</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>you have entered the lower case letter</p>
<p><strong>Program 8.3</strong></p>
<p><strong>C++ program to print the value of tan inverse x (i.e., the value of tan<sup>-1</sup> x)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x = 20;</p>
<p>cout&lt;&lt;"the value of tan inverse x = "&lt;&lt; atan(x);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the value of tan inverse x = 1.520838</p>
<p><strong>Program 8.4</strong></p>
<p><strong>C++ program to print the value of tan inverse x/y (i.e., the value of tan<sup>-1</sup>x/y)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x,y;</p>
<p>x = 20;</p>
<p>y =20;</p>
<p>cout&lt;&lt;"the value of tan inverse x/y = "&lt;&lt; atan2(x,y);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the value of tan inverse x/y = 0.785398</p>
<p>&nbsp;</p>
<p><strong>Program 8.5</strong></p>
<p><strong>C++ program to print the value of fmod(x, y)</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;math.h&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>float x = 20.500000;</p>
<p>float y =20.799999;</p>
<p>cout&lt;&lt;" the remainder of "&lt;&lt;x &lt;&lt;" divided by "&lt;&lt;y &lt;&lt;" is: "&lt;&lt; fmod(x,y);</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>the remainder of 20.500000 divided by 20.799999 is 20.500000</p>
<p><strong>Program 8.6</strong></p>
<p><strong>C++ program to print the value of ~x</strong></p>
<p><strong>&nbsp;</strong></p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int x, y;</p>
<p>x = 205;</p>
<p>y=~x;</p>
<p>cout&lt;&lt;"the value of y is: "&lt;&lt; y;</p>
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
<p>the value of y is:206</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following programs:</strong></li>
</ul>
<p>i)</p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i = 54;</p>
<p>int y = i&lt;&lt;1;</p>
<p>cout&lt;&lt;"The value of y = "&lt;&lt; y;</p>
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
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>i&lt;&lt;1 implies 54 * 2 = 108</p>
<p>i&lt;&lt;2 implies 54 * 4 = 216</p>
<p>i&lt;&lt;3 implies 54 * 6 = 324</p>
<p>i&lt;&lt;4 implies 54 * 8 = 432</p>
<p>&nbsp;</p>
<p>ii)</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i = 54;</p>
<p>int y = i&gt;&gt;1;</p>
<p>cout&lt;&lt;"The value of y = "&lt;&lt; y;</p>
<p>return 0;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>The value of y = 27</p>
<p>If the statement:</p>
<p>i&gt;&gt;1 is replaced by the statement: i&gt;&gt;2</p>
<p>Then the output on the screen is:</p>
<p>The value of y = 13</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>i&gt;&gt;1 implies 54 / 2 = 27</p>
<p>i&gt;&gt;2 implies 54 / 4 = 13</p>
<p>i&gt;&gt;3 implies 54 / 6 = 9</p>
<p>i&gt;&gt;4 implies 54 / 8 = 6</p>
<p>&lt;&lt; implies: left shift operator</p>
<p>&gt;&gt; implies: right shift operator</p>
<p>&nbsp;</p>
<p><strong>Program 8.7</strong></p>
<p><strong>C++ program to print the length of the entered character (i.e., to print the length of the string)</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>#include&lt;string.h&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>char ch[4];</p>
<p>cout&lt;&lt;"Enter any word: ";</p>
<p>cin&gt;&gt;ch;</p>
<p>cout&lt;&lt;"The length of the string = "&lt;&lt; strlen(ch);</p>
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
<p><strong>&nbsp;</strong></p>
<p><strong>Program 8.8</strong></p>
<p><strong>C++ program to print the factorial of the entered number</strong></p>
<p>&nbsp;</p>
<p>#include&lt;iostream&gt;</p>
<p>using namespace std;</p>
<p>int main()</p>
<p>{</p>
<p>int i, n, fact=1 ;</p>
<p>cout&lt;&lt;"Enter any number:";</p>
<p>cin&gt;&gt;n;</p>
<p>for(i=1; i&lt;=n; i++)</p>
<p>fact = fact *i;</p>
<p>cout&lt;&lt;"\n Entered number is: "&lt;&lt; n;</p>
<p>cout&lt;&lt;"\n The factorial of the entered number"&lt;&lt;n&lt;&lt;"is:"&lt;&lt; fact;</p>
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
<p>&nbsp;</p>
 
</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>The C++ Programming Language </xmp></center></td>
                <td><center><xmp>Brian W. Kernighan</xmp></center></td>
                <td><a href="img/pdf23.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>C++: The Complete Reference</xmp></center></td>
                <td><center><xmp>Herbert Schildt</xmp></center></td>
                <td><a href="img/pdf24.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Thinking in C++ </xmp></center></td>
                <td><center><xmp>Bruce Eckel </xmp></center></td>
                <td><a href="img/pdf25.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Object-Oriented Programming in C++</xmp></center></td>
                <td><center><xmp>Robert Lafore</xmp></center></td>
                <td><a href="img/pdf26.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C++: A Beginner's Guide</xmp></center></td>
                <td><center><xmp>Herbert Schildt</xmp></center></td>
                <td><a href="img/pdf27.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C++ Primer</xmp></center></td>
                <td><center><xmp> Stanley B. Lippman</xmp></center></td>
                <td><a href="img/pdf28.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Essential C++</xmp></center></td>
                <td><center><xmp>Stanley B. Lippman</xmp></center></td>
                <td><a href="img/pdf29.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp> C++ For Dummies</xmp></center></td>
                <td><center><xmp> Stephen Randy Davis</xmp></center></td>
                <td><a href="img/pdf30.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>C++ Without Fear</xmp></center></td>
                <td><center><xmp>Brian Overland</xmp></center></td>
                <td><a href="img/pdf31.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>Learn C++ Programming Language</xmp></center></td>
                <td><center><xmp>TutorialsPoint</xmp></center></td>
                <td><a href="img/pdf32.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Accelerated C++</xmp></center></td>
                <td><center><xmp>Andrew Koenig</xmp></center></td>
                <td><a href="img/pdf33.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>



</br>



</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>



<div id="code39" style ="font-family: Georgia, Serif;">
<center> <h3>  <font color="black" size="6" face="calibri"> Java Programming </font>            </h3> </center>
 </br>
 
 <ul>
<li>Java is a high level programming language conceived by James Gosling</li>
</ul>

</br>
<center> <img src="images/d3.jpg" alt="Smiley face" height="240" width="320"> </center>
</br>
<p>, Patrick Naughton, Chris Warth, Ed Frank, and Mike Sheridan at Sun Microsystems, Inc. in 1991 to create programs to control consumer electronics (which is now a subsidiary of Oracle Corporation) and released in 1995, used in internet programming, mobile devices, games, e-business solutions etc.,&nbsp; because of its reliability, high performance, simplicity and easy to use and quick to learn and rigid versus extensibility.</p>
<p>&nbsp;</p>
<p><strong>Process of Java program execution: A Java program:</strong>&nbsp;</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>is written using Text Editor , such as [ Notepad++, Notepad ] and saved with [.java] Extension.</p>
<p>&nbsp;</p>
<ul>
<li>File Saved with [.java] extension is called Source Program or Source Code.</li>
</ul>
<p>&nbsp;</p>
<p>// --- HelloWorld.java------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>-------(because the class name is HelloWorld the source file should be named as HelloWorld.java)---------------//</p>
<p>&nbsp;</p>
<p>and sent to the java compiler (i.e., javac compiler) where the source program is compiled (i.e., the program is entirely read and translated into Java byte codes (but not into machine language)).</p>
<p>&nbsp;</p>
<ul>
<li>If the javac compiler finds any error during compilation, it provides information about the error to the programmer. The programmer has to review code and check for the solution.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>And if there are no errors the translated program (i.e., java byte codes -- a highly optimized set of instructions) is stored in computers main memory as HelloWorld.class and since the java byte codes cannot be trusted to be correct. Therefore before execution they are verified and converted to machine level language i.e., machine code sequence of 0s and 1s by Java run-time system, which is called the Java Virtual Machine (JVM) and is executed by a Java interpreter and</li>
</ul>
<p>Hello, World!</p>
<p>is displayed on the console screen.&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
<li>JVM (Java Virtual Machine) resides under &rarr;</li>
<li><strong>RAM (Random Access Memory</strong> &ndash; the stuff that boost up your computer to run faster and allows your computer to perform many tasks at the same time)</li>
</ul>
<p>and JVM comprises:</p>
<ul>
<li><strong>Class Loader:</strong> it loads .class file that contains Java byte codes.</li>
<li><strong>Byte Code Verifier:</strong> it verifies byte codes.</li>
<li><strong>Execution Engine:</strong> it translates java byte codes to machine codes and executes them.</li>
</ul>
<p>&nbsp;</p>
<p>In the statement:</p>
<p>public class HelloWorld</p>
<p>&nbsp;</p>
<p>The word "HelloWorld" implies: name of the class is HelloWorld and this class is public.</p>
<p>public means that the class HelloWorld can be accessed by any other class in any package.</p>
<p>In the program:</p>
<p>&nbsp;</p>
<p>//------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>&nbsp;</p>
<p>} // imply the body of the class HelloWorld (Here: the curly brace '{' imply the beginning of the class and the curly brace '}' imply the end of the class) within which the</p>
<p>main method</p>
<p>&nbsp;</p>
<p>public static void main(String [] args) {</p>
<p>&nbsp;</p>
<p>} is written.</p>
<p>&nbsp;</p>
<p>public static void main(String [] args) imply: main method (a collection of statements or methods like System.out.println( ) that are grouped together to perform an operation)</p>
<p>and this main method is public</p>
<p>and</p>
<p>{</p>
<p>&nbsp;</p>
<p>} imply the body of the main method</p>
<p>(Here: the curly brace '{' imply the beginning of the main method and the curly brace '}' imply the end of the main method) within which the statement:</p>
<p>&nbsp;</p>
<p>System.out.println("Hello, World!");</p>
<p>&nbsp;</p>
<p>is written and executed.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> main method in java functions like main function main () in C and C++.</li>
</ul>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>public class HelloWorld is replaced by the statement:</p>
<p>public class sample i.e.,</p>
<p>public class sample {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the error will be displayed on the screen because the program written in notepad is saved as HelloWorld.java not as sample.java.</p>
<p>If we want to write the statement:</p>
<p>public class sample instead of the statement:</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public class HelloWorld, then we have to save the program written in notepad as sample.java but not as HelloWorld.java.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Like C &amp; C++, Java is also a case sensitive language i.e., capital letters (or upper case letters) must be avoided to prevent the display of error on the screen</p>
<p><strong>For example:</strong> If the statement:</p>
<p>PUBLIC static void main(String [] args) is written instead of the statement:</p>
<p>public static void main(String [] args), compilation Error will be displayed on the screen.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If we forget to end each program statement within the body of main method with a semicolon (";"), Error will be displayed on the screen</p>
<p>&nbsp;</p>
<p>public static void main(String [] args) &rarr;&nbsp; The program begins its execution with the method:</p>
<p>public static void main (String [] args)- the main method&nbsp; -- the entry point of the program execution</p>
<p>i.e., the point from where the execution of Java program begins.</p>
<p>&nbsp;</p>
<p><strong>Semicolon: </strong>program is a set of instructions and each instruction (or each statement) is ended by a semicolon. Like in an English paragraph each sentence is ended by a full stop which tells that one sentence ends and another begins, semicolon implies that one instruction (or statement) ends and another begins.</p>
<p>&nbsp;</p>
<p>In the statement:</p>
<p>System.out.println();</p>
<p>&nbsp;</p>
<ul>
<li><strong>System</strong> &rarr; name of a standard class that contains variables and methods for supporting simple keyboard and character output to the display.</li>
</ul>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>out</strong> &rarr; represents the standard output stream &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</li>
</ul>
<p>&nbsp;</p>
<ul>
<li><strong>println()</strong> &rarr; output method of the Java language which makes provision to print the output in the next line:</li>
</ul>
<p>&nbsp;</p>
<p>Hello,world!</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>on the screen.</p>
<p>The text</p>
<p>Hello,world!</p>
<p>should be enclosed by the <strong>double quotation marks</strong> ("") and should be written within the println method and this</p>
<p>println method should be ended with the semicolon i.e.,</p>
<p>System.out.println("Hello,world!");</p>
<p>otherwise the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p>//---------------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println("Hello, World!");</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>&nbsp;</p>
<p>Hello, World!</p>
<p>Hello, World!</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.print("Hello, World!");</p>
<p>System.out.print("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>Hello, World!Hello, World!</p>
<p>&nbsp;</p>
<p>---------------------------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>In the statement:</p>
<p>public static void main(String [] args)</p>
<p>&nbsp;</p>
<p>public &rarr; implies: this method can accessed from anywhere outside the class HelloWorld</p>
<p>If the word "public" in the statement:</p>
<p>public static void main(String [] args)</p>
<p>is replaced by the word</p>
<p><strong>private</strong></p>
<p>or</p>
<p><strong>protected</strong></p>
<p>&nbsp;</p>
<p>Then compilation error will be flagged on the screen because if the method is declared private or protected then this method does not make itself available to JVM for execution.</p>
<p>&nbsp;</p>
<p><strong>main</strong> &rarr; implies the name of the method</p>
<p>&nbsp;</p>
<p><strong>static</strong> means the main method is the part of the class HelloWorld</p>
<p>&nbsp;</p>
<ul>
<li><strong>Why static ? </strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>Because the program execution begins from the main method and if the main method is not declared static then the execution of the program does not take place.</p>
<p>&nbsp;</p>
<p>void &rarr; implies the main method does not return any value i.e., main method return nothing when it completes execution.</p>
<p>&nbsp;</p>
<p>String args[]&rarr; While running the program if we want to pass something to the main method, then this parameter is used as the way of taking input from the user--so we can pass some strings while running the program if we want.</p>
<p>&nbsp;</p>
<p>Moreover, JVM cannot recognize the method:</p>
<p>public static void main(String [] args)</p>
<p>as method if the parameter String [] args is not included.</p>
<p>&nbsp;</p>
<p>If the word args in the statement:</p>
<p>public static void main(String [] args) is replaced by another word say jamesgosling or java</p>
<p>i.e.,</p>
<p>//----------------------------------------------------------------------------------------------------------------------</p>
<p>public class HelloWorld</p>
<p>{</p>
<p>public static void main(String [] jamesgosling)</p>
<p>{</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] java) {</p>
<p>System.out.println("Hello, World!");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>----------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>No compilation error will be displayed on the screen i.e., Hello, World! will be outputted on the screen without display of any error on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>public static void main(String [] args)</p>
<p>is replaced by the statement public static void main(String []) -- Then the error is displayed on the screen.</p>
<p>&nbsp;</p>
<p>Note: Most Java programmers prefer args and argv i.e., the statements:</p>
<p>public static void main(String [] args)</p>
<p>and public static void main(String [] argv) are preferred.</p>
<p>&nbsp;</p>
<p>If the space is left between the words Hello and World i.e., if the statement:</p>
<p>public class Hello World is written instead of the statement:</p>
<p>public class HelloWorld. Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 1.1</strong></p>
<p><strong>Java program to print the word "hello Bill Gates" on screen</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>System.out.println("hello Bill Gates");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>hello Bill Gates</p>
<p>&nbsp;</p>
<p><strong>Program 1.2</strong></p>
<p><strong>Java program to print the word "****hello silicon city****" on screen</strong></p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println(" ****hello silicon city**** ");</p>
<p>}</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>****hello silicon city****</p>
<p>&nbsp;</p>
<p><strong>Program 1.3</strong></p>
<p><strong>Java program to print </strong></p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p><strong>on screen</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp; ***** ");</p>
<p>System.out.println("\n&nbsp; ***** ");</p>
<p>System.out.println("\n&nbsp; ***** ");</p>
<p>System.out.println("\n&nbsp; ***** ");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>*</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>*****</p>
<p>If new line \n is not included in the above program then the output on the screen is:</p>
<p>&nbsp;</p>
<p>*********************</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>Write a program to print the following outputs:</strong></li>
</ul>
<p>(a)</p>
<p>&nbsp;</p>
<p>*</p>
<p>****</p>
<p>**java**</p>
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
<p>Must have a main method!</p>
<p>java is done mostly in lowercase. Like C &amp; C++ it&rsquo;s also a case-sensitive language</p>
<p>&nbsp;</p>
<p><strong>Answers:</strong></p>
<p>&nbsp;</p>
<p>a)</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp;&nbsp; **java** ");</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****&nbsp;&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>b)</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****************&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * Hello World! *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");&nbsp;&nbsp;&nbsp;</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; * *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>System.out.println("\n&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ****************&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>c)</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>System.out.println("\n Braces come in pairs!");</p>
<p>System.out.println("\n Comments come in pairs!");</p>
<p>System.out.println("\n&nbsp; All statements end with a semicolon!");</p>
<p>System.out.println("\n&nbsp; Spaces are optional!");</p>
<p>System.out.println("\n Must have a main method!");</p>
<p>System.out.println("\n java is done mostly in lowercase. Like C &amp; C++ it's also a case-sensitive language");</p>
<p>}</p>
<p>}</p>
<p><strong>Program 1.4</strong></p>
<p><strong>Java program to find the area of the circle</strong></p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>int r, area;</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>System.out.println("The area of the circle = " + area);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>The area of the circle = 50</p>
<p>int means the integer data type.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> An integer is a whole number - no fractions, decimal parts, or funny stuff.</li>
</ul>
<p>&nbsp;</p>
<p>The statement:</p>
<p>int r, area; imply that we are creating the integer variables r , area.</p>
<p>Equal sign implies: storage operator.</p>
<p>&nbsp;</p>
<p>The statements:</p>
<p>r = 2;</p>
<p>area = 4 * 3.14 * r * r;</p>
<p>imply that we are storing the values to the created variables (i.e., we are storing the value 2 for r and 4 * 3.14 * r * r for area).</p>
<p>&nbsp;</p>
<p>Comma in the statement:</p>
<p>int r, area; imply:: variable separator.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If multiplication sign &amp;times; is used instead of multiplication operator * i.e.,</p>
<p>area = 4&nbsp; &times; 3.14 &times; r&nbsp; &times; r;</p>
<p>then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>In C language, the statement:</p>
<p>printf("The area of the circle = %d ",&nbsp; area);</p>
<p>make the provision to print the output on the screen.</p>
<p>&nbsp;</p>
<p>In C++ language, the statement</p>
<p>cout&lt;&lt;"The area of the circle = "&lt;&lt; area;</p>
<p>make the provision to print the output on the screen.</p>
<p>&nbsp;</p>
<p>whereas in the Java language, the statement:</p>
<p>&nbsp;</p>
<p>System.out.println("The area of the circle =&nbsp; " + area);</p>
<p>make the provision to print the output on the screen.</p>
<p>&nbsp;</p>
<p>In the statement:</p>
<p>System.out.println("The area of the circle =&nbsp; " +&nbsp; area);</p>
<p>There are two strings:</p>
<ul>
<li>The area of the circle =</li>
<li>area</li>
</ul>
<p>plus operator (+) functions as the concatenation operator (concatenation means connecting two statements to produce a single statement) &ndash; which (here) concatenates</p>
<p>the string:</p>
<p>"The area of the circle = "&nbsp; and the string:</p>
<p>"area (which is 4 * 3.14 * r * r (=50 since r = 2))" -- producing a String statement:</p>
<p>The area of the circle = 50</p>
<p>which will be displayed on the screen as the result.</p>
<p>&nbsp;</p>
<p>The area of the circle is = 50. 24 (for r = 2) but</p>
<p>The area of the circle = 50 is displayed on the screen because the data type int is used instead of data type float.</p>
<p>&nbsp;</p>
<p>If the data type float is used instead of int i.e., then the output on the screen is:</p>
<p>The area of the circle = 50.24</p>
<p>&nbsp;</p>
<p>If you write:</p>
<p>4 * 3.14 * r^2; instead of 4 * 3.14 * r * r;</p>
<p>Then error is displayed on the screen because like in other high level languages (such as C and C++) there is no operator for performing r ^ 2 operation so the statement:</p>
<p>4 * 3.14 * r^2; is invalid.</p>
<p>Even though if we write ARGS instead of args i.e., even though if we express args in capital letter, No error will be displayed on the screen.</p>
<p>public static void main(String [] ARGS) &rarr; no error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 1.5</strong></p>
<p>&nbsp;</p>
<p><strong>Java program to find the circumference of the circle</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>float r, circumference;</p>
<p>r = 2;</p>
<p>circumference = 3.14 * r * r;</p>
<p>System.out.println("The circumference of the circle = " + circumference);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>The circumference of the circle = 12.56</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following programs:</strong></li>
</ul>
<p>&nbsp;</p>
<p>a)</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>double l, b, area;</p>
<p>l=2;</p>
<p>b=2.5;</p>
<p>area = l*b;</p>
<p>System.out.println("The area of the rectangle = " + area);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>The area of the rectangle = 5.0</p>
<p>b)</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main (String [] args) {</p>
<p>int a, b, c;</p>
<p>a= 3;</p>
<p>b=3;</p>
<p>c=3;</p>
<p>if ((a + b&lt; c) || (b + c &lt; a) || (a==b &amp;&amp; b==c))</p>
<p>System.out.println(" the triangle is equilateral");</p>
<p>else</p>
<p>System.out.println(" the triangle is not possible");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>the triangle is equilateral</p>
<p><strong>Program 1.6</strong></p>
<p><strong>Java program to convert the temperature in Celsius to Fahrenheit</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>float C, F;</p>
<p>C=38.5;</p>
<p>F = 9*C/5 +32;</p>
<p>System.out.println("temperature in Fahrenheit= " +F);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>temperature in Fahrenheit= 101.3</p>
<p><strong>Program 1.7</strong></p>
<p><strong>Java program to find the sum of two numbers</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld</p>
<p>{</p>
<p>public static void main(String [] args)</p>
<p>{</p>
<p>int a, b, sum;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>sum = a + b;</p>
<p>System.out.println("the sum of a and b = " + sum);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the sum of a and b = 3</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then we have to rewrite the program as follows:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld</p>
<p>{</p>
<p>public static void main(String [] args) {</p>
<p>int a, b, sum;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any two Numbers: ");</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>sum = a + b;</p>
<p>System.out.println("the sum of a and b = " + sum);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two Numbers:</p>
<p>If you enter two numbers 2 and 3</p>
<p>the sum of a and b = 5</p>
<p>will be outputted on the screen</p>
<p>&nbsp;</p>
<p>//----------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>Scanner is a class found in java.util package. So to use Scanner class, we first need to include:</p>
<p>java.util package</p>
<p>in our program.</p>
<p>&nbsp;</p>
<p>import java.util.Scanner; // This will import just the Scanner class</p>
<p>import java.util.*; // This will import the entire java.util package</p>
<p>&nbsp;</p>
<p>------------------------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>&nbsp;</p>
<p>implies: declaring an object of the Scanner class "scan" to read the values entered for a and b through the key board.</p>
<p>&nbsp;</p>
<p>And the statements:</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>imply: scan is an object of Scanner class and nextInt() is a method of the object "scan" that allows the object "scan" to read only integer values from the keyboard.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>//----------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>Same as the method:</p>
<p>nextInt() that allows the object "scan" to read only integer values from the keyboard, methods that allows the object "scan" to read other data types from the keyboard are listed below:</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<table width="215">
<tbody>
<tr>
<td width="102">
<p><strong>Methods</strong></p>
</td>
<td width="113">
<p><strong>datatype</strong></p>
</td>
</tr>
<tr>
<td width="102">
<p>nextInt()</p>
</td>
<td width="113">
<p>Integer</p>
</td>
</tr>
<tr>
<td width="102">
<p>nextFloat()</p>
</td>
<td width="113">
<p>Float</p>
</td>
</tr>
<tr>
<td width="102">
<p>nextDouble()</p>
</td>
<td width="113">
<p>Double</p>
</td>
</tr>
<tr>
<td width="102">
<p>nextLong()</p>
</td>
<td width="113">
<p>Long</p>
</td>
</tr>
<tr>
<td width="102">
<p>nextShort()</p>
</td>
<td width="113">
<p>Short</p>
</td>
</tr>
<tr>
<td width="102">
<p>next()</p>
</td>
<td width="113">
<p>Single word</p>
</td>
</tr>
<tr>
<td width="102">
<p>nextLine()</p>
</td>
<td width="113">
<p>Line of Strings</p>
</td>
</tr>
<tr>
<td width="102">
<p>nextBoolean()</p>
</td>
<td width="113">
<p>Boolean</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>------------------------------------------------------------------------------------------------------------------------------------//</p>
<p><strong>Program 1.8</strong></p>
<ul>
<li><strong>Java program to find the square root of a number</strong></li>
</ul>
<p>&nbsp;</p>
<p>i)</p>
<p>&nbsp;</p>
<p>public class HelloWorld</p>
<p>{</p>
<p>public static void main(String [] args) {</p>
<p>float x;</p>
<p>x = 233;</p>
<p>System.out.println(" square root of a number = " + Math.sqrt(x));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>square root of a number = 15.264</p>
<p>&nbsp;</p>
<p>If you want to supply the value for x through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>int x;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any Number: ");</p>
<p>x = scan.nextFloat();</p>
<p>System.out.println(" square root of a number = " + Math.sqrt(x));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any Number:</p>
<p>If you enter the number 233&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>square root of a number = 15.264337522</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ol>
<li>ii)</li>
</ol>
<p>&nbsp;</p>
<p>public class HelloWorld</p>
<p>{</p>
<p>public static void main(String [] args) {</p>
<p>double x;</p>
<p>x = 233;</p>
<p>System.out.println(" square root of a number = " + Math.sqrt(x));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbnbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; square root of a number = 15.264337522473747&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to supply the value for x through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>double x;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any Number: ");</p>
<p>x = scan.nextDouble();</p>
<p>System.out.println(" square root of a number = " + Math.sqrt(x));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any Number:</p>
<p>If you enter the number 233&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>square root of a number = 15.264337522473747</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 1.9</strong></p>
<ul>
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) {</p>
<p>char c;</p>
<p>c = 'A';</p>
<p>System.out.println("ch= " + c);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>ch=A</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you want to supply the value for c through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String[] args) throws Exception {</p>
<p>char c;</p>
<p>System.out.print("Enter a character:");</p>
<p>c = (char)System.in.read();</p>
<p>System.out.println("ch= " + c);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter a character:</p>
<p>If you enter the character K</p>
<p>ch= K</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Note: Exception is a problem that arises during the execution of a program.</p>
<p>When an exception occurs, program abnormally terminates and disrupts -</p>
<p>throws Exception should be written after the statement public static void main(String[] args) so that the</p>
<p>exceptions are thrown to the operating system to handle and the program will be successfully executed and the output will be displayed on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.0</strong></p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>String m;</p>
<p>Scanner in = new Scanner(System.in);</p>
<p>System.out.print("Enter the word: ");</p>
<p>m = in.nextLine();</p>
<p>System.out.println(" the word you entered = " + m);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter the word:</p>
<p>If you enter the word dog</p>
<p>the word you entered = dog</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>//-------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>m = scan.nextLine();</p>
<p>is written instead of</p>
<p>m = in.nextLine();</p>
<p>Then we have to replace the statement:</p>
<p>Scanner in = new Scanner(System.in);</p>
<p>by the statement:</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>Otherwise compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the mistake in the following program:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld</p>
<p>{</p>
<p>static public void main(String args []) {</p>
<p>float x;</p>
<p>x = 233;</p>
<p>System.out.println(" cube root of a number = " + Math.cbrt(x));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>There is no mistake in the above program.</p>
<p>The statement:</p>
<p>public static void main(String[] args) can also be written as:</p>
<p>static public void main(String args [])</p>
<p><strong>The output on the screen is:</strong></p>
<p>cube root of a number = 6.1534494936636825</p>
<p>&nbsp;</p>
<p><strong>Program 2.1</strong></p>
<p><strong>Java program to find the product of two numbers.</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int a, b, product;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>product = a * b;</p>
<p>System.out.println("the product of a and b = " + product);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the sum of a and b = 2</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then we have to rewrite the above program as follows:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>int a, b, product;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any two Numbers: ");</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>product = a * b;</p>
<p>System.out.println("the product of a and b = " + product);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two Numbers:</p>
<p>If you enter two numbers 6 and 3</p>
<p>the product of a and b = 18</p>
<p>will be outputted on the screen</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>If you want to assign the floating point values for a &amp; b, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>float a, b, product;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any two Numbers: ");</p>
<p>a = scan.nextFloat();</p>
<p>b = scan.nextFloat();</p>
<p>product = a * b;</p>
<p>System.out.println("the product of a and b = " + product);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two Numbers:</p>
<p>If you enter two floating point values 2.9 and 3.6</p>
<p>the product of a and b = 10.44</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>float is used instead of int because a and b are assigned fractional values (i.e., 2.9 and 3.6) if int is used instead of float then the result will not be clearly outputted i.e., instead of 10.44 the computer displays only 10 (as said earlier).</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>System.out.println("the product of a and b = " + product);</p>
<p>is replaced by the statement:</p>
<p>System.out.println(a + "* " + b + " = " + product);</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>2.9 * 3.6 = 10.44</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong>The word public in the statement:</li>
</ul>
<p>public class HelloWorld</p>
<p>implies: that the program or the data within the program (such as methods, variables etc.) can be accessed directly by an external java program.</p>
<p>&nbsp;</p>
<p>If replace the word public by private i.e.,</p>
<p>private class HelloWorld</p>
<p>is written instead of</p>
<p>public class HelloWorld -- then the program or the data within the program (such as methods, variables etc.) cannot be accessed directly by an external program.</p>
<p>&nbsp;</p>
<p>If you insert a value 2^3 for a and 3^2 for b, then as said earlier wrong result or compilation error will be flagged on the screen.</p>
<p>a=2^3</p>
<p>b=3^2; ---&gt; ERROR</p>
<p>a=2* 2*2</p>
<p>b=3*3; ---&gt; Result will be outputted on the screen i.e.,</p>
<p>the product of a and b = 72</p>
<p>&nbsp;</p>
<p>If you want to insert a 10 digit number for a and b i.e.,</p>
<p>a=1000000000</p>
<p>b=3000000000, then the statement:</p>
<p>int a, b, product;</p>
<p>should be replaced by the statement:</p>
<p>long int a, b, product;</p>
<p>i.e.,</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>long int a, b, product;</p>
<p>a=1000000000;</p>
<p>b=2000000000;</p>
<p>product = a * b;</p>
<p>System.out.println("the product of a and b = " + product);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of a and b = 3000000000000000000</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>static public void main(String args []) {</p>
<p>float x;</p>
<p>x = 2;</p>
<p>System.out.println(" square of a number = " + Math.pow((x), 2));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>square of a number = 4</p>
<p><strong>Program 2.2</strong></p>
<p><strong>Java program to find the square of a number</strong></p>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b = a * a;</p>
<p>System.out.println("the square of a = " + b);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the square of a = 4</p>
<p>&nbsp;</p>
<p>If you want to supply the value for a through the key board, then we have to rewrite the above program as follows:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int a, b;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any Number: ");</p>
<p>a = scan.nextInt();</p>
<p>b = a * a;</p>
<p>System.out.println("the square of a = " + b);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any number:</p>
<p>If you enter a number 3</p>
<p>the square of a = 9 will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>&nbsp;</p>
<p>If scan.nextint() is written instead of scan.nextInt()</p>
<p>public static void main(string [] args); is written instead of public static void main(String [] args)</p>
<p>system.out.println("the square of a = " + b); is written instead of System.out.println("the square of a = " + b);</p>
<p>Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.3</strong></p>
<p><strong>Java program to find the greatest of two numbers using if - else statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>The syntax of if &ndash; else statement is:</p>
<p>&nbsp;</p>
<p><strong>if (this condition is true)</strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement using the println method </strong></p>
<p><strong>}</strong></p>
<p><strong>else </strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement using the println method</strong></p>
<p><strong>}</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b;</p>
<p>a=2;</p>
<p>b =3;</p>
<p>if(a&gt;b)</p>
<p>{</p>
<p>System.out.println("a is greater than b");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("b is greater than a");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>b is greater than a</p>
<p>In the above program:</p>
<p>if the condition (a&gt; b) is true, then the statement</p>
<p>{</p>
<p>System.out.println("a is greater than b");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>a is greater than b</p>
<p>else</p>
<p>the statement</p>
<p>{</p>
<p>System.out.println("b is greater than a");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>b is greater than a</p>
<p>&nbsp;</p>
<p>If you want to supply the values for a and b through the key board, then the above program should be rewritten as:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any two Numbers: ");</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>if(a&gt;b)</p>
<p>{</p>
<p>System.out.println("a is greater than b");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("b is greater than a");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two Numbers:</p>
<p>If you enter two numbers 2 and 3</p>
<p>b is greater than a</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>Even if the statements:</p>
<p>System.out.println("a is greater than b");</p>
<p>System.out.println ("b is greater than a");</p>
<p>are not written within the braces {&nbsp;&nbsp; }</p>
<p>i.e.,</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any two Numbers: ");</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>if(a&gt;b)</p>
<p>System.out.println("a is greater than b");</p>
<p>if(b&gt;a)</p>
<p>System.out.println("b is greater than a");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>There will no display of compilation error on the screen or there will be no change in the output displayed on the screen (i.e., b is greater than a will be outputted on the screen).</p>
<p>&nbsp;</p>
<p><strong>Program 2.4</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Java program to find the greatest of three numbers using if &ndash; else if &ndash; else&nbsp; statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>The syntax of if &ndash; else&nbsp; if &ndash; else statement is:</p>
<p>&nbsp;</p>
<p><strong>if (this condition is true)</strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement using the method System.out.println( );</strong></p>
<p><strong>}</strong></p>
<p><strong>else if (this condition is true)</strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement using the method System.out.println( );</strong></p>
<p><strong>}</strong></p>
<p><strong>else&nbsp; </strong></p>
<p><strong>{</strong></p>
<p><strong>print this statement using the method System.out.println( );</strong></p>
<p><strong>}</strong></p>
<p><strong>&nbsp;</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b, c;</p>
<p>a=2;</p>
<p>b =3;</p>
<p>c=4;</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>{</p>
<p>System.out.println("a is greater than b and c");</p>
<p>}</p>
<p>else if(b&gt;a&amp;&amp;b&gt;c)</p>
<p>{</p>
<p>System.out.println("b is greater than a and c");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("c is greater than b and a");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>c is greater than b and a</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note: </strong></li>
</ul>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>&nbsp;</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>{</p>
<p>System.out.println("a is greater than b and c");</p>
<p>}</p>
<p>else if(b&gt;a&amp;&amp;b&gt;c)</p>
<p>{</p>
<p>System.out.println("b is greater than a and c");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("c is greater than b and a");</p>
<p>}</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>if(a&gt;b&amp;&amp;a&gt;c)</p>
<p>{</p>
<p>System.out.println(a + "is greater than" + b&nbsp; + "and" + c);</p>
<p>}</p>
<p>else if(b&gt;a&amp;&amp;b&gt;c)</p>
<p>{</p>
<p>System.out.println(b + "is greater than" + a&nbsp; + "and" + c);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println(c + "is greater than" + b&nbsp; + "and" + a);</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen is:</strong></p>
<p>4 is greater than 3 and 2</p>
<p>&nbsp;</p>
<p><strong>Program 2.5</strong></p>
<p><strong>Java program to find the average of 10 numbers</strong></p>
<p><strong>&nbsp;</strong></p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int N1, N2, N3, N4, N5, N6, N7, N8, N9, N10, X;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any ten Numbers: ");</p>
<p>N1 = scan.nextInt();</p>
<p>N2 = scan.nextInt();</p>
<p>N3 = scan.nextInt();</p>
<p>N4 = scan.nextInt();</p>
<p>N5 = scan.nextInt();</p>
<p>N6 = scan.nextInt();</p>
<p>N7 = scan.nextInt();</p>
<p>N8 = scan.nextInt();</p>
<p>N9 = scan.nextInt();</p>
<p>N10 = scan.nextInt();</p>
<p>X = (N1 + N2 + N3 + N4 + N5 + N6 + N7 + N8 + N9 + N10) /10;</p>
<p>System.out.println("the average of 10 numbers = " + X);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any ten Numbers:</p>
<p>If you enter ten numbers 1, 2, 3, 4, 5, 6, 7, 8, 9 and 10</p>
<p>the average of 10 numbers = 5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> The average of 10 numbers is 5.5, the output on the screen is 5 because int is used instead of float.</li>
</ul>
<p>&nbsp;</p>
<p><strong>Program 2.6</strong></p>
<p><strong>Java program to find the simple interest</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int P,T, R, SI;</p>
<p>P = 1000;</p>
<p>T = 2;</p>
<p>R = 3;</p>
<p>SI = P*T*R/100;</p>
<p>System.out.println("the simple interest = " + SI);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the simple interest = 60</p>
<p>&nbsp;</p>
<p>If you want to supply the values for P, T and R through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>int P,T, R, SI;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter principal amount:");</p>
<p>P = scan.nextInt();</p>
<p>System.out.println("Enter time:");</p>
<p>T = scan.nextInt();</p>
<p>System.out.println("Enter rate of interest:");</p>
<p>R = scan.nextInt();</p>
<p>SI = P*T*R/100;</p>
<p>System.out.println("the simple interest = " + SI);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter principal amount:</p>
<p>If you enter the principal amount 1000</p>
<p>Enter time:</p>
<p>If you enter the time 2</p>
<p>Enter rate of interest:</p>
<p>If you enter the rate of interest 3</p>
<p>the simple interest = 60</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.7</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Java program to find the senior citizen</strong></p>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int age;</p>
<p>age=20;</p>
<p>if(age&gt; = 60)</p>
<p>{</p>
<p>System.out.println("senior citizen");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("not a senior citizen");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>not a senior citizen</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>(age&gt; = 60) implies age greater than or equal to 60</p>
<p>&nbsp;</p>
<p>If you want to supply the value for age through the key board, then the above program should be rewritten as:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int age;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter the age: ");</p>
<p>age = scan.nextInt();</p>
<p>if(age&gt; = 60)</p>
<p>{</p>
<p>System.out.println("senior citizen");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("not a senior citizen");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter the age:</p>
<p>If you enter the age 60</p>
<p>senior citizen</p>
<p>will be outputted on the screen.</p>
<p>Suppose if you enter the age 28</p>
<p>not a senior citizen</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.8</strong></p>
<p><strong>Java program to get marks for 3 subjects and declare the result:</strong></p>
<p><strong>If the marks &gt;= 35 in all the subjects the student passes else fails.</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int M1, M2,M3;</p>
<p>M1 = 38;</p>
<p>M2= 45;</p>
<p>M3 = 67;</p>
<p>if(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35)</p>
<p>{</p>
<p>System.out.println("candidate is passed");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("candidate is failed");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>candidate is passed</p>
<p>(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35) imply M1 is greater than or equal to 35 and M2 is greater than or equal to 35 and M3 is greater than or equal to 35.</p>
<p>&gt;= imply greater than or equal to.</p>
<p>&amp;&amp; imply and whereas &amp; imply address.</p>
<p>(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35) is the condition and if the condition:</p>
<p>(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35) is true, then the statement</p>
<p>{</p>
<p>System.out.println("candidate is passed");</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>candidate is passed</p>
<p>else the statement</p>
<p>{</p>
<p>System.out.println("candidate is failed");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>candidate is failed</p>
<p>&nbsp;</p>
<p>If you want to supply the values for marks M1, M2 and M3 through the key board, then the above program should be rewritten as:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int age;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any three Numbers: ");</p>
<p>M1= scan.nextInt();</p>
<p>M2 = scan.nextInt();</p>
<p>M3 = scan.nextInt();</p>
<p>if(M1&gt;= 35 &amp;&amp; M2&gt;= 35 &amp;&amp; M3&gt;= 35)</p>
<p>{</p>
<p>System.out.println("candidate is passed");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("candidate is failed");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any three Numbers:</p>
<p>If you enter three numbers 26, 28, 39</p>
<p>candidate is failed</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 2.9</strong></p>
<p><strong>Java program to find profit or loss</strong></p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int CP, SP, loss, profit;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter cost price: ");</p>
<p>CP = scan.nextInt();</p>
<p>System.out.println("Enter selling price: ");</p>
<p>SP = scan.nextInt();</p>
<p>if(SP&gt;CP)</p>
<p>{</p>
<p>System.out.println("profit= " + (SP-CP));</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("loss ="&nbsp; +(CP-SP));</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter cost price:</p>
<p>If you enter the cost price 25</p>
<p>Enter selling price:</p>
<p>If you enter the selling price 26</p>
<p>profit = 1</p>
<p>will be outputted on the screen.</p>
<p>If the condition (SP&gt;CP) is true, then the statement:</p>
<p>{</p>
<p>System.out.println("profit= " + (SP-CP));</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>profit = (SP-CP) (in this case profit = 26-25 =1)</p>
<p>else the statement:</p>
<p>{</p>
<p>System.out.println("loss ="&nbsp; + (CP-SP));</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>loss = (CP-SP)</p>
<p><strong>Program 3.0</strong></p>
<p><strong>Java program to find the incremented and decremented values of two numbers</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b, c, d, e, f;</p>
<p>a = 10;</p>
<p>b=12;</p>
<p>c=a+1;</p>
<p>d=b+1;</p>
<p>e=a-1;</p>
<p>f=b-1;</p>
<p>&nbsp;</p>
<p>System.out.print("the incremented value of a = "+ c);</p>
<p>System.out.print("the incremented value of b = "+ d);</p>
<p>System.out.print("the decremented value of a = "+ e);</p>
<p>System.out.print("the decremented value of b = "+ f);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the incremented value of a = 11 the incremented value of b = 13 the decremented value of a = 9 the decremented value of b = 11</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>System.out.print("the incremented value of a = "+ c);</p>
<p>System.out.print("the incremented value of b = " + d);</p>
<p>System.out.print("the decremented value of a = " + e);</p>
<p>System.out.print("the decremented value of b = " + f);</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>System.out.print("\n the incremented value of a = "&nbsp; + c);</p>
<p>System.out.print("\n the incremented value of b = " + d);</p>
<p>System.out.print("\n the decremented value of a = " + e);</p>
<p>System.out.print("\n the decremented value of b = " + f);</p>
<p>&nbsp;</p>
<p>i.e., if the above program is rewritten as:</p>
<p>Then the output on the screen is:</p>
<p>the incremented value of a = 11</p>
<p>the incremented value of b = 13</p>
<p>the decremented value of a = 9</p>
<p>the decremented value of b = 11</p>
<p>&nbsp;</p>
<p>i.e., \n make provision for the another result to print in the new line. If you want to supply the values for a and b through the key board, then the above program should take the form:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a, b, c, d, e, f;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any Number: ");</p>
<p>a = scan.nextInt();</p>
<p>System.out.println("Enter any Number: ");</p>
<p>b = scan.nextInt();</p>
<p>c=a+1;</p>
<p>d=b+1;</p>
<p>e=a-1;</p>
<p>f=b-1;</p>
<p>System.out.print("\n the incremented value of a = "&nbsp; + c);</p>
<p>System.out.print("\n the incremented value of b = " + d);</p>
<p>System.out.print("\n the decremented value of a = " + e);</p>
<p>System.out.print("\n the decremented value of b = " + f);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any Number:</p>
<p>If you enter the value 2</p>
<p>Enter any Number:</p>
<p>If you enter the value 3</p>
<p>the incremented value of a = 3</p>
<p>the incremented value of b = 4</p>
<p>the decremented value of a = 1</p>
<p>the decremented value of b = 2</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> b++ is same as b + 1 and b-- is same as b - 1.</li>
<li><strong>What will be the output of the following programs:</strong></li>
</ul>
<p>&nbsp;</p>
<p>A)</p>
<p>import java.util.Scanner;</p>
<p>public class temperature{</p>
<p>public static void main(String [] args) {</p>
<p>float T1, T2, A;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any Number: ");</p>
<p>T1 = scan.nextFloat();</p>
<p>System.out.println("Enter any Number: ");</p>
<p>T2 = scan.nextFloat();</p>
<p>A = (T1 + T2) / 2;</p>
<p>System.out.println("the average temperature of the day = " + A);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>Enter any Number:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you enter the number 2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Enter any Number:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbnbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you enter the number 3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>the average temperature of the day = 2.5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>B)</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int P;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter the percentage: ");</p>
<p>P = scan.nextInt();</p>
<p>if(P &gt;= 60)</p>
<p>{</p>
<p>System.out.println("first class");</p>
<p>}</p>
<p>else if(P&gt;=50&amp;&amp;P &lt;60)</p>
<p>{</p>
<p>System.out.println("second class");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("pass class");</p>
<p>}</p>
<p>if(P&lt;40)</p>
<p>{</p>
<p>System.out.println("fail");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>Enter the percentage:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If you enter the number 60&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>first class</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 3.1</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Java&nbsp; program to calculate the discounted price and the total price after discount</strong></p>
<p><strong>Given:</strong></p>
<p>If purchase value is greater than 1000, 10% discount</p>
<p>If purchase value is greater than 5000, 20% discount</p>
<p>If purchase value is greater than 10000, 30% discount</p>
<p>&nbsp;</p>
<ul>
<li><strong>discounted price</strong></li>
</ul>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int PV, dis;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter purchased value: ");</p>
<p>PV = scan.nextInt();</p>
<p>if(PV&lt;1000)</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.1);</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.2);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("dis= " + PV* 0.3);</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 6500</p>
<p>dis = 1300</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>(PV&gt;1000), (PV&gt;5000) denote the conditions and if the condition (PV&gt;1000) is true i.e., purchased value is greater than 1000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.1);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>dis= PV* 10% = PV* 10 /100 = PV* 0.1</p>
<p>and if the condition (PV&gt;1000) is false and if the condition (PV&gt;5000) is true i.e., purchased value is greater than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.2);</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>dis= PV* 20% = PV* 20 /100 = PV* 0.2</p>
<p>and if the condition (PV&gt;5000) is not true i.e., purchased value is less than 5000, then the statement</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.3);</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>dis= PV* 30% = PV* 30 /100 = PV* 0.3</p>
<p>&nbsp;</p>
<ul>
<li><strong>total price </strong></li>
</ul>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int PV, total;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter purchased value: ");</p>
<p>PV = scan.nextInt();</p>
<p>if(PV&lt;1000)</p>
<p>{</p>
<p>System.out.println("total= " +&nbsp; PV - PV* 0.1);</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>System.out.println("total = " + PV- PV* 0.2);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("total= " + PV- PV* 0.3);</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 650</p>
<p>total = 585</p>
<p>will be outputted on the screen.</p>
<p>If the condition (PV&gt;1000) is true i.e., purchased value is greater than 1000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>System.out.println("total= " +&nbsp; PV - PV* 0.1);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*10% = PV- PV* 10 /100 = PV - PV * 0.1</p>
<p>and if the condition (PV&gt;1000) is false and if the condition (PV&gt;5000) is true i.e., purchased value is greater than 5000, then the statement</p>
<p>&nbsp;</p>
<p>{</p>
<p>System.out.println("total= " +&nbsp; PV - PV* 0.2);</p>
<p>}</p>
<p>&nbsp;</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*20% = PV- PV* 20 /100 = PV - PV * 0.2</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>and if the condition (PV&gt; 5000) is not true i.e., purchased value is less than 5000, then the statement</p>
<p>{</p>
<p>System.out.println("total= " +&nbsp; PV - PV* 0.3);</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>total =PV- dis = PV- PV*30% = PV- PV* 30 /100 = PV - PV * 0.3</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> Combing both the programs (above), we can write:</li>
</ul>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int PV, dis, total;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter purchased value: ");</p>
<p>PV = scan.nextInt();</p>
<p>if(PV&lt;1000)</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.1);</p>
<p>System.out.println("total= " + total - dis);</p>
<p>}</p>
<p>else if(PV&gt;5000)</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.2);</p>
<p>System.out.println("total= " + total - dis);</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("dis = " + PV* 0.3);</p>
<p>System.out.println("total= " + total - dis);</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter purchased value:</p>
<p>If you enter the purchased value 850</p>
<p>dis = 85</p>
<p>total = 765</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 3.2</strong></p>
<p><strong>Java program to print the first ten natural numbers using for loop statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int i;</p>
<p>for (i=1; i&lt;=10; i++)</p>
<p>System.out.println("value of i = " + i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>value of i = 1 value of i = 2&nbsp; value of i= 3&nbsp; value of i= 4&nbsp; value of i= 5&nbsp; value of i= 6 value of i = 7 value of i= 8&nbsp; value of i = 9&nbsp; value of i = 10</p>
<p>&nbsp;</p>
<p>for (i=1; i&lt;=10; i++) denote the</p>
<p>for loop statement and the syntax of the</p>
<p>for loop statement is:</p>
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
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 1</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 1+1 = 2</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=2</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 2</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 2+1 = 3</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=3</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 3</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 3+1 = 4</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=4</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 4</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 4+1 = 5</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=5</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 5</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 5+1 = 6</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=6</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 6</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 6+1 = 7</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=7</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 7</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 7+1 = 8</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=8</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 8</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 8+1 = 9</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=9</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 9</p>
<p>Now, the value of i is:</p>
<p>i =&nbsp; 9+1 = 10</p>
<p>Is the condition (i&lt;=10) is true?</p>
<p>Yes because i=10</p>
<p>The statement System.out.println("value of i = " + i); is executed to print the output:</p>
<p>value of i = 10</p>
<p>and stop because the condition i&lt;=10 is achieved.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>System.out.println("value of i = " + i);</p>
<p>is replaced by the statement:</p>
<p>System.out.println("\nvalue of i = " + i);</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>Then the output on the screen is:</p>
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
<p>value of i = 1 value of i = 2 &nbsp;value of i= 3&nbsp; value of i= 4&nbsp; value of i= 5&nbsp; value of i= 6 value of i = 7 value of i= 8&nbsp; value of i = 9</p>
<p>&nbsp;</p>
<p>(<strong>Note: </strong>the condition i&lt;=10 tells to print till value of i =10 but the condition i&lt;10 tells to print till value of i=9)</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>for(i=1; i=10; i++)</p>
<p>is written instead of the statement:</p>
<p>for (i=1; i&lt;=10; i++), then the <strong>output on the screen</strong> is:</p>
<p>value of i = 10&nbsp; value of i = 10&nbsp; value of i = 10&nbsp; value of&nbsp; i = 10&nbsp; value of i= 10&nbsp; value of i= 10 value of i = 10 value of i= 10&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10&nbsp; value of i = 10&nbsp;&nbsp;&nbsp; value of i = 10&nbsp;&nbsp; value of i = 10 (continues ...).</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>If the statement:</p>
<p>System.out.println("\n value of i = " + i); is replaced by the statement</p>
<p>System.out.println("\n " + i);</p>
<p>&nbsp;</p>
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
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the mistake in the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String []args) throws Exception{</p>
<p>System.out.println("Hello World");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer: </strong></p>
<p>There is no mistake in the above program. Addition of the statement throws Exception does not make any change in the output displayed on the screen or give rise to any compilation error on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 3.3</strong></p>
<p><strong>What will be the output of the following program:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int i;</p>
<p>for (i =1; i&lt;=5; i ++)</p>
<p>System.out.println("\n Linux is not portable");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>Linux is not portable</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the first ten natural numbers using for while loop statement</strong></li>
</ul>
<p>&nbsp;</p>
<p>The syntax of while loop statement is:</p>
<p><strong>while (this is the condition)</strong></p>
<p><strong>{</strong></p>
<p><strong>execute this statement;</strong></p>
<p><strong>}</strong></p>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args)</p>
<p>{</p>
<p>int i = 1;</p>
<p>while (i&lt;=10)</p>
<p>{</p>
<p>System.out.println("\n&nbsp; " + i++);</p>
<p>}</p>
<p>&nbsp;</p>
<p>}</p>
<p>}</p>
<p><strong>The output on the screen is:</strong></p>
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
<p>(i&lt;=10) is the condition and&nbsp;&nbsp;</p>
<p>The statement</p>
<p>System.out.println("\n&nbsp; " + i++);</p>
<p>&nbsp;</p>
<p>is repeatedly executed as long as a given condition (i&lt;=10) is true.</p>
<p>If the statement:</p>
<p>int i=1;</p>
<p>is replaced by the statement:</p>
<p>int i;</p>
<p>Then the compilation error will be displayed on the console screen because initialization is not defined i.e., from where to start is not declared.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int i = 1;</p>
<p>is replaced by the int i = 0;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
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
<ul>
<li><strong>Java program to print first 10 numbers using do while loop statement</strong></li>
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
<p>public class HelloWorld{</p>
<p>public static void main(String [] args)</p>
<p>{</p>
<p>int i =1;</p>
<p>do</p>
<p>{</p>
<p>System.out.println(" \n i= " + i++);</p>
<p>} while (i&lt;=10);</p>
<p>}</p>
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
<p>System.out.println(" \n i= " + i++);</p>
<p>is executed and then condition (i&lt;=10) is checked. If condition (i&lt;=10) is true then</p>
<p>The statement:</p>
<p>System.out.println(" \n i= " + i++);</p>
<p>is executed again. This process repeats until the given condition (i&lt;=10) becomes false.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 3.4</strong></p>
<p><strong>Java program to print the characters from A to Z using for loop, do while loop and while loop statement.</strong></p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the characters from A to Z using for loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>char a;</p>
<p>for( a='A'; a&lt;='Z'; a++)</p>
<p>System.out.println("\n&nbsp;&nbsp; " + a);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p><strong>&nbsp;</strong></p>
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
<p>The statement:</p>
<p>char a; imply that we are creating the character a.</p>
<p>If the statement:</p>
<p>for( a=A; a&lt;=Z; a++) is written instead of the statement for( a='A'; a&lt;='Z'; a++)</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the characters from A to Z using while loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>char a = 'A';</p>
<p>while (a&lt;='Z')</p>
<p>{</p>
<p>System.out.println("\n&nbsp; "&nbsp; + a++);</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the characters from A to Z using do while loop statement:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>char a = 'A';</p>
<p>do</p>
<p>{</p>
<p>System.out.println("\n "&nbsp; +&nbsp; a++);</p>
<p>} while (a&lt;='Z');</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 3.5</strong></p>
<p><strong>Java program to print the given number is even or odd.</strong></p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int a;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter a number: ");</p>
<p>a = scan.nextInt();</p>
<p>if(a%2 = = 0)</p>
<p>{</p>
<p>System.out.println("the number is even");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("the number is odd");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter a number:</p>
<p>If you enter the number 4</p>
<p>the number is even</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>(a%2 = = 0) is the condition and this condition imply: a divided by 2 yields reminder = 0.</p>
<p>For example: if you enter the number 4</p>
<p>Then a = 4</p>
<p>Then 4 divided by 2 yields the remainder = 0</p>
<p>Then the statement:</p>
<p>{</p>
<p>System.out.println("the number is even");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>the number is even</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>(<strong>Note:</strong> in Java language also = = implies equal to)</p>
<p>&nbsp;</p>
<p>If you enter the number 3</p>
<p>Then a = 3</p>
<p>Then 3 divided by 2 yields the remainder = 1</p>
<p>Then the statement</p>
<p>{</p>
<p>System.out.println("the number is odd");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>the number is odd</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Program 3.6</strong></p>
<p><strong>Java program to print the remainder of two numbers </strong></p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int a, b, c;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter a number: ");</p>
<p>a = scan.nextInt();</p>
<p>System.out.println("Enter a number: ");</p>
<p>b = scan.nextInt();</p>
<p>c = a%b;</p>
<p>System.out.println("the remainder of a and b =&nbsp; " + c);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter a number:</p>
<p>If you enter the number 3</p>
<p>Enter a number:</p>
<p>If you enter the number 2</p>
<p>the remainder of a and b = 1</p>
<p>will be outputted on the screen.</p>
<p>Since (a =3 and b =2). Therefore:</p>
<p>3 divided by 2 (i.e., a divided by b) yields the remainder equal to 1.</p>
<p>&nbsp;</p>
<p><strong>Program 3.7</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Java program to check equivalence of two numbers.</strong></p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int x, y;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter a number: ");</p>
<p>x = scan.nextInt();</p>
<p>System.out.println("Enter a number: ");</p>
<p>y = scan.nextInt();</p>
<p>if(x-y==0)</p>
<p>{</p>
<p>System.out.println("the two numbers are equivalent");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("the number are not equivalent");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter a number:</p>
<p>If you enter the number 2</p>
<p>Enter a number:</p>
<p>If you enter the number 2</p>
<p>the two numbers are equivalent</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>Since 2-2 is equal to 0 (i.e., x-y = = 0). Therefore: the statement</p>
<p>{</p>
<p>System.out.println("the two numbers are equivalent");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>two numbers are equivalent</p>
<p>&nbsp;</p>
<p>If you enter the integers 3 and 2</p>
<p><strong>The output on the screen is:</strong></p>
<p>the two numbers are not equivalent</p>
<p>Since 3-2 is not equal to 0 (i.e., x-y != 0). Therefore: the statement</p>
<p>{</p>
<p>System.out.println("the two numbers are not equivalent");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>two numbers are not equivalent</p>
<p>(<strong>Note:</strong> Like in C &amp; C++, in Java language also != implies not equal to)</p>
<p>&nbsp;</p>
<p><strong>Program 3.8</strong></p>
<p><strong>Java program to print the leap year or not </strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int year;</p>
<p>year =1996;</p>
<p>if(year%4==0)</p>
<p>{</p>
<p>System.out.println("leap year");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println("not a leap year");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>The other logic for finding the leap year.</p>
<p>import java.util.Scanner;</p>
<p>public class Check_Leap_Year {</p>
<p>public static void main(String args[]) {</p>
<p>Scanner s = new Scanner(System.in);</p>
<p>System.out.print("Enter any year:");</p>
<p>int year = s.nextInt();</p>
<p>boolean flag = false;</p>
<p>if(year % 400 == 0) {</p>
<p>flag = true;</p>
<p>} else if (year % 100 == 0) {</p>
<p>flag = false;</p>
<p>} else if(year % 4 == 0) {</p>
<p>flag = true;</p>
<p>} else {</p>
<p>flag = false;</p>
<p>}</p>
<p>if(flag) {</p>
<p>System.out.println("Year "+year+" is a Leap Year");</p>
<p>}</p>
<p>else {</p>
<p>System.out.println("Year "+year+" is not a Leap Year");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>leap year</p>
<p>Since year =1996. Therefore:</p>
<p>1996 divided by 4 (i.e., year divided by 4) yields the remainder equal to 0.</p>
<p>The statement</p>
<p>{</p>
<p>System.out.println("leap year");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>leap year</p>
<p>If the year is = 1995. Then</p>
<p>1995 divided by 4 (i.e., year divided by 4) yields the remainder not equal to 0.</p>
<p>The statement</p>
<p>{</p>
<p>System.out.println("not a leap year");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>not a leap year</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output on the screen:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>int a =5;</p>
<p>public static void main(String[] args){</p>
<p>int a =2 ;</p>
<p>System.out.println(" value of a = " + a);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>value of a = 2</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>System.out.println(" value of a = " + a); is replaced by the statement</p>
<p>System.out.println(" value of a = " + ::a);&nbsp; (where :: denote scope resolution operator)</p>
<p>i.e.,</p>
<p>public class HelloWorld{</p>
<p>int a =5;</p>
<p>public static void main(String[] args){</p>
<p>int a =2 ;</p>
<p>System.out.println(" value of a = " + ::a);</p>
<p>}</p>
<p>}</p>
<p>Then the compilation error will be displayed on the screen because like C++ -- java does not hold / support the resolution operator.</p>
<p>&nbsp;</p>
<p><strong>Program 3.9</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Java program to print whether the given number is positive or negative</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int a;</p>
<p>a = -35;</p>
<p>if(a&gt;0)</p>
<p>{</p>
<p>System.out.println("number is positive");</p>
<p>}</p>
<p>else</p>
<p>{</p>
<p>System.out.println(" number entered is negative");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>number entered is negative</p>
<p>Since a = -35. Therefore:</p>
<p>a is less than 0 i.e., a&lt;0</p>
<p>The statement</p>
<p>{</p>
<p>System.out.println("number is negative");</p>
<p>}</p>
<p>is executed to print the output:</p>
<p>number entered is negative</p>
<p>&nbsp;</p>
<p><strong>Program 4.0</strong></p>
<p><strong>Java program to print the sum of the first 10 digits using for loop statement:</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int i,&nbsp; sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>System.out.println("sum of&nbsp; the first 10 digits = " + sum);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 digits = 55</p>
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
<p>System.out.println("sum of&nbsp; the first 10 digits = " + sum); is executed to display the output:</p>
<p>sum of the first 10 digits = 55</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>System.out.println("sum of&nbsp; the first 10 digits = " + sum);</p>
<p>is executed to print the output:</p>
<p>sum of the first 10 digits = 55</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>If the statement:</p>
<p>int i, sum = 0;</p>
<p>is replaced by int i, sum = 1;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>sum of the first10 digits = 56</p>
<ul>
<li><strong>What will be the output if the for loop statement </strong>for(i =1; i&lt;=10; i++)<strong> is replaced by the statement </strong>for(i =2; i&lt;10; i++)<strong>?</strong></li>
</ul>
<p>&nbsp;</p>
<p><strong>Answer: </strong>sum of 10 digits = 44</p>
<p>&nbsp;</p>
<p>If the statement int i, sum, sum = 0; is written instead of int i, sum = 0;</p>
<p>Then the compilation error message will be displayed on the screen (stating that sum is twice declared).</p>
<p>&nbsp;</p>
<p>If the for loop is ended with a semicolon i.e.,</p>
<p>for( i=1; i&lt;=10; i++);</p>
<p>Then the compilation error will be displayed on the console screen.</p>
<p>&nbsp;</p>
<p><strong>Program 4.1</strong></p>
<p><strong>Java program to print the average of the first 10 numbers using for loop statement</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int i, avg, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>avg = sum/10;</p>
<p>System.out.println("sum of the first 10 numbers = " + sum);</p>
<p>System.out.println("average of the first 10 numbers =&nbsp; " + avg);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 numbers = 55</p>
<p>average of the first 10 numbers = 5</p>
<p>The average of the first 10 numbers = 55/10 = 5.5 not 5. But the output on the screen is:</p>
<p>average of the first 10 numbers = 5</p>
<p>because int is used instead of float.</p>
<p>&nbsp;</p>
<p>If the data type float is used i.e.,</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>float i, avg, sum = 0;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>sum = sum + i;</p>
<p>avg = sum/10;</p>
<p>System.out.println("sum of the first 10 numbers = " + sum);</p>
<p>System.out.println("average of the first 10 numbers = " + avg);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of the first 10 numbers = 55</p>
<p>average of the first 10 numbers = 5.5</p>
<p>&nbsp;</p>
<p><strong>Program 4.2</strong></p>
<p><strong>Java program to print the product of the first 10 digits using for loop statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args) {</p>
<p>int i, product = 1;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>product = product * i;</p>
<p>System.out.println("the product of the first 10 digits = " + product);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>the product of the first 10 digits = 3628800</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
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
<p>System.out.println("the product of the first10 digits = " + product); is executed to display the output:</p>
<p>the product of the first 10 digits = 3628800</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>If the statement int i, product = 1; is replaced by int i, product = 0;</p>
<p>Then the output on the screen is:</p>
<p>the product of the first 10 digits = 0</p>
<p>&nbsp;</p>
<p>If the statement for(i=1; i&lt;=10; i++) is replaced by for(i=5; i&lt;=8; i++)</p>
<p>Then the output on the screen is:</p>
<p>the product of the first 10 digits = 1680</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p><strong>Program 4.3</strong></p>
<p><strong>Java Program to print the table of a number using the for loop statement</strong></p>
<p><strong>&nbsp;</strong></p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int n, i;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter a number: ");</p>
<p>n = scan.nextInt();</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; *&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n * i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
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
<p>Since you entered the number 2, therefore: n=2.</p>
<p>i=1</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 1 = 2</p>
<p>using the statement System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; *&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n * i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 2 = 4</p>
<p>using the statement System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; *&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n * i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 3 = 6</p>
<p>using the statement System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; *&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n * i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 4 = 8</p>
<p>using the statement System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; *&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n * i);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=5</p>
<p>Is i&lt;=5 true?</p>
<p>Yes, print this</p>
<p>2 * 5 = 10</p>
<p>using the statement System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; *&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n * i);</p>
<p>&nbsp;</p>
<p>stop Now because the condition i &lt;=5 is achieved.</p>
<p>&nbsp;</p>
<p>If the symbol * is replaced by +</p>
<p>i.e.,</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String [] args){</p>
<p>int n, i;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter a number: ");</p>
<p>n = scan.nextInt();</p>
<p>for( i=1; i&lt;=5; i++)</p>
<p>System.out.println ( \n n&nbsp; +&nbsp; "&nbsp; +&nbsp;&nbsp; " +&nbsp; i + "&nbsp; =&nbsp; " +&nbsp; n + i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
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
<p><strong>Program 4.4</strong></p>
<p><strong>Java program to print the first 10 numbers starting from one together with their squares</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>System.out.println(" number = " +&nbsp; i +&nbsp; " its square =&nbsp; " + i*i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>number = 1 its square=1number = 2 its square=4number = 3 its square=9number = 4 its square=16number = 5 its square=25number = 6 its square=36number = 7 its square=49number = 8 its square=64number = 9 its square=81number= 10 its square=100</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>System.out.println(" number = " +&nbsp; i +&nbsp; " its square =&nbsp; " + i*i); is replaced by the statement</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " its square =&nbsp; " + i*i);</p>
<p>&nbsp;</p>
<p>i.e., if the above program is rewritten as:</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " its square =&nbsp; " + i*i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen is:</strong></p>
<p>number = 1 its square=1</p>
<p>number = 2 its square=4</p>
<p>number = 3 its square=9</p>
<p>number = 4 its square=16</p>
<p>number = 5 its square=25</p>
<p>number = 6 its square=36</p>
<p>number = 7 its square=49</p>
<p>number = 8 its square=64</p>
<p>number = 9 its square=81</p>
<p>number= 10 its square=100</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " its square =&nbsp; " + i*i); is replaced by the statement:</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " \t its square =&nbsp; " + i*i);</p>
<p>&nbsp;</p>
<p>i.e., if the above program is rewritten as:</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " \t its square =&nbsp; " + i*i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>number=1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; its square=1</p>
<p>number=2&nbsp;&nbsp;&nbsp;&nbsp; its square=4</p>
<p>number=3&nbsp;&nbsp;&nbsp;&nbsp; its square=9</p>
<p>number=4&nbsp;&nbsp;&nbsp;&nbsp; its square=16</p>
<p>number=5&nbsp;&nbsp;&nbsp;&nbsp; its square=25</p>
<p>number=6&nbsp;&nbsp;&nbsp;&nbsp; its square=36</p>
<p>number=7&nbsp;&nbsp;&nbsp;&nbsp; its square=49</p>
<p>number=8&nbsp;&nbsp;&nbsp;&nbsp; its square=64</p>
<p>number=9&nbsp;&nbsp;&nbsp;&nbsp; its square=81</p>
<p>number=10&nbsp;&nbsp;&nbsp;&nbsp; its square=100</p>
<p>&nbsp;</p>
<p>tab /t is included because to leave space between</p>
<p>number =1&nbsp;&nbsp; and&nbsp;&nbsp; its square=1</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>System.out.println(" \n number = " + i +&nbsp; " \t its square =&nbsp; " + i*i);&nbsp; is replaced by the statement:</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " \n its square =&nbsp; " + i*i);</p>
<p>&nbsp;</p>
<p>i.e., if the above program is rewritten as:</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " \n its square =&nbsp; " + i*i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>number = 1</p>
<p>its square=1</p>
<p>number = 2</p>
<p>its square=4</p>
<p>number = 3</p>
<p>its square=9</p>
<p>number = 4</p>
<p>its square=16</p>
<p>number = 5</p>
<p>its square=25</p>
<p>number = 6</p>
<p>its square=36</p>
<p>number = 7</p>
<p>its square=49</p>
<p>number = 8</p>
<p>its square=64</p>
<p>number = 9</p>
<p>its square=81</p>
<p>number= 10</p>
<p>its square=100</p>
<p>&nbsp;</p>
<ul>
<li><strong>Write a program to print the first 10 numbers starting from one together with their squares and cubes:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p><strong>Answer: </strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) throws Exception{</p>
<p>int i;</p>
<p>for( i=1; i&lt;=10; i++)</p>
<p>System.out.println(" \n number = " +&nbsp; i +&nbsp; " its square =&nbsp; " + i*i + " its cube = " + i*i*i);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Program 4.5</strong></p>
<p><strong>Java program to print the sum of two numbers using method</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int a, b, c;</p>
<p>a = 11;</p>
<p>b = 6;</p>
<p>c = add (a, b);</p>
<p>System.out.println(" sum of two numbers = " + c);</p>
<p>}</p>
<p>public static int add (int a, int b) {</p>
<p>return (a+b) ;</p>
<p>}</p>
<p>}</p>
<p><strong>The output on the screen:</strong></p>
<p>sum of two numbers = 17</p>
<p>&nbsp;</p>
<p>There are 2 methods in the above program:</p>
<ul>
<li>public static void main(String[] args)</li>
<li>public static int add (int a, int b)</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>public static void main(String[] args) imply: main method and</p>
<p>{</p>
<p>} imply the body of the main method with in which the program statements:</p>
<p>int a, b, c;</p>
<p>a = 11;</p>
<p>b = 6;</p>
<p>c = add (a, b);</p>
<p>System.out.println(" sum of two numbers = " + c); are written.</p>
<p>&nbsp;</p>
<p>Like in C ++ (the function declaration is not made) and unlike in C ((the function declaration is made) -- there is no need for method declaration in Java (i.e., without the method declaration the program will be successfully executed and the result will be outputted on the screen)</p>
<p>&nbsp;</p>
<p>public static int add (int a, int b) imply: the method to add two integers x and y and</p>
<p>{</p>
<p>return (a+b) ;</p>
<p>}</p>
<p>} imply the body of the method public static int add (int a, int b)</p>
<p>&nbsp;</p>
<p>main method:&nbsp;</p>
<p>public static void main(String[] args)</p>
<p>and the method:&nbsp;</p>
<p>public static int add (int a, int b)</p>
<p>should be written inside the body of the public class HelloWorld.</p>
<p>&nbsp;</p>
<p>The statement int a, b, c; imply that we creating the integer variables a, b and c.</p>
<p>&nbsp;</p>
<p>The statements:</p>
<p>a = 11;</p>
<p>b = 6;</p>
<p>c = add (a, b);</p>
<p>imply that we are assigning the values to the created variables.</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>c = add (x, y); imply method call (i.e., we are calling the method public static int add (int a, int b) to add the values (i.e., 11 and 6) and return the result (i.e., 17) to the statement System.out.println(" sum of two numbers = " + c); to make provision to display the output of the sum of two entered numbers as 17 on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the product of two numbers using method</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) {</p>
<p>int a, b, c;</p>
<p>a = 2;</p>
<p>b = 3;</p>
<p>c = mult (a, b);</p>
<p>System.out.println(" product of two numbers&nbsp; = " + c);</p>
<p>}</p>
<p>public static int mult (int a, int b){</p>
<p>return (a*b) ;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>product of two numbers = 6</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the greatest of two numbers using method</strong></li>
</ul>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) {</p>
<p>int a, b;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any two numbers: ");</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>System.out.println(" largest of two numbers&nbsp; = " + max (a, b) );</p>
<p>}</p>
<p>public static int max (int a, int b) {</p>
<p>if(a&gt;b)</p>
<p>return a;</p>
<p>else</p>
<p>return b;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any two numbers:</p>
<p>If you enter two numbers 5 and 2</p>
<p>largest of two numbers= 5</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the greatest of three numbers using method</strong></li>
</ul>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) {</p>
<p>int a, b, c;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any three numbers: ");</p>
<p>a = scan.nextInt();</p>
<p>b = scan.nextInt();</p>
<p>c= scan.nextInt();</p>
<p>System.out.println(" largest of two numbers&nbsp; = " + max (a, b, c) );</p>
<p>}</p>
<p>public static int max (int a, int b, int c) {</p>
<p>if(a&gt;b &amp;&amp; a&gt;c)</p>
<p>return a;</p>
<p>else if (b&gt;c &amp;&amp; b&gt;a)</p>
<p>return b;</p>
<p>else</p>
<p>return c;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any three numbers:</p>
<p>If you enter three numbers 3, 5 and 10</p>
<p>largest of three numbers = 10</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the square of the number using method</strong></li>
</ul>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) {</p>
<p>int x;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.println("Enter any number: ");</p>
<p>x = scan.nextInt();</p>
<p>System.out.println("square of the number = " + square (x));</p>
<p>}</p>
<p>public static int square (int x){</p>
<p>return x*x;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>Enter any number:</p>
<p>If you enter the number 5</p>
<p>square of the number = 25</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p><strong>Program 4.6</strong></p>
<p><strong>Switch (case)</strong> allows to make decision from the number of choices i.e., from the number of cases</p>
<p><strong>For example:</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args)throws Exception{</p>
<p>char ch;</p>
<p>System.out.print("Enter a character:");</p>
<p>ch = (char)System.in.read();</p>
<p>switch(ch)</p>
<p>{</p>
<p>case 'R':</p>
<p>System.out.print("Red");</p>
<p>break;</p>
<p>case 'W':</p>
<p>System.out.print("White");</p>
<p>break;</p>
<p>case 'Y':</p>
<p>System.out.print("Yellow");</p>
<p>break;</p>
<p>case 'G':</p>
<p>System.out.print("Green");</p>
<p>break;</p>
<p>default:</p>
<p>System.out.print("Error");</p>
<p>break;</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen is:</strong></p>
<p>Enter a character:</p>
<p>If you enter a character R</p>
<p>Red</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>switch(ch) allow to make decision from the number of choices i.e., from the number of cases</p>
<p>case 'R':</p>
<p>case 'W':</p>
<p>case 'Y':</p>
<p>case 'G':</p>
<p>Since we have entered the character R (which corresponds to case 'R':)</p>
<p>The statement:</p>
<p>System.out.print("Red");</p>
<p>is executed to display the output:</p>
<p>Red</p>
<p>on the screen.</p>
<p>Suppose you enter a character K</p>
<p><strong>The output on the screen is:</strong></p>
<p>Error</p>
<p>(Entered character K does not correspond to any of the cases</p>
<p>case 'R':</p>
<p>case 'W':</p>
<p>case 'Y':</p>
<p>case 'G':</p>
<p>Therefore the statements:</p>
<p>default:</p>
<p>System.out.print("Error");</p>
<p>are executed to display the output:</p>
<p>Error</p>
<p>on the screen).</p>
<p>&nbsp;</p>
<p>If the statements:</p>
<p>{</p>
<p>case 'R':</p>
<p>System.out.print("Red");</p>
<p>break;</p>
<p>case 'W':</p>
<p>System.out.print("White");</p>
<p>break;</p>
<p>case 'Y':</p>
<p>System.out.print("Yellow");</p>
<p>break;</p>
<p>case 'G':</p>
<p>System.out.print("Green");</p>
<p>break;</p>
<p>default:</p>
<p>System.out.print("Error");</p>
<p>break;</p>
<p>}</p>
<p>&nbsp;</p>
<p>are replaced by the statements:</p>
<p>&nbsp;</p>
<p>{</p>
<p>case 'R':</p>
<p>System.out.print("Red");</p>
<p>case 'W':</p>
<p>System.out.print("White");</p>
<p>case 'Y':</p>
<p>System.out.print("Yellow");</p>
<p>break;</p>
<p>case 'G':</p>
<p>System.out.print("Green");</p>
<p>break;</p>
<p>default:</p>
<p>System.out.print("Error");</p>
<p>break;</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen is:</strong></p>
<p>Red</p>
<p>White</p>
<p>Yellow</p>
<p>i.e., the output is printed till yellow even though you have entered the character R.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong> C and C++ supports pointers and structures whereas Java does not i.e., Java do not support structures and pointers because JVM (Java virtual machine&rarr; a core component of java) do not support structures and pointers.</li>
</ul>
<p>&nbsp;</p>
<p><strong>Program 4.7</strong></p>
<p><strong>Java program to print the output </strong></p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p><strong>using arrays: </strong></p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i;</p>
<p>int [] num = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>Ends because of the condition i&lt;5.</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>//--------------------------------------------------------------------------------------------------------------------//-</p>
<p>Array declaration in C:</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>or</p>
<p>int num [] = {16, 18, 20, 25, 36};</p>
<p>&nbsp;</p>
<p>Array declaration in C++:</p>
<p>int num [5] = {16, 18, 20, 25, 36};</p>
<p>or</p>
<p>int num [] = {16, 18, 20, 25, 36};</p>
<p>&nbsp;</p>
<p>But array declaration in java:</p>
<p>int [] num = {16, 18, 20, 25, 36};</p>
<p>&nbsp;</p>
<p>//------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<p>The statement:</p>
<p>int [] num = {16, 18, 20, 25, 36}; imply that we are creating an integer array (and the name of array is num) consisting of 5 values (i.e., 16, 18, 20, 25, 36) of the same data type int.</p>
<p>&nbsp;</p>
<p>With the declaration int [] num = {16, 18, 20, 25, 36}; -- computer creates 5 memory cells (because there are 5 elements within the braces {}) with name num[0], num[1], num[2], num[3], num[4]. And since</p>
<p>int [ ] num = {16, 18, 20, 25, 36};</p>
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
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=1</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [1] = 18</p>
<p>using the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=2</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [2] = 20</p>
<p>using the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=3</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [3] = 25</p>
<p>using the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]);</p>
<p>&nbsp;</p>
<p>Now,</p>
<p>i=4</p>
<p>Is i&lt;5 true?</p>
<p>Yes, print this</p>
<p>Element [4] = 36</p>
<p>using the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]);</p>
<p>Stop because the condition is i&lt;5.</p>
<p>&nbsp;</p>
<p>If i&lt;=5 i.e., if the for loop statement was</p>
<p>for(i=0; i&lt;=5; i++)</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>Element [0] = 16</p>
<p>Element [1] = 18</p>
<p>Element [2] = 20</p>
<p>Element [3] = 25</p>
<p>Element [4] = 36</p>
<p>Element [5] = 365</p>
<p>&nbsp;</p>
<p>365 is the number stored in the memory i.e., any number stored in the memory will be displayed.</p>
<p>&nbsp;</p>
<p>If the statement int [] num = {16, 18, 20, 25, 36}; is replaced by the statement:</p>
<p>int [5] num = {16, 18, 20, 25, 36};</p>
<p>or by the statement:</p>
<p>int num [i] = {16, 18, 20, 25, 36};</p>
<p>Then the compilation error will be displayed on the screen.</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]); is replaced by the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[0]);</p>
<p>&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>Element [0] = 16</p>
<p>Element [1] = 16</p>
<p>Element [2] = 16</p>
<p>Element [3] = 16</p>
<p>Element [4] = 16</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]); is replaced by the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[1]);</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>Element [0] = 18</p>
<p>Element [1] = 18</p>
<p>Element [2] = 18</p>
<p>Element [3] = 18</p>
<p>Element [4] = 18</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]); is replaced by the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[2]);</p>
<p>&nbsp;</p>
<p>Then the <strong>output on the screen</strong> is:</p>
<p>Element [0] = 20</p>
<p>Element [1] = 20</p>
<p>Element [2] = 20</p>
<p>Element [3] = 20</p>
<p>Element [4] = 20</p>
<p>&nbsp;</p>
<p>Suppose the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[i]); is replaced by the statement:</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[3]);</p>
<p>&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>Element [0] = 25</p>
<p>Element [1] = 25</p>
<p>Element [2] = 25</p>
<p>Element [3] = 25</p>
<p>Element [4] = 25</p>
<p>&nbsp;</p>
<p>Suppose the statement System.out.println("Element [" +&nbsp; i + " ] = " + num[i]); is replaced by the statement</p>
<p>System.out.println("Element [" +&nbsp; i + " ] = " + num[4]);</p>
<p>&nbsp;</p>
<p>Then the output on the screen is:</p>
<p>Element [0] = 36</p>
<p>Element [1] = 36</p>
<p>Element [2] = 36</p>
<p>Element [3] = 36</p>
<p>Element [4] = 36</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the sum of the elements in array.</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i, sum = 0;</p>
<p>int [] num = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>sum = sum + num[i];</p>
<p>System.out.println("Sum of the Elements in the array&nbsp; = " +&nbsp; sum);</p>
<p>}</p>
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
<p>System.out.println("Sum of the Elements in the array&nbsp; = " +&nbsp; sum); is executed to display the output:</p>
<p>Sum of the Elements in the array = 115</p>
<p>on the screen.</p>
<p>&nbsp;</p>
<p>If the statement:</p>
<p>int i, sum = 0;</p>
<p>is replaced by int i, sum = 1;</p>
<p>Then The output on the screen:</p>
<p>Sum of the Elements in the array = 116</p>
<p>&nbsp;</p>
<ul>
<li><strong>Java program to print the average of the elements in the array </strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args){</p>
<p>int i, avg, sum = 0;</p>
<p>int [] num = {16, 18, 20, 25, 36};</p>
<p>for(i=0; i&lt;5; i++)</p>
<p>sum = sum + num[i];</p>
<p>avg = sum/5;</p>
<p>System.out.println("Sum of the Elements in the array = " +&nbsp; sum);</p>
<p>System.out.println("average of the Elements in the array = " +&nbsp; avg);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Sum of the Elements in the array = 115</p>
<p>average of the elements in the array = 23</p>
<ul>
<li><strong>Write a program to print </strong></li>
</ul>
<p>Einstein [0] = E</p>
<p>Einstein [1] = I</p>
<p>Einstein [2] = N</p>
<p>Einstein [3] = S</p>
<p>Einstein [4] = T</p>
<p>Einstein [5] = E</p>
<p>Einstein [6] = I</p>
<p>Einstein [7] = N</p>
<p><strong>using arrays</strong></p>
<p><strong>Answer:</strong></p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) throws Exception{</p>
<p>int i;</p>
<p>char [] num = {'E' , 'I', 'N', 'S', 'T', 'E', 'I', 'N'};</p>
<p>for(i=0; i&lt;8; i++)</p>
<p>System.out.println("Einstein [" + i + " ] = " + num[i]);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<ul>
<li><strong>What will be the output of the following programs?</strong></li>
</ul>
<p>i)</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) throws Exception{</p>
<p>int i;</p>
<p>int [] name = {'E' , 'I', 'N', 'S', 'T ', 'E', 'I', 'N'};</p>
<p>for(i=0; i&lt;8; i++)</p>
<p>System.out.println("Einstein [" +&nbsp; i + " ] = " + name[i]);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>Einstein [0] = 69</p>
<p>Einstein [1] = 73</p>
<p>Einstein [2] = 78</p>
<p>Einstein [3] = 83</p>
<p>Einstein [4] = 84</p>
<p>Einstein [5] = 69</p>
<p>Einstein [6] = 73</p>
<p>Einstein [7] = 78</p>
<p>&nbsp;</p>
<p>ii)</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String[] args) throws Exception{</p>
<p>int i;&nbsp;</p>
<p>char [] body&nbsp; = {'b', 'o', 'd', 'y'};</p>
<p>for(i=0; i&lt;4; i++)</p>
<p>System.out.println("body [" +&nbsp; body [i] + " ] = " + body [i]);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>body [b] = b</p>
<p>body [o] = o</p>
<p>body [d] = d</p>
<p>body [y] = y</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>//-------------------------------------------------------------------------------------------------------------------------------------</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>int x, y;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any Number: ");</p>
<p>x = scan.nextFloat();</p>
<p>System.out.print("Enter any Number: ");</p>
<p>y = scan.nextInt();</p>
<p>System.out.println(" square root of x = " + Math.sqrt(x));</p>
<p>System.out.println(" square root of y = " + Math.sqrt(y));</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>The output on the screen:</strong></p>
<p>Enter any Number:</p>
<p>If you enter the number 9</p>
<p>square root of x = 3</p>
<p>will be outputted on the screen.</p>
<p>Enter any Number:</p>
<p>If you enter the number 4</p>
<p>square root of y = 2</p>
<p>will be outputted on the screen.</p>
<p>&nbsp;</p>
<p>If&nbsp;</p>
<p>/*</p>
<p>&nbsp;</p>
<p>*/</p>
<p>&nbsp;</p>
<p>is introduced i.e., if the above program is rewritten as:</p>
<p>&nbsp;</p>
<p>import java.util.Scanner;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>int x, y;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any Number: ");</p>
<p>x = scan.nextInt();</p>
<p>/*</p>
<p>System.out.print("Enter any Number: ");</p>
<p>y = scan.nextInt();</p>
<p>*/</p>
<p>System.out.println(" square root of x = " + Math.sqrt(x));</p>
<p>/*</p>
<p>System.out.println(" square root of y = " + Math.sqrt(y));</p>
<p>*/</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Then the output on the screen is:</strong></p>
<p>Enter any Number:</p>
<p>If you enter the number 9</p>
<p>square root of x = 3</p>
<p>will be outputted on the screen.</p>
<p>----------------------------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;</p>
<ul>
<li><strong>What is the mistake in the following program:</strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<p>public class HelloWorld {</p>
<p>public static void main(String [] args) {</p>
<p>long float x;</p>
<p>Scanner scan = new Scanner(System.in);</p>
<p>System.out.print("Enter any Number: ");</p>
<p>x = scan.nextFloat();</p>
<p>System.out.println(" square root of x = " + Math.cbrt(x));</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Answer:</strong></p>
<p>long float x; should not be used -- only float x should be used because Java do not support the data type such as long int, long float etc.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Program 4.8</strong></p>
<p><strong>continue and break statements: </strong></p>
<p>A)</p>
<p>&nbsp;</p>
<p>public class HelloWorld{</p>
<p>public static void main(String []args){</p>
<p>int i;</p>
<p>for (i=1; i&lt;=5; i++){</p>
<p>if (i==3){</p>
<p>continue;</p>
<p>}</p>
<p>&nbsp;</p>
<p>System.out.println("" + i);</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>1</p>
<p>2</p>
<p>4</p>
<p>5</p>
<p>&nbsp;</p>
<p>B)</p>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String []args){</p>
<p>int i;</p>
<p>for (i=1; i&lt;=5; i++){</p>
<p>if (i==3){</p>
<p>break;</p>
<p>}</p>
<p>System.out.println("" + i);</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>1</p>
<p>2</p>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>What will be the output of the following program:</strong></li>
</ul>
<p>&nbsp;</p>
<p>public class HelloWorld {</p>
<p>public static void main(String args[]){</p>
<p>System.out.println(Math.max(1269, 1356));&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p><strong>Output on the screen:</strong></p>
<p>1356</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>//------------------------------------------------------------------------------------------------------------------------------------------&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>Abstraction</strong>&rarr; hiding implementation details from the user by providing interface</li>
<li><strong>Encapsulation</strong> &rarr; hiding data</li>
</ul>
<p>&nbsp;</p>
<p>In the statement:</p>
<p>"1 + 2"</p>
<p>"1" and "2" imply the <strong>operands</strong> and the plus symbol imply the <strong>operator</strong>.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Polymorphism </strong></li>
</ul>
<p>&nbsp;</p>
<p>Suppose if you are in class room that time you behave like a student, when you are in shopping mall at that time you behave like a customer, when you at your home at that time you behave like a son or daughter. Your ability to present in different-different behaviors is known as polymorphism.</p>
<p>&nbsp;</p>
<p>In the example:</p>
<p>&nbsp;</p>
<p>public class HelloWorld</p>
<p>{</p>
<p>public static void main(String [] args)</p>
<p>{</p>
<p>int a, b, sum;</p>
<p>a=1;</p>
<p>b=2;</p>
<p>sum = a + b;</p>
<p>System.out.println("the sum of a and b = " + sum);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>Plus symbol ("+") act as an arithmetic operator in the statement:</p>
<p>&nbsp;</p>
<p>sum = a+b;</p>
<p>and it act as the concatenation operator in the statement:</p>
<p>System.out.println("the sum of a and b = " + sum);</p>
<p>&nbsp;</p>
<p>The ability of plus symbol to behave both as arithmetic operator and concatenation operator is known as polymorphism.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>Inheritance </strong></li>
</ul>
<p>&nbsp;</p>
<p>public class game {</p>
<p>}</p>
<p>public class player extends game{</p>
<p>}</p>
<p>&nbsp;</p>
<p>Here public class player extends game implies:</p>
<p>class player is public and it is the sub class of the class game.</p>
<p>Since class player is the subclass of class game -- class player automatically takes on all the behavior and attributes of its parent class "game" i.e., methods&nbsp; or fields within the class game will be automatically be included in the class player.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Note:</strong></li>
</ul>
<p>&nbsp;</p>
<p>The statements:</p>
<p>&nbsp;</p>
<ul>
<li><strong>public class player extends game </strong></li>
</ul>
<p><strong>&nbsp;</strong></p>
<ul>
<li><strong>public class game extends ball</strong></li>
</ul>
<p>&nbsp;</p>
<p>implies: that class player is not only a subclass of class game but also it is a subclass of class ball.</p>
<p>&nbsp;</p>
<ul>
<li><strong>Encapsulation</strong></li>
</ul>
<p>public class Account {</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private decimal accountBalance = 500.00;</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public decimal CheckBalance() {</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return accountBalance;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /* accountBalance can be checked via public "CheckBalance" method provided by the "Account" class</p>
<p>but its value cannot be manipulated because data variable accountBalance is declared private */</p>
<p>&nbsp;</p>
<p>Encapsulation is the technique of bringing the data variables and methods in single frame and declaring data variable private (so it cannot be accessed by anyone outside the class, thereby hiding / encapsulating the data variable (String name) within the public class Student)&nbsp; and providing indirect access to the data variable via public methods.</p>
<p>&nbsp;</p>
<p>-----------------------------------------------------------------------------------------------------------------------------------------//</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<ul>
<li><strong>Comparison of C, C++ and Java </strong></li>
<li>C &amp; C++ support pointers and structures while Java do not.</li>
<li>The code of C and C++ are directly converted into machine level language and it is executed while the code of Java is converted into Java byte codes and then it is converted into machine level language and it is executed.</li>
<li>C uses scanf as input function to read the character or integer entered through the keyboard and printf as output function to print the output on the screen.</li>
<li>C++ uses cin as input function to read the character or integer entered through the keyboard and cout as output function to print the output on the screen.</li>
<li>But Java uses scan.nextInt() or scan.nextFloat() as input method to read the variable entered through the keyboard and System.out.println as output method to print the output on the screen.</li>
<li>Functions are in C &amp; C++ whereas methods are in Java.</li>
<li>C &amp; C++ are platform dependent whereas Java is platform independent (Code written in Java can be taken from one computer to the other without having to worry about system configuration details).</li>
<li>In C &amp; C++, program instruction codes are written and executed within the body of main function main() where as in Java -- program instruction codes are written and executed within the body of main method public static void main(String[] args).</li>
<li>data types like int float, char are same in C, C++ &amp; Java.</li>
<li>C is structured language whereas C++ &amp; Java is object oriented language (i.e., C++ &amp; Java has the extensive power and immense extensibility to write large scale complex programs).</li>
<li>Operators such as %d, %f &amp; %c are used in C whereas no operators are used in C++ &amp; Java.</li>
<li>A program written in Java usually requires more memory space than the same program written in C &amp; C++ and it is fast, reliable, and secure. According to Oracle, the company that owns Java, Java runs on 3 billion devices worldwide.</li>
<li>Java provides both high speed and high performance and reliability, flexibility and seamless integration with other frameworks and technologies -- compared to C &amp; C++.</li>
<li>Java is a popular general-purpose programming language and computing platform that supports multithreading (a process of executing several codes concurrently) while C &amp; C++ do not.</li>
<li>One of the reasons why Java is widely used is because of the availability of huge standard library that consists hundreds of classes and methods under different packages to help software developers.</li>
</ul>
<p><strong>For example:</strong></p>
<ul>
<li><strong>lang</strong>&rarr; for advanced features of strings, arrays etc.</li>
<li><strong>util</strong>&rarr; for data structures, regular expressions, date and time functions etc.</li>
<li><strong>io</strong>&rarr; for file i/o, exception handling etc.</li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong><u>The object oriented programming in Java</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p>The Java programming came in the midst of several programming languages which had object oriented features in their arsenal. Their were programming languages like smalltalk and C++ which were handling the object oriented programming. But, the idea was make programming easier, which could only be done by mounting up the piles of libraries of classes and function which could be used to solve complex programming problems.</p>
<p>The idea behind building a programming language was that every tool in the language has to be an object. As objects can be reliably used as different instances of the program adding up to the reuse of code and portability.</p>
<p>&nbsp;</p>
<p>The Object class is the base class of all the classes in Java. Let&rsquo;s go through some example of exception handling and files before diving into oriented programming in Java.</p>
<p>&nbsp;</p>
<p>The java.io package contains nearly every class you might ever need to perform input and output (I/O) in Java. All these streams represent an input source and an output destination. The stream in the java.io package supports many data such as primitives, object, localized characters, etc.</p>
<p>&nbsp;</p>
<h2>Stream</h2>
<p>A stream can be defined as a sequence of data. There are two kinds of Streams &minus;</p>
<ul>
<li><strong>InPutStream</strong>&minus; The InputStream is used to read data from a source.</li>
<li><strong>OutPutStream</strong>&minus; The OutputStream is used for writing data to a destination.</li>
</ul>
<p>Java provides strong but flexible support for I/O related to files and networks but this tutorial covers very basic functionality related to streams and I/O. We will see the most commonly used examples one by one &minus;</p>
<h3>Byte Streams</h3>
<p>Java byte streams are used to perform input and output of 8-bit bytes. Though there are many classes related to byte streams but the most frequently used classes are, <strong><u>FileInputStream </u></strong>and <strong><u>FileOutputStream</u></strong>. Following is an example which makes use of these two classes to copy an input file into an output file &minus;</p>
<p>import java.io.*; // This library is required to execute I/O operations on files.</p>
<p>publicclassCopyFile{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[])throwsIOException{</p>
<p>FileInputStreamin=null;</p>
<p>FileOutputStreamout=null;</p>
<p>&nbsp;</p>
<p>try{</p>
<p>in=newFileInputStream("input.txt");</p>
<p>out=newFileOutputStream("output.txt");</p>
<p>&nbsp;</p>
<p>int c;</p>
<p>while((c =in.read())!=-1){</p>
<p>out.write(c);</p>
<p>}</p>
<p>}finally{</p>
<p>if(in!=null){</p>
<p>in.close();</p>
<p>}</p>
<p>if(out!=null){</p>
<p>out.close();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>Now let's have a file <strong><u>input.txt</u></strong>with the following content &minus;</p>
<p>This is test for copy file.</p>
<p>As a next step, compile the above program and execute it, which will result in creating output.txt file with the same content as we have in input.txt. So let's put the above code in CopyFile.java file and do the following &minus;</p>
<p>$javac CopyFile.java</p>
<p>$java CopyFile</p>
<h3>Character Streams</h3>
<p>Java&nbsp;<strong>Byte</strong>&nbsp;streams are used to perform input and output of 8-bit bytes, whereas Java&nbsp;<strong>Character</strong>&nbsp;streams are used to perform input and output for 16-bit unicode. Though there are many classes related to character streams but the most frequently used classes are, <strong><u>FileReader</u></strong>and <strong><u>FileWriter</u></strong>. Though internally FileReader uses FileInputStream and FileWriter uses FileOutputStream but here the major difference is that FileReader reads two bytes at a time and FileWriter writes two bytes at a time.</p>
<p>We can re-write the above example, which makes the use of these two classes to copy an input file (having unicode characters) into an output file &minus;</p>
<p><strong>Example</strong></p>
<p>import java.io.*;</p>
<p>publicclassCopyFile{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[])throwsIOException{</p>
<p>FileReaderin=null;</p>
<p>FileWriterout=null;</p>
<p>&nbsp;</p>
<p>try{</p>
<p>in=newFileReader("input.txt");</p>
<p>out=newFileWriter("output.txt");</p>
<p>&nbsp;</p>
<p>int c;</p>
<p>while((c =in.read())!=-1){</p>
<p>out.write(c);</p>
<p>}</p>
<p>}finally{</p>
<p>if(in!=null){</p>
<p>in.close();</p>
<p>}</p>
<p>if(out!=null){</p>
<p>out.close();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>Now let's have a file <strong><u>input.txt</u></strong>with the following content &minus;</p>
<p>This is test for copy file.</p>
<p>As a next step, compile the above program and execute it, which will result in creating output.txt file with the same content as we have in input.txt. So let's put the above code in CopyFile.java file and do the following &minus;</p>
<p>$javac CopyFile.java</p>
<p>$java CopyFile</p>
<h2>Standard Streams</h2>
<p>All the programming languages provide support for standard I/O where the user's program can take input from a keyboard and then produce an output on the computer screen. If you are aware of C or C++ programming languages, then you must be aware of three standard devices STDIN, STDOUT and STDERR. Similarly, Java provides the following three standard streams &minus;</p>
<ul>
<li><strong>Standard Input </strong>&minus; This is used to feed the data to user's program and usually a keyboard is used as standard input stream and represented as <strong><u>in</u></strong>.</li>
<li><strong>Standard Output </strong>&minus; This is used to output the data produced by the user's program and usually a computer screen is used for standard output stream and represented as <strong>out</strong>.</li>
<li><strong>Standard Error </strong>&minus; This is used to output the error data produced by the user's program and usually a computer screen is used for standard error stream and represented as <strong><u>err</u></strong>.</li>
</ul>
<p>Following is a simple program, which creates <strong><u>InputStreamReader</u></strong>to read standard input stream until the user types a "q" &minus;</p>
<p><strong><u>Example</u></strong></p>
<p><u>import</u><u> java</u><u>.</u><u>io</u><u>.*;</u></p>
<p>publicclassReadConsole{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[])throwsIOException{</p>
<p>InputStreamReader cin =null;</p>
<p>&nbsp;</p>
<p>try{</p>
<p>cin =newInputStreamReader(System.in);</p>
<p>System.out.println("Enter characters, 'q' to quit.");</p>
<p>char c;</p>
<p>do{</p>
<p>c =(char) cin.read();</p>
<p>System.out.print(c);</p>
<p>}while(c !='q');</p>
<p>}finally{</p>
<p>if(cin !=null){</p>
<p>cin.close();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>Let's keep the above code in ReadConsole.java file and try to compile and execute it as shown in the following program. This program continues to read and output the same character until we press 'q' &minus;</p>
<p>$javac ReadConsole.java</p>
<p>$java ReadConsole</p>
<p>Enter characters, 'q' to quit.</p>
<p>1</p>
<p>1</p>
<p>e</p>
<p>e</p>
<p>q</p>
<p>q</p>
<h2>Reading and Writing Files</h2>
<p>As described earlier, a stream can be defined as a sequence of data. The <strong>InputStream </strong>is used to read data from a source and the <strong>OutputStream </strong>is used for writing data to a destination.</p>
<p>Here is a hierarchy of classes to deal with Input and Output streams.</p>
<p>The two important streams are&nbsp;<strong>FileInputStream</strong>&nbsp;and&nbsp;<strong>FileOutputStream</strong>, which would be discussed in this tutorial.</p>
<h3>FileInputStream</h3>
<p>This stream is used for reading data from the files. Objects can be created using the keyword&nbsp;<strong>new</strong>&nbsp;and there are several types of constructors available.</p>
<p>Following constructor takes a file name as a string to create an input stream object to read the file &minus;</p>
<p>InputStream f = new FileInputStream("C:/java/hello");</p>
<p>Following constructor takes a file object to create an input stream object to read the file. First we create a file object using File() method as follows &minus;</p>
<p>File f = new File("C:/java/hello");</p>
<p>InputStream f = new FileInputStream(f);</p>
<p>Once you have&nbsp;<em>InputStream</em>&nbsp;object in hand, then there is a list of helper methods which can be used to read to stream or to do other operations on the stream.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>public void close() throws IOException{}</strong></p>
<p>This method closes the file output stream. Releases any system resources associated with the file. Throws an IOException.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>protected void finalize()throws IOException {}</strong></p>
<p>This method cleans up the connection to the file. Ensures that the close method of this file output stream is called when there are no more references to this stream. Throws an IOException.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>public int read(int r)throws IOException{}</strong></p>
<p>This method reads the specified byte of data from the InputStream. Returns an int. Returns the next byte of data and -1 will be returned if it's the end of the file.</p>
</td>
</tr>
<tr>
<td width="51">
<p>4</p>
</td>
<td width="573">
<p><strong>public int read(byte[] r) throws IOException{}</strong></p>
<p>This method reads r.length bytes from the input stream into an array. Returns the total number of bytes read. If it is the end of the file, -1 will be returned.</p>
</td>
</tr>
<tr>
<td width="51">
<p>5</p>
</td>
<td width="573">
<p><strong>public int available() throws IOException{}</strong></p>
<p>Gives the number of bytes that can be read from this file input stream. Returns an int.</p>
</td>
</tr>
</tbody>
</table>
<p>There are other important input streams available, for more detail you can refer to the following links &minus;</p>
<ul>
<li><a href="https://www.tutorialspoint.com/java/java_bytearrayinputstream.htm">ByteArrayInputStream</a></li>
<li><a href="https://www.tutorialspoint.com/java/java_datainputstream.htm">DataInputStream</a></li>
</ul>
<h2>FileOutputStream</h2>
<p>FileOutputStream is used to create a file and write data into it. The stream would create a file, if it doesn't already exist, before opening it for output.</p>
<p>Here are two constructors which can be used to create a FileOutputStream object.</p>
<p>Following constructor takes a file name as a string to create an input stream object to write the file &minus;</p>
<p>OutputStream f = new FileOutputStream("C:/java/hello")</p>
<p>Following constructor takes a file object to create an output stream object to write the file. First, we create a file object using File() method as follows &minus;</p>
<p>File f = new File("C:/java/hello");</p>
<p>OutputStream f = new FileOutputStream(f);</p>
<p>Once you have&nbsp;<em>OutputStream</em>&nbsp;object in hand, then there is a list of helper methods, which can be used to write to stream or to do other operations on the stream.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>public void close() throws IOException{}</strong></p>
<p>This method closes the file output stream. Releases any system resources associated with the file. Throws an IOException.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>protected void finalize()throws IOException {}</strong></p>
<p>This method cleans up the connection to the file. Ensures that the close method of this file output stream is called when there are no more references to this stream. Throws an IOException.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>public void write(int w)throws IOException{}</strong></p>
<p>This methods writes the specified byte to the output stream.</p>
</td>
</tr>
<tr>
<td width="51">
<p>4</p>
</td>
<td width="573">
<p><strong>public void write(byte[] w)</strong></p>
<p>Writes w.length bytes from the mentioned byte array to the OutputStream.</p>
</td>
</tr>
</tbody>
</table>
<p>There are other important output streams available, for more detail you can refer to the following links &minus;</p>
<ul>
<li><a href="https://www.tutorialspoint.com/java/java_bytearrayoutputstream.htm">ByteArrayOutputStream</a></li>
<li><a href="https://www.tutorialspoint.com/java/java_dataoutputstream.htm">DataOutputStream</a></li>
</ul>
<p><strong>Example</strong></p>
<p>Following is the example to demonstrate InputStream and OutputStream &minus;</p>
<p>import java.io.*;</p>
<p>publicclass fileStreamTest {</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>&nbsp;</p>
<p>try{</p>
<p>byte bWrite []={11,21,3,40,5};</p>
<p>OutputStream os =newFileOutputStream("test.txt");</p>
<p>for(int x =0; x &lt; bWrite.length ; x++){</p>
<p>os.write( bWrite[x]);// writes the bytes</p>
<p>}</p>
<p>os.close();</p>
<p>&nbsp;</p>
<p>InputStreamis=newFileInputStream("test.txt");</p>
<p>int size =is.available();</p>
<p>&nbsp;</p>
<p>for(int i =0; i &lt; size; i++){</p>
<p>System.out.print((char)is.read()+"");</p>
<p>}</p>
<p>is.close();</p>
<p>}catch(IOException e){</p>
<p>System.out.print("Exception");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>The above code would create file test.txt and would write given numbers in binary format. Same would be the output on the stdout screen.</p>
<h2><u>File Navigation and I/O</u></h2>
<p>There are several other classes that we would be going through to get to know the basics of File Navigation and I/O.</p>
<h1><u>Java - File Class</u></h1>
<p>Java File class represents the files and directory pathnames in an abstract manner. This class is used for creation of files and directories, file searching, file deletion, etc.</p>
<p>The File object represents the actual file/directory on the disk. Following is the list of constructors to create a File object.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>File(File parent, String child)</strong></p>
<p>This constructor creates a new File instance from a parent abstract pathname and a child pathname string.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>File(String pathname)</strong></p>
<p>This constructor creates a new File instance by converting the given pathname string into an abstract pathname.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>File(String parent, String child)</strong></p>
<p>This constructor creates a new File instance from a parent pathname string and a child pathname string.</p>
</td>
</tr>
<tr>
<td width="51">
<p>4</p>
</td>
<td width="573">
<p><strong>File(URI uri)</strong></p>
<p>This constructor creates a new File instance by converting the given file: URI into an abstract pathname.</p>
</td>
</tr>
</tbody>
</table>
<p>Once you have&nbsp;<em>File</em>&nbsp;object in hand, then there is a list of helper methods which can be used to manipulate the files.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>public String getName()</strong></p>
<p>Returns the name of the file or directory denoted by this abstract pathname.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>public String getParent()</strong></p>
<p>Returns the pathname string of this abstract pathname's parent, or null if this pathname does not name a parent directory.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>public File getParentFile()</strong></p>
<p>Returns the abstract pathname of this abstract pathname's parent, or null if this pathname does not name a parent directory.</p>
</td>
</tr>
<tr>
<td width="51">
<p>4</p>
</td>
<td width="573">
<p><strong>public String getPath()</strong></p>
<p>Converts this abstract pathname into a pathname string.</p>
</td>
</tr>
<tr>
<td width="51">
<p>5</p>
</td>
<td width="573">
<p><strong>public boolean isAbsolute()</strong></p>
<p>Tests whether this abstract pathname is absolute. Returns true if this abstract pathname is absolute, false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>6</p>
</td>
<td width="573">
<p><strong>public String getAbsolutePath()</strong></p>
<p>Returns the absolute pathname string of this abstract pathname.</p>
</td>
</tr>
<tr>
<td width="51">
<p>7</p>
</td>
<td width="573">
<p><strong>public boolean canRead()</strong></p>
<p>Tests whether the application can read the file denoted by this abstract pathname. Returns true if and only if the file specified by this abstract pathname exists and can be read by the application; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>8</p>
</td>
<td width="573">
<p><strong>public boolean canWrite()</strong></p>
<p>Tests whether the application can modify to the file denoted by this abstract pathname. Returns true if and only if the file system actually contains a file denoted by this abstract pathname and the application is allowed to write to the file; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>9</p>
</td>
<td width="573">
<p><strong>public boolean exists()</strong></p>
<p>Tests whether the file or directory denoted by this abstract pathname exists. Returns true if and only if the file or directory denoted by this abstract pathname exists; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>10</p>
</td>
<td width="573">
<p><strong>public boolean isDirectory()</strong></p>
<p>Tests whether the file denoted by this abstract pathname is a directory. Returns true if and only if the file denoted by this abstract pathname exists and is a directory; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>11</p>
</td>
<td width="573">
<p><strong>public boolean isFile()</strong></p>
<p>Tests whether the file denoted by this abstract pathname is a normal file. A file is normal if it is not a directory and, in addition, satisfies other system-dependent criteria. Any non-directory file created by a Java application is guaranteed to be a normal file. Returns true if and only if the file denoted by this abstract pathname exists and is a normal file; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>12</p>
</td>
<td width="573">
<p><strong>public long lastModified()</strong></p>
<p>Returns the time that the file denoted by this abstract pathname was last modified. Returns a long value representing the time the file was last modified, measured in milliseconds since the epoch (00:00:00 GMT, January 1, 1970), or 0L if the file does not exist or if an I/O error occurs.</p>
</td>
</tr>
<tr>
<td width="51">
<p>13</p>
</td>
<td width="573">
<p><strong>public long length()</strong></p>
<p>Returns the length of the file denoted by this abstract pathname. The return value is unspecified if this pathname denotes a directory.</p>
</td>
</tr>
<tr>
<td width="51">
<p>14</p>
</td>
<td width="573">
<p><strong>public boolean createNewFile() throws IOException</strong></p>
<p>Atomically creates a new, empty file named by this abstract pathname if and only if a file with this name does not yet exist. Returns true if the named file does not exist and was successfully created; false if the named file already exists.</p>
</td>
</tr>
<tr>
<td width="51">
<p>15</p>
</td>
<td width="573">
<p><strong>public boolean delete()</strong></p>
<p>Deletes the file or directory denoted by this abstract pathname. If this pathname denotes a directory, then the directory must be empty in order to be deleted. Returns true if and only if the file or directory is successfully deleted; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>16</p>
</td>
<td width="573">
<p><strong>public void deleteOnExit()</strong></p>
<p>Requests that the file or directory denoted by this abstract pathname be deleted when the virtual machine terminates.</p>
</td>
</tr>
<tr>
<td width="51">
<p>17</p>
</td>
<td width="573">
<p><strong>public String[] list()</strong></p>
<p>Returns an array of strings naming the files and directories in the directory denoted by this abstract pathname.</p>
</td>
</tr>
<tr>
<td width="51">
<p>18</p>
</td>
<td width="573">
<p><strong>public String[] list(FilenameFilter filter)</strong></p>
<p>Returns an array of strings naming the files and directories in the directory denoted by this abstract pathname that satisfy the specified filter.</p>
</td>
</tr>
<tr>
<td width="51">
<p>20</p>
</td>
<td width="573">
<p><strong>public File[] listFiles()</strong></p>
<p>Returns an array of abstract pathnames denoting the files in the directory denoted by this abstract pathname.</p>
</td>
</tr>
<tr>
<td width="51">
<p>21</p>
</td>
<td width="573">
<p><strong>public File[] listFiles(FileFilter filter)</strong></p>
<p>Returns an array of abstract pathnames denoting the files and directories in the directory denoted by this abstract pathname that satisfy the specified filter.</p>
</td>
</tr>
<tr>
<td width="51">
<p>22</p>
</td>
<td width="573">
<p><strong>public boolean mkdir()</strong></p>
<p>Creates the directory named by this abstract pathname. Returns true if and only if the directory was created; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>23</p>
</td>
<td width="573">
<p><strong>public boolean mkdirs()</strong></p>
<p>Creates the directory named by this abstract pathname, including any necessary but nonexistent parent directories. Returns true if and only if the directory was created, along with all necessary parent directories; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>24</p>
</td>
<td width="573">
<p><strong>public boolean renameTo(File dest)</strong></p>
<p>Renames the file denoted by this abstract pathname. Returns true if and only if the renaming succeeded; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>25</p>
</td>
<td width="573">
<p><strong>public boolean setLastModified(long time)</strong></p>
<p>Sets the last-modified time of the file or directory named by this abstract pathname. Returns true if and only if the operation succeeded; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>26</p>
</td>
<td width="573">
<p><strong>public boolean setReadOnly()</strong></p>
<p>Marks the file or directory named by this abstract pathname so that only read operations are allowed. Returns true if and only if the operation succeeded; false otherwise.</p>
</td>
</tr>
<tr>
<td width="51">
<p>27</p>
</td>
<td width="573">
<p><strong>public static File createTempFile(String prefix, String suffix, File directory) throws IOException</strong></p>
<p>Creates a new empty file in the specified directory, using the given prefix and suffix strings to generate its name. Returns an abstract pathname denoting a newly-created empty file.</p>
</td>
</tr>
<tr>
<td width="51">
<p>28</p>
</td>
<td width="573">
<p><strong>public static File createTempFile(String prefix, String suffix) throws IOException</strong></p>
<p>Creates an empty file in the default temporary-file directory, using the given prefix and suffix to generate its name. Invoking this method is equivalent to invoking createTempFile(prefix, suffix, null). Returns abstract pathname denoting a newly-created empty file.</p>
</td>
</tr>
<tr>
<td width="51">
<p>29</p>
</td>
<td width="573">
<p><strong>public int compareTo(File pathname)</strong></p>
<p>Compares two abstract pathnames lexicographically. Returns zero if the argument is equal to this abstract pathname, a value less than zero if this abstract pathname is lexicographically less than the argument, or a value greater than zero if this abstract pathname is lexicographically greater than the argument.</p>
</td>
</tr>
<tr>
<td width="51">
<p>30</p>
</td>
<td width="573">
<p><strong>public int compareTo(Object o)</strong></p>
<p>Compares this abstract pathname to another object. Returns zero if the argument is equal to this abstract pathname, a value less than zero if this abstract pathname is lexicographically less than the argument, or a value greater than zero if this abstract pathname is lexicographically greater than the argument.</p>
</td>
</tr>
<tr>
<td width="51">
<p>31</p>
</td>
<td width="573">
<p><strong>public boolean equals(Object obj)</strong></p>
<p>Tests this abstract pathname for equality with the given object. Returns true if and only if the argument is not null and is an abstract pathname that denotes the same file or directory as this abstract pathname.</p>
</td>
</tr>
<tr>
<td width="51">
<p>32</p>
</td>
<td width="573">
<p><strong>public String toString()</strong></p>
<p>Returns the pathname string of this abstract pathname. This is just the string returned by the getPath() method.</p>
</td>
</tr>
</tbody>
</table>
<h2><u>Example</u></h2>
<p>Following is an example to demonstrate File object &minus;</p>
<p>import java.io.File;</p>
<p>publicclassFileDemo{</p>
<p>publicstaticvoid main(String[] args){</p>
<p>File f =null;</p>
<p>String[] strs ={"test1.txt","test2.txt"};</p>
<p>try{</p>
<p>// for each string in string array</p>
<p>for(String s:strs ){</p>
<p>// create new file</p>
<p>f =newFile(s);</p>
<p>// true if the file is executable</p>
<p>booleanbool= f.canExecute();</p>
<p>// find the absolute path</p>
<p>String a = f.getAbsolutePath();</p>
<p>// prints absolute path</p>
<p>System.out.print(a);</p>
<p>// prints</p>
<p>System.out.println(" is executable: "+bool);</p>
<p>}</p>
<p>}catch(Exception e){</p>
<p>// if any I/O error occurs</p>
<p>e.printStackTrace();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>Consider there is an executable file test1.txt and another file test2.txt is non executable in the current directory. Let us compile and run the above program, This will produce the following result &minus;</p>
<h2><u>Output</u></h2>
<p>/home/cg/root/2880380/test1.txt is executable: false</p>
<p>/home/cg/root/2880380/test2.txt is executable: false</p>
<h1><u>Java - FileReader Class</u></h1>
<p><u>This class inherits from the InputStreamReader class. FileReader is used for reading streams of characters.</u></p>
<p>This class has several constructors to create required objects. Following is the list of constructors provided by the FileReader class.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Constructor &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>FileReader(File file)</strong></p>
<p>This constructor creates a new FileReader, given the File to read from.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>FileReader(FileDescriptor fd)</strong></p>
<p>This constructor creates a new FileReader, given the FileDescriptor to read from.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>FileReader(String fileName)</strong></p>
<p>This constructor creates a new FileReader, given the name of the file to read from.</p>
</td>
</tr>
</tbody>
</table>
<p>Once you have FileReader object in hand then there is a list of helper methods which can be used to manipulate the files.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>public int read() throws IOException</strong></p>
<p>Reads a single character. Returns an int, which represents the character read.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>public int read(char [] c, int offset, int len)</strong></p>
<p>Reads characters into an array. Returns the number of characters read.</p>
</td>
</tr>
</tbody>
</table>
<p><br /> <strong><u>Example</u></strong></p>
<p>Following is an example to demonstrate class &minus;</p>
<p>import java.io.*;</p>
<p>publicclassFileRead{</p>
<p>publicstaticvoid main(String args[])throwsIOException{</p>
<p>File file =newFile("Hello1.txt");</p>
<p>// creates the file</p>
<p>file.createNewFile();</p>
<p>// creates a FileWriter Object</p>
<p>FileWriter writer =newFileWriter(file);</p>
<p>// Writes the content to the file</p>
<p>writer.write("This\n is\n an\n example\n");</p>
<p>writer.flush();</p>
<p>writer.close();</p>
<p>// Creates a FileReader Object</p>
<p>FileReader fr =newFileReader(file);</p>
<p>char[] a =newchar[50];</p>
<p>fr.read(a);// reads the content to the array</p>
<p>for(char c : a)</p>
<p>System.out.print(c);// prints the characters one by one</p>
<p>fr.close();</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h2>Output</h2>
<p>This</p>
<p>is</p>
<p>an</p>
<p>example</p>
<h1><u>Java - FileWriter Class</u></h1>
<p>This class inherits from the OutputStreamWriter class. The class is used for writing streams of characters.</p>
<p>This class has several constructors to create required objects. Following is a list.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Constructor &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>FileWriter(File file)</strong></p>
<p>This constructor creates a FileWriter object given a File object.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>FileWriter(File file, boolean append)</strong></p>
<p>This constructor creates a FileWriter object given a File object with a boolean indicating whether or not to append the data written.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>FileWriter(FileDescriptor fd)</strong></p>
<p>This constructor creates a FileWriter object associated with the given file descriptor.</p>
</td>
</tr>
<tr>
<td width="51">
<p>4</p>
</td>
<td width="573">
<p><strong>FileWriter(String fileName)</strong></p>
<p>This constructor creates a FileWriter object, given a file name.</p>
</td>
</tr>
<tr>
<td width="51">
<p>5</p>
</td>
<td width="573">
<p><strong>FileWriter(String fileName, boolean append)</strong></p>
<p>This constructor creates a FileWriter object given a file name with a boolean indicating whether or not to append the data written.</p>
</td>
</tr>
</tbody>
</table>
<p>Once you have&nbsp;<em>FileWriter</em>&nbsp;object in hand, then there is a list of helper methods, which can be used to manipulate the files.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>public void write(int c) throws IOException</strong></p>
<p>Writes a single character.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>public void write(char [] c, int offset, int len)</strong></p>
<p>Writes a portion of an array of characters starting from offset and with a length of len.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>public void write(String s, int offset, int len)</strong></p>
<p>Write a portion of a String starting from offset and with a length of len.</p>
</td>
</tr>
</tbody>
</table>
<p><br /> Example</p>
<p>Following is an example to demonstrate class &minus;</p>
<p>import java.io.*;</p>
<p>publicclassFileRead{</p>
<p>publicstaticvoid main(String args[])throwsIOException{</p>
<p>File file =newFile("Hello1.txt");</p>
<p>// creates the file</p>
<p>file.createNewFile();</p>
<p>// creates a FileWriter Object</p>
<p>FileWriter writer =newFileWriter(file);</p>
<p>// Writes the content to the file</p>
<p>writer.write("This\n is\n an\n example\n");</p>
<p>writer.flush();</p>
<p>writer.close();</p>
<p>// Creates a FileReader Object</p>
<p>FileReader fr =newFileReader(file);</p>
<p>char[] a =newchar[50];</p>
<p>fr.read(a);// reads the content to the array</p>
<p>for(char c : a)</p>
<p>System.out.print(c);// prints the characters one by one</p>
<p>fr.close();</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h2><u>Output</u></h2>
<p>This</p>
<p>is</p>
<p>an</p>
<p>example</p>
<p>&nbsp;</p>
<h1><u>Java &ndash; Exceptions</u></h1>
<p>An exception (or exceptional event) is a problem that arises during the execution of a program. When an&nbsp;<strong>Exception</strong>&nbsp;occurs the normal flow of the program is disrupted and the program/Application terminates abnormally, which is not recommended, therefore, these exceptions are to be handled.</p>
<p>An exception can occur for many different reasons. Following are some scenarios where an exception occurs.</p>
<ul>
<li>A user has entered an invalid data.</li>
<li>A file that needs to be opened cannot be found.</li>
<li>A network connection has been lost in the middle of communications or the JVM has run out of memory.</li>
</ul>
<p>Some of these exceptions are caused by user error, others by programmer error, and others by physical resources that have failed in some manner.</p>
<p>Based on these, we have three categories of Exceptions. You need to understand them to know how exception handling works in Java.</p>
<ul>
<li><strong>Checked exceptions </strong>&minus; A checked exception is an exception that occurs at the compile time, these are also called as compile time exceptions. These exceptions cannot simply be ignored at the time of compilation, the programmer should take care of (handle) these exceptions.</li>
</ul>
<p>For example, if you use <strong>FileReader </strong>class in your program to read data from a file, if the file specified in its constructor doesn't exist, then a <em>FileNotFoundException </em>occurs, and the compiler prompts the programmer to handle the exception.</p>
<h3><u>Example</u></h3>
<p><u>import</u><u> java</u><u>.</u><u>io</u><u>.</u><u>File</u><u>;</u></p>
<p>import java.io.FileReader;</p>
<p>publicclassFilenotFound_Demo{</p>
<p>publicstaticvoid main(String args[]){</p>
<p>File file =newFile("E://file.txt");</p>
<p>FileReader fr =newFileReader(file);</p>
<p>}</p>
<p>}</p>
<p>If you try to compile the above program, you will get the following exceptions.</p>
<h3><u>Output</u></h3>
<p>C:\&gt;javac FilenotFound_Demo.java</p>
<p>FilenotFound_Demo.java:8: error: unreported exception FileNotFoundException; must be caught or declared to be thrown</p>
<p>FileReader fr = new FileReader(file);</p>
<p>^</p>
<p>1 error</p>
<p><strong>Note </strong>&minus; Since the methods <strong>read() </strong>and <strong>close() </strong>of FileReader class throws IOException, you can observe that the compiler notifies to handle IOException, along with FileNotFoundException.</p>
<ul>
<li><strong>Unchecked exceptions </strong>&minus; An unchecked exception is an exception that occurs at the time of execution. These are also called as <strong>Runtime Exceptions</strong>. These include programming bugs, such as logic errors or improper use of an API. Runtime exceptions are ignored at the time of compilation.</li>
</ul>
<p>For example, if you have declared an array of size 5 in your program, and trying to call the 6<sup>th</sup> element of the array then an <em>ArrayIndexOutOfBoundsExceptionexception </em>occurs.</p>
<h3><u>Example</u></h3>
<p><u>publicclass</u><u>Unchecked_Demo</u><u>{</u></p>
<p>publicstaticvoid main(String args[]){</p>
<p>int num[]={1,2,3,4};</p>
<p>System.out.println(num[5]);</p>
<p>}</p>
<p>}</p>
<p>If you compile and execute the above program, you will get the following exception.</p>
<h3><u>Output</u></h3>
<p>Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException: 5</p>
<p>at Exceptions.Unchecked_Demo.main(Unchecked_Demo.java:8)</p>
<ul>
<li><strong>Errors </strong>&minus; These are not exceptions at all, but problems that arise beyond the control of the user or the programmer. Errors are typically ignored in your code because you can rarely do anything about an error. For example, if a stack overflow occurs, an error will arise. They are also ignored at the time of compilation.</li>
</ul>
<h2>Exception Hierarchy</h2>
<p>All exception classes are subtypes of the java.lang.Exception class. The exception class is a subclass of the Throwable class. Other than the exception class there is another subclass called Error which is derived from the Throwable class.</p>
<p>Errors are abnormal conditions that happen in case of severe failures, these are not handled by the Java programs. Errors are generated to indicate errors generated by the runtime environment. Example: JVM is out of memory. Normally, programs cannot recover from errors.</p>
<p>The Exception class has two main subclasses: IOException class and RuntimeException Class.</p>
<p>Following is a list of most common checked and unchecked&nbsp;<a href="https://www.tutorialspoint.com/java/java_builtin_exceptions.htm">Java's Built-in Exceptions</a>.</p>
<h2>Exceptions Methods</h2>
<p>Following is the list of important methods available in the Throwable class.</p>
<table width="624">
<tbody>
<tr>
<td width="51">
<p>Sr.No.</p>
</td>
<td width="573">
<p>Method &amp; Description</p>
</td>
</tr>
<tr>
<td width="51">
<p>1</p>
</td>
<td width="573">
<p><strong>public String getMessage()</strong></p>
<p>Returns a detailed message about the exception that has occurred. This message is initialized in the Throwable constructor.</p>
</td>
</tr>
<tr>
<td width="51">
<p>2</p>
</td>
<td width="573">
<p><strong>public Throwable getCause()</strong></p>
<p>Returns the cause of the exception as represented by a Throwable object.</p>
</td>
</tr>
<tr>
<td width="51">
<p>3</p>
</td>
<td width="573">
<p><strong>public String toString()</strong></p>
<p>Returns the name of the class concatenated with the result of getMessage().</p>
</td>
</tr>
<tr>
<td width="51">
<p>4</p>
</td>
<td width="573">
<p><strong>public void printStackTrace()</strong></p>
<p>Prints the result of toString() along with the stack trace to System.err, the error output stream.</p>
</td>
</tr>
<tr>
<td width="51">
<p>5</p>
</td>
<td width="573">
<p><strong>public StackTraceElement [] getStackTrace()</strong></p>
<p>Returns an array containing each element on the stack trace. The element at index 0 represents the top of the call stack, and the last element in the array represents the method at the bottom of the call stack.</p>
</td>
</tr>
<tr>
<td width="51">
<p>6</p>
</td>
<td width="573">
<p><strong>public Throwable fillInStackTrace()</strong></p>
<p>Fills the stack trace of this Throwable object with the current stack trace, adding to any previous information in the stack trace.</p>
</td>
</tr>
</tbody>
</table>
<h2>Catching Exceptions</h2>
<p>A method catches an exception using a combination of the <strong>try </strong>and <strong>catch </strong>keywords. A try/catch block is placed around the code that might generate an exception. Code within a try/catch block is referred to as protected code, and the syntax for using try/catch looks like the following &minus;</p>
<h3><u>Syntax</u></h3>
<p>try {</p>
<p>// Protected code</p>
<p>} catch (ExceptionName e1) {</p>
<p>// Catch block</p>
<p>}</p>
<p>The code which is prone to exceptions is placed in the try block. When an exception occurs, that exception occurred is handled by catch block associated with it. Every try block should be immediately followed either by a catch block or finally block.</p>
<p>A catch statement involves declaring the type of exception you are trying to catch. If an exception occurs in protected code, the catch block (or blocks) that follows the try is checked. If the type of exception that occurred is listed in a catch block, the exception is passed to the catch block much as an argument is passed into a method parameter.</p>
<h3><u>Example</u></h3>
<p>The following is an array declared with 2 elements. Then the code tries to access the 3<sup>rd</sup> element of the array which throws an exception.</p>
<p>// File Name : ExcepTest.java</p>
<p>import java.io.*;</p>
<p>&nbsp;</p>
<p>publicclassExcepTest{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>try{</p>
<p>int a[]=newint[2];</p>
<p>System.out.println("Access element three :"+ a[3]);</p>
<p>}catch(ArrayIndexOutOfBoundsException e){</p>
<p>System.out.println("Exception thrown&nbsp; :"+ e);</p>
<p>}</p>
<p>System.out.println("Out of the block");</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Exception thrown&nbsp; :java.lang.ArrayIndexOutOfBoundsException: 3</p>
<p>Out of the block</p>
<h2>Multiple Catch Blocks</h2>
<p>A try block can be followed by multiple catch blocks. The syntax for multiple catch blocks looks like the following &minus;</p>
<h3>Syntax</h3>
<p>try {</p>
<p>// Protected code</p>
<p>} catch (ExceptionType1 e1) {</p>
<p>// Catch block</p>
<p>} catch (ExceptionType2 e2) {</p>
<p>// Catch block</p>
<p>} catch (ExceptionType3 e3) {</p>
<p>// Catch block</p>
<p>}</p>
<p>The previous statements demonstrate three catch blocks, but you can have any number of them after a single try. If an exception occurs in the protected code, the exception is thrown to the first catch block in the list. If the data type of the exception thrown matches ExceptionType1, it gets caught there. If not, the exception passes down to the second catch statement. This continues until the exception either is caught or falls through all catches, in which case the current method stops execution and the exception is thrown down to the previous method on the call stack.</p>
<h3>Example</h3>
<p>Here is code segment showing how to use multiple try/catch statements.</p>
<p>try{</p>
<p>file =newFileInputStream(fileName);</p>
<p>x =(byte) file.read();</p>
<p>}catch(IOException i){</p>
<p>i.printStackTrace();</p>
<p>return-1;</p>
<p>}catch(FileNotFoundException f)// Not valid! {</p>
<p>f.printStackTrace();</p>
<p>return-1;</p>
<p>}</p>
<h2>Catching Multiple Type of Exceptions</h2>
<p>Since Java 7, you can handle more than one exception using a single catch block, this feature simplifies the code. Here is how you would do it &minus;</p>
<p>catch (IOException|FileNotFoundException ex) {</p>
<p>logger.log(ex);</p>
<p>throw ex;</p>
<h2>The Throws/Throw Keywords</h2>
<p>If a method does not handle a checked exception, the method must declare it using the&nbsp;<strong>throws</strong>&nbsp;keyword. The throws keyword appears at the end of a method's signature.</p>
<p>You can throw an exception, either a newly instantiated one or an exception that you just caught, by using the&nbsp;<strong>throw</strong>&nbsp;keyword.</p>
<p>Try to understand the difference between throws and throw keywords,&nbsp;<em>throws</em>is used to postpone the handling of a checked exception and&nbsp;<em>throw</em>&nbsp;is used to invoke an exception explicitly.</p>
<p>The following method declares that it throws a RemoteException &minus;</p>
<h3>Example</h3>
<p>import java.io.*;</p>
<p>publicclass className {</p>
<p>&nbsp;</p>
<p>publicvoid deposit(double amount)throwsRemoteException{</p>
<p>// Method implementation</p>
<p>thrownewRemoteException();</p>
<p>}</p>
<p>// Remainder of class definition</p>
<p>}</p>
<p>A method can declare that it throws more than one exception, in which case the exceptions are declared in a list separated by commas. For example, the following method declares that it throws a RemoteException and an InsufficientFundsException &minus;</p>
<h3>Example</h3>
<p>import java.io.*;</p>
<p>publicclass className {</p>
<p>&nbsp;</p>
<p>publicvoid withdraw(double amount)throwsRemoteException,</p>
<p>InsufficientFundsException{</p>
<p>// Method implementation</p>
<p>}</p>
<p>// Remainder of class definition</p>
<p>}</p>
<h2>The Finally Block</h2>
<p>The finally block follows a try block or a catch block. A finally block of code always executes, irrespective of occurrence of an Exception.</p>
<p>Using a finally block allows you to run any cleanup-type statements that you want to execute, no matter what happens in the protected code.</p>
<p>A finally block appears at the end of the catch blocks and has the following syntax &minus;</p>
<h3>Syntax</h3>
<p>try {</p>
<p>// Protected code</p>
<p>} catch (ExceptionType1 e1) {</p>
<p>// Catch block</p>
<p>} catch (ExceptionType2 e2) {</p>
<p>// Catch block</p>
<p>} catch (ExceptionType3 e3) {</p>
<p>// Catch block</p>
<p>}finally {</p>
<p>// The finally block always executes.</p>
<p>}</p>
<h3>Example</h3>
<p>publicclassExcepTest{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>int a[]=newint[2];</p>
<p>try{</p>
<p>System.out.println("Access element three :"+ a[3]);</p>
<p>}catch(ArrayIndexOutOfBoundsException e){</p>
<p>System.out.println("Exception thrown&nbsp; :"+ e);</p>
<p>}finally{</p>
<p>a[0]=6;</p>
<p>System.out.println("First element value: "+ a[0]);</p>
<p>System.out.println("The finally statement is executed");</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Exception thrown&nbsp; :java.lang.ArrayIndexOutOfBoundsException: 3</p>
<p>First element value: 6</p>
<p>The finally statement is executed</p>
<p>Note the following &minus;</p>
<ul>
<li>A catch clause cannot exist without a try statement.</li>
<li>It is not compulsory to have finally clauses whenever a try/catch block is present.</li>
<li>The try block cannot be present without either catch clause or finally clause.</li>
<li>Any code cannot be present in between the try, catch, finally blocks.</li>
</ul>
<h2>The try-with-resources</h2>
<p>Generally, when we use any resources like streams, connections, etc. we have to close them explicitly using finally block. In the following program, we are reading data from a file using&nbsp;<strong>FileReader</strong>&nbsp;and we are closing it using finally block.</p>
<h3>Example</h3>
<p>import java.io.File;</p>
<p>import java.io.FileReader;</p>
<p>import java.io.IOException;</p>
<p>&nbsp;</p>
<p>publicclassReadData_Demo{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>FileReader fr =null;</p>
<p>try{</p>
<p>File file =newFile("file.txt");</p>
<p>fr =newFileReader(file);char[] a =newchar[50];</p>
<p>fr.read(a);// reads the content to the array</p>
<p>for(char c : a)</p>
<p>System.out.print(c);// prints the characters one by one</p>
<p>}catch(IOException e){</p>
<p>e.printStackTrace();</p>
<p>}finally{</p>
<p>try{</p>
<p>fr.close();</p>
<p>}catch(IOException ex){</p>
<p>ex.printStackTrace();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p><strong>try-with-resources</strong>, also referred as&nbsp;<strong>automatic resource management</strong>, is a new exception handling mechanism that was introduced in Java 7, which automatically closes the resources used within the try catch block.</p>
<p>To use this statement, you simply need to declare the required resources within the parenthesis, and the created resource will be closed automatically at the end of the block. Following is the syntax of try-with-resources statement.</p>
<h3>Syntax</h3>
<p>try(FileReader fr = new FileReader("file path")) {</p>
<p>// use the resource</p>
<p>} catch () {</p>
<p>// body of catch</p>
<p>}</p>
<p>}</p>
<p>Following is the program that reads the data in a file using try-with-resources statement.</p>
<h3>Example</h3>
<p>import java.io.FileReader;</p>
<p>import java.io.IOException;</p>
<p>&nbsp;</p>
<p>publicclassTry_withDemo{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>try(FileReader fr =newFileReader("E://file.txt")){</p>
<p>char[] a =newchar[50];</p>
<p>fr.read(a);// reads the contentto the array</p>
<p>for(char c : a)</p>
<p>System.out.print(c);// prints the characters one by one</p>
<p>}catch(IOException e){</p>
<p>e.printStackTrace();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>Following points are to be kept in mind while working with try-with-resources statement.</p>
<ul>
<li>To use a class with try-with-resources statement it should implement&nbsp;<strong>AutoCloseable</strong>interface and the&nbsp;<strong>close()</strong>method of it gets invoked automatically at runtime.</li>
<li>You can declare more than one class in try-with-resources statement.</li>
<li>While you declare multiple classes in the try block of try-with-resources statement these classes are closed in reverse order.</li>
<li>Except the declaration of resources within the parenthesis everything is the same as normal try/catch block of a try block.</li>
<li>The resource declared in try gets instantiated just before the start of the try-block.</li>
<li>The resource declared at the try block is implicitly declared as final.</li>
</ul>
<h2>User-defined Exceptions</h2>
<p>You can create your own exceptions in Java. Keep the following points in mind when writing your own exception classes &minus;</p>
<ul>
<li>All exceptions must be a child of Throwable.</li>
<li>If you want to write a checked exception that is automatically enforced by the Handle or Declare Rule, you need to extend the Exception class.</li>
<li>If you want to write a runtime exception, you need to extend the RuntimeException class.</li>
</ul>
<p>We can define our own Exception class as below &minus;</p>
<p>class MyException extends Exception {</p>
<p>}</p>
<p>You just need to extend the predefined&nbsp;<strong>Exception</strong>&nbsp;class to create your own Exception. These are considered to be checked exceptions. The following&nbsp;<strong>InsufficientFundsException</strong>&nbsp;class is a user-defined exception that extends the Exception class, making it a checked exception. An exception class is like any other class, containing useful fields and methods.</p>
<h3>Example</h3>
<p>// File Name InsufficientFundsException.java</p>
<p>import java.io.*;</p>
<p>&nbsp;</p>
<p>publicclassInsufficientFundsExceptionextendsException{</p>
<p>privatedouble amount;</p>
<p>&nbsp;</p>
<p>publicInsufficientFundsException(double amount){</p>
<p>this.amount = amount;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble getAmount(){</p>
<p>return amount;</p>
<p>}</p>
<p>}</p>
<p>To demonstrate using our user-defined exception, the following CheckingAccount class contains a withdraw() method that throws an InsufficientFundsException.</p>
<p>// File Name CheckingAccount.java</p>
<p>import java.io.*;</p>
<p>&nbsp;</p>
<p>publicclassCheckingAccount{</p>
<p>privatedouble balance;</p>
<p>privateint number;</p>
<p>&nbsp;</p>
<p>publicCheckingAccount(int number){</p>
<p>this.number = number;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid deposit(double amount){</p>
<p>balance += amount;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid withdraw(double amount)throwsInsufficientFundsException{</p>
<p>if(amount &lt;= balance){</p>
<p>balance -= amount;</p>
<p>}else{</p>
<p>double needs = amount - balance;</p>
<p>thrownewInsufficientFundsException(needs);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble getBalance(){</p>
<p>return balance;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicint getNumber(){</p>
<p>return number;</p>
<p>}</p>
<p>}</p>
<p>The following BankDemo program demonstrates invoking the deposit() and withdraw() methods of CheckingAccount.</p>
<p>// File Name BankDemo.java</p>
<p>publicclassBankDemo{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String[] args){</p>
<p>CheckingAccount c =newCheckingAccount(101);</p>
<p>System.out.println("Depositing $500...");</p>
<p>c.deposit(500.00);</p>
<p>&nbsp;</p>
<p>try{</p>
<p>System.out.println("\nWithdrawing $100...");</p>
<p>c.withdraw(100.00);</p>
<p>System.out.println("\nWithdrawing $600...");</p>
<p>c.withdraw(600.00);</p>
<p>}catch(InsufficientFundsException e){</p>
<p>System.out.println("Sorry, but you are short $"+ e.getAmount());</p>
<p>e.printStackTrace();</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>Compile all the above three files and run BankDemo. This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Depositing $500...</p>
<p>&nbsp;</p>
<p>Withdrawing $100...</p>
<p>&nbsp;</p>
<p>Withdrawing $600...</p>
<p>Sorry, but you are short $200.0</p>
<p>InsufficientFundsException</p>
<p>at CheckingAccount.withdraw(CheckingAccount.java:25)</p>
<p>at BankDemo.main(BankDemo.java:13)</p>
<h2>Common Exceptions</h2>
<p>In Java, it is possible to define two catergories of Exceptions and Errors.</p>
<ul>
<li><strong>JVM Exceptions</strong>&minus; These are exceptions/errors that are exclusively or logically thrown by the JVM. Examples: NullPointerException, ArrayIndexOutOfBoundsException, ClassCastException.</li>
<li><strong>Programmatic Exceptions</strong>&minus; These exceptions are thrown explicitly by the application or the API programmers. Examples: IllegalArgumentException, IllegalStateException.</li>
</ul>
<h1><u>Java - Inner classes</u></h1>
<p><u>In this chapter, we will discuss inner classes of Java.</u></p>
<h2>Nested Classes</h2>
<p>In Java, just like methods, variables of a class too can have another class as its member. Writing a class within another is allowed in Java. The class written within is called the&nbsp;<strong>nested class</strong>, and the class that holds the inner class is called the&nbsp;<strong>outer class</strong>.</p>
<p><strong>Syntax</strong></p>
<p>Following is the syntax to write a nested class. Here, the class&nbsp;<strong>Outer_Demo</strong>is the outer class and the class&nbsp;<strong>Inner_Demo</strong>&nbsp;is the nested class.</p>
<p>class Outer_Demo {</p>
<p>class Nested_Demo {</p>
<p>}</p>
<p>}</p>
<p>Nested classes are divided into two types &minus;</p>
<ul>
<li><strong>Non-static nested classes</strong>&minus; These are the non-static members of a class.</li>
<li><strong>Static nested classes</strong>&minus; These are the static members of a class.</li>
</ul>
<h2>Inner Classes (Non-static Nested Classes)</h2>
<p>Inner classes are a security mechanism in Java. We know a class cannot be associated with the access modifier&nbsp;<strong>private</strong>, but if we have the class as a member of other class, then the inner class can be made private. And this is also used to access the private members of a class.</p>
<p>Inner classes are of three types depending on how and where you define them. They are &minus;</p>
<ul>
<li>Inner Class</li>
<li>Method-local Inner Class</li>
<li>Anonymous Inner Class</li>
</ul>
<h3>Inner Class</h3>
<p>Creating an inner class is quite simple. You just need to write a class within a class. Unlike a class, an inner class can be private and once you declare an inner class private, it cannot be accessed from an object outside the class.</p>
<p>Following is the program to create an inner class and access it. In the given example, we make the inner class private and access the class through a method.</p>
<p><strong>Example</strong></p>
<p>classOuter_Demo{</p>
<p>int num;</p>
<p>&nbsp;</p>
<p>// inner class</p>
<p>privateclassInner_Demo{</p>
<p>publicvoidprint(){</p>
<p>System.out.println("This is an inner class");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>// Accessing he inner class from the method within</p>
<p>void display_Inner(){</p>
<p>Inner_Demo inner =newInner_Demo();</p>
<p>inner.print();</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassMy_class{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>// Instantiating the outer class</p>
<p>Outer_Demo outer =newOuter_Demo();</p>
<p>&nbsp;</p>
<p>// Accessing the display_Inner() method.</p>
<p>outer.display_Inner();</p>
<p>}</p>
<p>}</p>
<p>Here you can observe that&nbsp;<strong>Outer_Demo</strong>&nbsp;is the outer class,&nbsp;<strong>Inner_Demo</strong>&nbsp;is the inner class,&nbsp;<strong>display_Inner()</strong>&nbsp;is the method inside which we are instantiating the inner class, and this method is invoked from the&nbsp;<strong>main</strong>method.</p>
<p>If you compile and execute the above program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>This is an inner class.</p>
<h3>Accessing the Private Members</h3>
<p>As mentioned earlier, inner classes are also used to access the private members of a class. Suppose, a class is having private members to access them. Write an inner class in it, return the private members from a method within the inner class, say,&nbsp;<strong>getValue()</strong>, and finally from another class (from which you want to access the private members) call the getValue() method of the inner class.</p>
<p>To instantiate the inner class, initially you have to instantiate the outer class. Thereafter, using the object of the outer class, following is the way in which you can instantiate the inner class.</p>
<p>Outer_Demo outer = new Outer_Demo();</p>
<p>Outer_Demo.Inner_Demo inner = outer.new Inner_Demo();</p>
<p>The following program shows how to access the private members of a class using inner class.</p>
<p><strong>Example</strong></p>
<p>classOuter_Demo{</p>
<p>// private variable of the outer class</p>
<p>privateint num =175;</p>
<p>&nbsp;</p>
<p>// inner class</p>
<p>publicclassInner_Demo{</p>
<p>publicint getNum(){</p>
<p>System.out.println("This is the getnum method of the inner class");</p>
<p>return num;</p>
<p>}</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassMy_class2{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>// Instantiating the outer class</p>
<p>Outer_Demo outer =newOuter_Demo();</p>
<p>&nbsp;</p>
<p>// Instantiating the inner class</p>
<p>Outer_Demo.Inner_Demo inner = outer.newInner_Demo();</p>
<p>System.out.println(inner.getNum());</p>
<p>}</p>
<p>}</p>
<p>If you compile and execute the above program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>This is the getnum method of the inner class: 175</p>
<h2>Method-local Inner Class</h2>
<p>In Java, we can write a class within a method and this will be a local type. Like local variables, the scope of the inner class is restricted within the method.</p>
<p>A method-local inner class can be instantiated only within the method where the inner class is defined. The following program shows how to use a method-local inner class.</p>
<p><strong>Example</strong></p>
<p>publicclassOuterclass{</p>
<p>// instance method of the outer class</p>
<p>void my_Method(){</p>
<p>int num =23;</p>
<p>&nbsp;</p>
<p>// method-local inner class</p>
<p>classMethodInner_Demo{</p>
<p>publicvoidprint(){</p>
<p>System.out.println("This is method inner class "+num);</p>
<p>}</p>
<p>}// end of inner class</p>
<p>&nbsp;</p>
<p>// Accessing the inner class</p>
<p>MethodInner_Demo inner =newMethodInner_Demo();</p>
<p>inner.print();</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Outerclass outer =newOuterclass();</p>
<p>outer.my_Method();</p>
<p>}</p>
<p>}</p>
<p>If you compile and execute the above program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>This is method inner class 23</p>
<h2>Anonymous Inner Class</h2>
<p>An inner class declared without a class name is known as an&nbsp;<strong>anonymous inner class</strong>. In case of anonymous inner classes, we declare and instantiate them at the same time. Generally, they are used whenever you need to override the method of a class or an interface. The syntax of an anonymous inner class is as follows &minus;</p>
<p><strong>Syntax</strong></p>
<p>AnonymousInner an_inner = new AnonymousInner() {</p>
<p>public void my_method() {</p>
<p>........</p>
<p>........</p>
<p>}&nbsp;&nbsp;</p>
<p>};</p>
<p>The following program shows how to override the method of a class using anonymous inner class.</p>
<p><strong>Example</strong></p>
<p>abstractclassAnonymousInner{</p>
<p>publicabstractvoid mymethod();</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassOuter_class{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>AnonymousInner inner =newAnonymousInner(){</p>
<p>publicvoid mymethod(){</p>
<p>System.out.println("This is an example of anonymous inner class");</p>
<p>}</p>
<p>};</p>
<p>inner.mymethod();</p>
<p>}</p>
<p>}</p>
<p>If you compile and execute the above program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>This is an example of anonymous inner class</p>
<p>In the same way, you can override the methods of the concrete class as well as the interface using an anonymous inner class.</p>
<h2>Anonymous Inner Class as Argument</h2>
<p>Generally, if a method accepts an object of an interface, an abstract class, or a concrete class, then we can implement the interface, extend the abstract class, and pass the object to the method. If it is a class, then we can directly pass it to the method.</p>
<p>But in all the three cases, you can pass an anonymous inner class to the method. Here is the syntax of passing an anonymous inner class as a method argument &minus;</p>
<p>obj.my_Method(new My_Class() {</p>
<p>public void Do() {</p>
<p>.....</p>
<p>.....</p>
<p>}</p>
<p>});</p>
<p>The following program shows how to pass an anonymous inner class as a method argument.</p>
<p><strong>Example</strong></p>
<p>// interface</p>
<p>interfaceMessage{</p>
<p>String greet();</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassMy_class{</p>
<p>// method which accepts the object of interface Message</p>
<p>publicvoid displayMessage(Message m){</p>
<p>System.out.println(m.greet()+</p>
<p>", This is an example of anonymous inner class as an argument");</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>// Instantiating the class</p>
<p>My_class obj =newMy_class();</p>
<p>&nbsp;</p>
<p>// Passing an anonymous inner class as an argument</p>
<p>obj.displayMessage(newMessage(){</p>
<p>publicString greet(){</p>
<p>return"Hello";</p>
<p>}</p>
<p>});</p>
<p>}</p>
<p>}</p>
<p>If you compile and execute the above program, it gives you the following result &minus;</p>
<p><strong>Output</strong></p>
<p>Hello, This is an example of anonymous inner class as an argument</p>
<h2>Static Nested Class</h2>
<p>A static inner class is a nested class which is a static member of the outer class. It can be accessed without instantiating the outer class, using other static members. Just like static members, a static nested class does not have access to the instance variables and methods of the outer class. The syntax of static nested class is as follows &minus;</p>
<p><strong>Syntax</strong></p>
<p>class MyOuter {</p>
<p>static class Nested_Demo {</p>
<p>}</p>
<p>}</p>
<p>Instantiating a static nested class is a bit different from instantiating an inner class. The following program shows how to use a static nested class.</p>
<p><strong>Example</strong></p>
<p>publicclassOuter{</p>
<p>staticclassNested_Demo{</p>
<p>publicvoid my_method(){</p>
<p>System.out.println("This is my nested class");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Outer.Nested_Demo nested =newOuter.Nested_Demo();</p>
<p>nested.my_method();</p>
<p>}</p>
<p>}</p>
<p>If you compile and execute the above program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>This is my nested class</p>
<h1><u>Java &ndash; Inheritance</u></h1>
<p><u>Inheritance can be defined as the process where one class acquires the properties (methods and fields) of another. With the use of inheritance the information is made manageable in a hierarchical order.</u></p>
<p>The class which inherits the properties of other is known as subclass (derived class, child class) and the class whose properties are inherited is known as superclass (base class, parent class).</p>
<h2>extends Keyword</h2>
<p><strong>extends</strong>&nbsp;is the keyword used to inherit the properties of a class. Following is the syntax of extends keyword.</p>
<p><strong>Syntax</strong></p>
<p>class Super {</p>
<p>.....</p>
<p>.....</p>
<p>}</p>
<p>class Sub extends Super {</p>
<p>.....</p>
<p>.....</p>
<p>}</p>
<h2>Sample Code</h2>
<p>Following is an example demonstrating Java inheritance. In this example, you can observe two classes namely Calculation and My_Calculation.</p>
<p>Using extends keyword, the My_Calculation inherits the methods addition() and Subtraction() of Calculation class.</p>
<p>Copy and paste the following program in a file with name My_Calculation.java</p>
<p><strong>Example</strong></p>
<p><u>class</u><u>Calculation</u><u>{</u></p>
<p>int z;</p>
<p>&nbsp;</p>
<p>publicvoid addition(int x,int y){</p>
<p>z = x + y;</p>
<p>System.out.println("The sum of the given numbers:"+z);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoidSubtraction(int x,int y){</p>
<p>z = x - y;</p>
<p>System.out.println("The difference between the given numbers:"+z);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassMy_CalculationextendsCalculation{</p>
<p>publicvoid multiplication(int x,int y){</p>
<p>z = x * y;</p>
<p>System.out.println("The product of the given numbers:"+z);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>int a =20, b =10;</p>
<p>My_Calculation demo =newMy_Calculation();</p>
<p>demo.addition(a, b);</p>
<p>demo.Subtraction(a, b);</p>
<p>demo.multiplication(a, b);</p>
<p>}</p>
<p>}</p>
<p>Compile and execute the above code as shown below.</p>
<p>javac My_Calculation.java</p>
<p>java My_Calculation</p>
<p>After executing the program, it will produce the following result &minus;</p>
<p><strong>Output</strong></p>
<p>The sum of the given numbers:30</p>
<p>The difference between the given numbers:10</p>
<p>The product of the given numbers:200</p>
<p>In the given program, when an object to&nbsp;<strong>My_Calculation</strong>&nbsp;class is created, a copy of the contents of the superclass is made within it. That is why, using the object of the subclass you can access the members of a superclass.</p>
<p>The Superclass reference variable can hold the subclass object, but using that variable you can access only the members of the superclass, so to access the members of both classes it is recommended to always create reference variable to the subclass.</p>
<p>If you consider the above program, you can instantiate the class as given below. But using the superclass reference variable (&nbsp;<strong>cal</strong>&nbsp;in this case) you cannot call the method&nbsp;<strong>multiplication()</strong>, which belongs to the subclass My_Calculation.</p>
<p>Calculation cal =newMy_Calculation();</p>
<p>demo.addition(a, b);</p>
<p>demo.Subtraction(a, b);</p>
<p><strong>Note</strong>&nbsp;&minus; A subclass inherits all the members (fields, methods, and nested classes) from its superclass. Constructors are not members, so they are not inherited by subclasses, but the constructor of the superclass can be invoked from the subclass.</p>
<h2>The super keyword</h2>
<p>The&nbsp;<strong>super</strong>&nbsp;keyword is similar to&nbsp;<strong>this</strong>&nbsp;keyword. Following are the scenarios where the super keyword is used.</p>
<ul>
<li>It is used to&nbsp;<strong>differentiate the members</strong>of superclass from the members of subclass, if they have same names.</li>
<li>It is used to&nbsp;<strong>invoke the superclass</strong>constructor from subclass.</li>
</ul>
<h3>Differentiating the Members</h3>
<p>If a class is inheriting the properties of another class. And if the members of the superclass have the names same as the sub class, to differentiate these variables we use super keyword as shown below.</p>
<p>super.variable</p>
<p>super.method();</p>
<h3>Sample Code</h3>
<p>This section provides you a program that demonstrates the usage of the&nbsp;<strong>super</strong>&nbsp;keyword.</p>
<p>In the given program, you have two classes namely&nbsp;<em>Sub_class</em>&nbsp;and&nbsp;<em>Super_class</em>, both have a method named display() with different implementations, and a variable named num with different values. We are invoking display() method of both classes and printing the value of the variable num of both classes. Here you can observe that we have used super keyword to differentiate the members of superclass from subclass.</p>
<p>Copy and paste the program in a file with name Sub_class.java.</p>
<p><strong>Example</strong></p>
<p><u>class</u><u>Super_class</u><u>{</u></p>
<p>int num =20;</p>
<p>&nbsp;</p>
<p>// display method of superclass</p>
<p>publicvoid display(){</p>
<p>System.out.println("This is the display method of superclass");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassSub_classextendsSuper_class{</p>
<p>int num =10;</p>
<p>&nbsp;</p>
<p>// display method of sub class</p>
<p>publicvoid display(){</p>
<p>System.out.println("This is the display method of subclass");</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid my_method(){</p>
<p>// Instantiating subclass</p>
<p>Sub_classsub=newSub_class();</p>
<p>&nbsp;</p>
<p>// Invoking the display() method of sub class</p>
<p>sub.display();</p>
<p>&nbsp;</p>
<p>// Invoking the display() method of superclass</p>
<p>super.display();</p>
<p>&nbsp;</p>
<p>// printing the value of variable num of subclass</p>
<p>System.out.println("value of the variable named num in sub class:"+sub.num);</p>
<p>&nbsp;</p>
<p>// printing the value of variable num of superclass</p>
<p>System.out.println("value of the variable named num in super class:"+super.num);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Sub_class obj =newSub_class();</p>
<p>obj.my_method();</p>
<p>}</p>
<p>}</p>
<p>Compile and execute the above code using the following syntax.</p>
<p>javac Super_Demo</p>
<p>java Super</p>
<p>On executing the program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>This is the display method of subclass</p>
<p>This is the display method of superclass</p>
<p>value of the variable named num in sub class:10</p>
<p>value of the variable named num in super class:20</p>
<h2>Invoking Superclass Constructor</h2>
<p>If a class is inheriting the properties of another class, the subclass automatically acquires the default constructor of the superclass. But if you want to call a parameterized constructor of the superclass, you need to use the super keyword as shown below.</p>
<p>super(values);</p>
<h3>Sample Code</h3>
<p>The program given in this section demonstrates how to use the super keyword to invoke the parametrized constructor of the superclass. This program contains a superclass and a subclass, where the superclass contains a parameterized constructor which accepts a string value, and we used the super keyword to invoke the parameterized constructor of the superclass.</p>
<p>Copy and paste the following program in a file with the name Subclass.java</p>
<p><strong>Example</strong></p>
<p><u>class</u><u>Superclass</u><u>{</u></p>
<p>int age;</p>
<p>&nbsp;</p>
<p>Superclass(int age){</p>
<p>this.age = age;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid getAge(){</p>
<p>System.out.println("The value of the variable named age in super class is: "+age);</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassSubclassextendsSuperclass{</p>
<p>Subclass(int age){</p>
<p>super(age);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String argd[]){</p>
<p>Subclass s =newSubclass(24);</p>
<p>s.getAge();</p>
<p>}</p>
<p>}</p>
<p>Compile and execute the above code using the following syntax.</p>
<p>javac Subclass</p>
<p>java Subclass</p>
<p>On executing the program, you will get the following result &minus;</p>
<p><strong>Output</strong></p>
<p>The value of the variable named age in super class is: 24</p>
<h2>IS-A Relationship</h2>
<p>IS-A is a way of saying: This object is a type of that object. Let us see how the&nbsp;<strong>extends</strong>&nbsp;keyword is used to achieve inheritance.</p>
<p>publicclassAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassMammalextendsAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassReptileextendsAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassDogextendsMammal{</p>
<p>}</p>
<p>Now, based on the above example, in Object-Oriented terms, the following are true &minus;</p>
<ul>
<li>Animal is the superclass of Mammal class.</li>
<li>Animal is the superclass of Reptile class.</li>
<li>Mammal and Reptile are subclasses of Animal class.</li>
<li>Dog is the subclass of both Mammal and Animal classes.</li>
</ul>
<p>Now, if we consider the IS-A relationship, we can say &minus;</p>
<ul>
<li>Mammal IS-A Animal</li>
<li>Reptile IS-A Animal</li>
<li>Dog IS-A Mammal</li>
<li>Hence: Dog IS-A Animal as well</li>
</ul>
<p>With the use of the extends keyword, the subclasses will be able to inherit all the properties of the superclass except for the private properties of the superclass.</p>
<p>We can assure that Mammal is actually an Animal with the use of the instance operator.</p>
<p><strong>Example</strong></p>
<p><u>class</u><u>Animal</u><u>{</u></p>
<p>}</p>
<p>&nbsp;</p>
<p>classMammalextendsAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>classReptileextendsAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassDogextendsMammal{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Animal a =newAnimal();</p>
<p>Mammal m =newMammal();</p>
<p>Dog d =newDog();</p>
<p>&nbsp;</p>
<p>System.out.println(m instanceofAnimal);</p>
<p>System.out.println(d instanceofMammal);</p>
<p>System.out.println(d instanceofAnimal);</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<p><strong>Output</strong></p>
<p>true</p>
<p>true</p>
<p>true</p>
<p>Since we have a good understanding of the&nbsp;<strong>extends</strong>&nbsp;keyword, let us look into how the&nbsp;<strong>implements</strong>&nbsp;keyword is used to get the IS-A relationship.</p>
<p>Generally, the&nbsp;<strong>implements</strong>&nbsp;keyword is used with classes to inherit the properties of an interface. Interfaces can never be extended by a class.</p>
<p><strong>Example</strong></p>
<p>publicinterfaceAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassMammalimplementsAnimal{</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassDogextendsMammal{</p>
<p>}</p>
<h2>The instanceof Keyword</h2>
<p>Let us use the&nbsp;<strong>instanceof</strong>&nbsp;operator to check determine whether Mammal is actually an Animal, and dog is actually an Animal.</p>
<p><strong>Example</strong></p>
<p><u>interface</u><u>Animal</u><u>{}</u></p>
<p>classMammalimplementsAnimal{}</p>
<p>&nbsp;</p>
<p>publicclassDogextendsMammal{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Mammal m =newMammal();</p>
<p>Dog d =newDog();</p>
<p>&nbsp;</p>
<p>System.out.println(m instanceofAnimal);</p>
<p>System.out.println(d instanceofMammal);</p>
<p>System.out.println(d instanceofAnimal);</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<p><strong>Output</strong></p>
<p>true</p>
<p>true</p>
<p>true</p>
<h2>HAS-A relationship</h2>
<p>These relationships are mainly based on the usage. This determines whether a certain class&nbsp;<strong>HAS-A</strong>&nbsp;certain thing. This relationship helps to reduce duplication of code as well as bugs.</p>
<p>Lets look into an example &minus;</p>
<p><strong>Example</strong></p>
<p>publicclassVehicle{}</p>
<p>publicclassSpeed{}</p>
<p>&nbsp;</p>
<p>publicclassVanextendsVehicle{</p>
<p>privateSpeed sp;</p>
<p>}</p>
<p>This shows that class Van HAS-A Speed. By having a separate class for Speed, we do not have to put the entire code that belongs to speed inside the Van class, which makes it possible to reuse the Speed class in multiple applications.</p>
<p>In Object-Oriented feature, the users do not need to bother about which object is doing the real work. To achieve this, the Van class hides the implementation details from the users of the Van class. So, basically what happens is the users would ask the Van class to do a certain action and the Van class will either do the work by itself or ask another class to perform the action.</p>
<h2>Types of Inheritance</h2>
<p>There are various types of inheritance as demonstrated below.</p>
<h1><u>Java &ndash; Overriding</u></h1>
<p><u>In the previous chapter, we talked about superclasses and subclasses. If a class inherits a method from its superclass, then there is a chance to override the method provided that it is not marked final.</u></p>
<p>The benefit of overriding is: ability to define a behavior that's specific to the subclass type, which means a subclass can implement a parent class method based on its requirement.</p>
<p>In object-oriented terms, overriding means to override the functionality of an existing method.</p>
<h3>Example</h3>
<p>Let us look at an example.</p>
<p><u>class</u><u>Animal</u><u>{</u></p>
<p>publicvoid move(){</p>
<p>System.out.println("Animals can move");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>classDogextendsAnimal{</p>
<p>publicvoid move(){</p>
<p>System.out.println("Dogs can walk and run");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassTestDog{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Animal a =newAnimal();// Animal reference and object</p>
<p>Animal b =newDog();// Animal reference but Dog object</p>
<p>&nbsp;</p>
<p>a.move();// runs the method in Animal class</p>
<p>b.move();// runs the method in Dog class</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Animals can move</p>
<p>Dogs can walk and run</p>
<p>In the above example, you can see that even though&nbsp;<strong>b</strong>&nbsp;is a type of Animal it runs the move method in the Dog class. The reason for this is: In compile time, the check is made on the reference type. However, in the runtime, JVM figures out the object type and would run the method that belongs to that particular object.</p>
<p>Therefore, in the above example, the program will compile properly since Animal class has the method move. Then, at the runtime, it runs the method specific for that object.</p>
<p>Consider the following example &minus;</p>
<h3>Example</h3>
<h1><u>&nbsp;</u></h1>
<p>&nbsp;</p>
<p>A very important fact to remember is that Java does not support multiple inheritance. This means that a class cannot extend more than one class. Therefore following is illegal &minus;</p>
<p><strong>Example</strong></p>
<p>publicclassextendsAnimal,Mammal{}</p>
<p>However, a class can implement one or more interfaces, which has helped Java get rid of the impossibility of multiple inheritance.</p>
<p>classAnimal{</p>
<p>publicvoid move(){</p>
<p>System.out.println("Animals can move");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>classDogextendsAnimal{</p>
<p>publicvoid move(){</p>
<p>System.out.println("Dogs can walk and run");</p>
<p>}</p>
<p>publicvoid bark(){</p>
<p>System.out.println("Dogs can bark");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassTestDog{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Animal a =newAnimal();// Animal reference and object</p>
<p>Animal b =newDog();// Animal reference but Dog object</p>
<p>&nbsp;</p>
<p>a.move();// runs the method in Animal class</p>
<p>b.move();// runs the method in Dog class</p>
<p>b.bark();</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>TestDog.java:26: error: cannot find symbol</p>
<p>b.bark();</p>
<p>^</p>
<p>symbol:&nbsp;&nbsp; method bark()</p>
<p>location: variable b of type Animal</p>
<p>1 error</p>
<p>This program will throw a compile time error since b's reference type Animal doesn't have a method by the name of bark.</p>
<h2>Rules for Method Overriding</h2>
<ul>
<li>The argument list should be exactly the same as that of the overridden method.</li>
<li>The return type should be the same or a subtype of the return type declared in the original overridden method in the superclass.</li>
<li>The access level cannot be more restrictive than the overridden method's access level. For example: If the superclass method is declared public then the overridding method in the sub class cannot be either private or protected.</li>
<li>Instance methods can be overridden only if they are inherited by the subclass.</li>
<li>A method declared final cannot be overridden.</li>
<li>A method declared static cannot be overridden but can be re-declared.</li>
<li>If a method cannot be inherited, then it cannot be overridden.</li>
<li>A subclass within the same package as the instance's superclass can override any superclass method that is not declared private or final.</li>
<li>A subclass in a different package can only override the non-final methods declared public or protected.</li>
<li>An overriding method can throw any uncheck exceptions, regardless of whether the overridden method throws exceptions or not. However, the overriding method should not throw checked exceptions that are new or broader than the ones declared by the overridden method. The overriding method can throw narrower or fewer exceptions than the overridden method.</li>
<li>Constructors cannot be overridden.</li>
</ul>
<h2>Using the super Keyword</h2>
<p>When invoking a superclass version of an overridden method the&nbsp;<strong>super</strong>keyword is used.</p>
<h3>Example</h3>
<p>classAnimal{</p>
<p>publicvoid move(){</p>
<p>System.out.println("Animals can move");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>classDogextendsAnimal{</p>
<p>publicvoid move(){</p>
<p>super.move();// invokes the super class method</p>
<p>System.out.println("Dogs can walk and run");</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicclassTestDog{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>Animal b =newDog();// Animal reference but Dog object</p>
<p>b.move();// runs the method in Dog class</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Animals can move</p>
<p>Dogs can walk and run</p>
<h1><u>Java &ndash; Polymorphism</u></h1>
<p>Polymorphism is the ability of an object to take on many forms. The most common use of polymorphism in OOP occurs when a parent class reference is used to refer to a child class object.</p>
<p>Any Java object that can pass more than one IS-A test is considered to be polymorphic. In Java, all Java objects are polymorphic since any object will pass the IS-A test for their own type and for the class Object.</p>
<p>It is important to know that the only possible way to access an object is through a reference variable. A reference variable can be of only one type. Once declared, the type of a reference variable cannot be changed.</p>
<p>The reference variable can be reassigned to other objects provided that it is not declared final. The type of the reference variable would determine the methods that it can invoke on the object.</p>
<p>A reference variable can refer to any object of its declared type or any subtype of its declared type. A reference variable can be declared as a class or interface type.</p>
<h3>Example</h3>
<p>Let us look at an example.</p>
<p>publicinterfaceVegetarian{}</p>
<p>publicclassAnimal{}</p>
<p>publicclassDeerextendsAnimalimplementsVegetarian{}</p>
<p>Now, the Deer class is considered to be polymorphic since this has multiple inheritance. Following are true for the above examples &minus;</p>
<ul>
<li>A Deer IS-A Animal</li>
<li>A Deer IS-A Vegetarian</li>
<li>A Deer IS-A Deer</li>
<li>A Deer IS-A Object</li>
</ul>
<p>When we apply the reference variable facts to a Deer object reference, the following declarations are legal &minus;</p>
<h3>Example</h3>
<p>Deer d =newDeer();</p>
<p>Animal a = d;</p>
<p>Vegetarian v = d;</p>
<p>Object o = d;</p>
<p>All the reference variables d, a, v, o refer to the same Deer object in the heap.</p>
<h2>Virtual Methods</h2>
<p>In this section, I will show you how the behavior of overridden methods in Java allows you to take advantage of polymorphism when designing your classes.</p>
<p>We already have discussed method overriding, where a child class can override a method in its parent. An overridden method is essentially hidden in the parent class, and is not invoked unless the child class uses the super keyword within the overriding method.</p>
<h3>Example</h3>
<p>/* File name : Employee.java */</p>
<p>publicclassEmployee{</p>
<p>privateString name;</p>
<p>privateString address;</p>
<p>privateint number;</p>
<p>&nbsp;</p>
<p>publicEmployee(String name,String address,int number){</p>
<p>System.out.println("Constructing an Employee");</p>
<p>this.name = name;</p>
<p>this.address = address;</p>
<p>this.number = number;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid mailCheck(){</p>
<p>System.out.println("Mailing a check to "+this.name +""+this.address);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicString toString(){</p>
<p>return name +""+ address +""+ number;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicString getName(){</p>
<p>return name;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicString getAddress(){</p>
<p>return address;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid setAddress(String newAddress){</p>
<p>address = newAddress;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicint getNumber(){</p>
<p>return number;</p>
<p>}</p>
<p>}</p>
<p>Now suppose we extend Employee class as follows &minus;</p>
<p>/* File name : Salary.java */</p>
<p>publicclassSalaryextendsEmployee{</p>
<p>privatedouble salary;// Annual salary</p>
<p>&nbsp;</p>
<p>publicSalary(String name,String address,int number,double salary){</p>
<p>super(name, address, number);</p>
<p>setSalary(salary);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid mailCheck(){</p>
<p>System.out.println("Within mailCheck of Salary class ");</p>
<p>System.out.println("Mailing check to "+ getName()</p>
<p>+" with salary "+ salary);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble getSalary(){</p>
<p>return salary;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid setSalary(double newSalary){</p>
<p>if(newSalary &gt;=0.0){</p>
<p>salary = newSalary;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble computePay(){</p>
<p>System.out.println("Computing salary pay for "+ getName());</p>
<p>return salary/52;</p>
<p>}</p>
<p>}</p>
<p>Now, you study the following program carefully and try to determine its output &minus;</p>
<p>/* File name : VirtualDemo.java */</p>
<p>publicclassVirtualDemo{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String[] args){</p>
<p>Salary s =newSalary("Mohd Mohtashim","Ambehta, UP",3,3600.00);</p>
<p>Employee e =newSalary("John Adams","Boston, MA",2,2400.00);</p>
<p>System.out.println("Call mailCheck using Salary reference --");</p>
<p>s.mailCheck();</p>
<p>System.out.println("\n Call mailCheck using Employee reference--");</p>
<p>e.mailCheck();</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Constructing an Employee</p>
<p>Constructing an Employee</p>
<p>&nbsp;</p>
<p>Call mailCheck using Salary reference --</p>
<p>Within mailCheck of Salary class</p>
<p>ailing check to Mohd Mohtashim with salary 3600.0</p>
<p>&nbsp;</p>
<p>Call mailCheck using Employee reference--</p>
<p>Within mailCheck of Salary class</p>
<p>ailing check to John Adams with salary 2400.0</p>
<p>Here, we instantiate two Salary objects. One using a Salary reference&nbsp;<strong>s</strong>, and the other using an Employee reference&nbsp;<strong>e</strong>.</p>
<p>While invoking&nbsp;<em>s.mailCheck()</em>, the compiler sees mailCheck() in the Salary class at compile time, and the JVM invokes mailCheck() in the Salary class at run time.</p>
<p>mailCheck() on&nbsp;<strong>e</strong>&nbsp;is quite different because&nbsp;<strong>e</strong>&nbsp;is an Employee reference. When the compiler sees&nbsp;<em>e.mailCheck()</em>, the compiler sees the mailCheck() method in the Employee class.</p>
<p>Here, at compile time, the compiler used mailCheck() in Employee to validate this statement. At run time, however, the JVM invokes mailCheck() in the Salary class.</p>
<p>This behavior is referred to as virtual method invocation, and these methods are referred to as virtual methods. An overridden method is invoked at run time, no matter what data type the reference is that was used in the source code at compile time.</p>
<h1><u>Java &ndash; Abstraction</u></h1>
<p>As per dictionary,&nbsp;<strong>abstraction</strong>&nbsp;is the quality of dealing with ideas rather than events. For example, when you consider the case of e-mail, complex details such as what happens as soon as you send an e-mail, the protocol your e-mail server uses are hidden from the user. Therefore, to send an e-mail you just need to type the content, mention the address of the receiver, and click send.</p>
<p>Likewise in Object-oriented programming, abstraction is a process of hiding the implementation details from the user, only the functionality will be provided to the user. In other words, the user will have the information on what the object does instead of how it does it.</p>
<p>In Java, abstraction is achieved using Abstract classes and interfaces.</p>
<h2>Abstract Class</h2>
<p>A class which contains the&nbsp;<strong>abstract</strong>&nbsp;keyword in its declaration is known as abstract class.</p>
<ul>
<li>Abstract classes may or may not contain&nbsp;<em>abstract methods</em>, i.e., methods without body ( public void get(); )</li>
<li>But, if a class has at least one abstract method, then the class&nbsp;<strong>must</strong>be declared abstract.</li>
<li>If a class is declared abstract, it cannot be instantiated.</li>
<li>To use an abstract class, you have to inherit it from another class, provide implementations to the abstract methods in it.</li>
<li>If you inherit an abstract class, you have to provide implementations to all the abstract methods in it.</li>
</ul>
<h3>Example</h3>
<p>This section provides you an example of the abstract class. To create an abstract class, just use the&nbsp;<strong>abstract</strong>&nbsp;keyword before the class keyword, in the class declaration.</p>
<p>/* File name : Employee.java */</p>
<p>publicabstractclassEmployee{</p>
<p>privateString name;</p>
<p>privateString address;</p>
<p>privateint number;</p>
<p>&nbsp;</p>
<p>publicEmployee(String name,String address,int number){</p>
<p>System.out.println("Constructing an Employee");</p>
<p>this.name = name;</p>
<p>this.address = address;</p>
<p>this.number = number;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble computePay(){</p>
<p>System.out.println("Inside Employee computePay");</p>
<p>return0.0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid mailCheck(){</p>
<p>System.out.println("Mailing a check to "+this.name +""+this.address);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicString toString(){</p>
<p>return name +""+ address +""+ number;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicString getName(){</p>
<p>return name;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicString getAddress(){</p>
<p>return address;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid setAddress(String newAddress){</p>
<p>address = newAddress;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicint getNumber(){</p>
<p>return number;</p>
<p>}</p>
<p>}</p>
<p>You can observe that except abstract methods the Employee class is same as normal class in Java. The class is now abstract, but it still has three fields, seven methods, and one constructor.</p>
<p>Now you can try to instantiate the Employee class in the following way &minus;</p>
<p>/* File name : AbstractDemo.java */</p>
<p>publicclassAbstractDemo{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String[] args){</p>
<p>/* Following is not allowed and would raise error */</p>
<p>Employee e =newEmployee("George W.","Houston, TX",43);</p>
<p>System.out.println("\n Call mailCheck using Employee reference--");</p>
<p>e.mailCheck();</p>
<p>}</p>
<p>}</p>
<p>When you compile the above class, it gives you the following error &minus;</p>
<p>Employee.java:46: Employee is abstract; cannot be instantiated</p>
<p>Employee e = new Employee("George W.", "Houston, TX", 43);</p>
<p>^</p>
<p>1 error</p>
<h2>Inheriting the Abstract Class</h2>
<p>We can inherit the properties of Employee class just like concrete class in the following way &minus;</p>
<h3>Example</h3>
<p>/* File name : Salary.java */</p>
<p>publicclassSalaryextendsEmployee{</p>
<p>privatedouble salary;// Annual salary</p>
<p>&nbsp;</p>
<p>publicSalary(String name,String address,int number,double salary){</p>
<p>super(name, address, number);</p>
<p>setSalary(salary);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid mailCheck(){</p>
<p>System.out.println("Within mailCheck of Salary class ");</p>
<p>System.out.println("Mailing check to "+ getName()+" with salary "+ salary);</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble getSalary(){</p>
<p>return salary;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid setSalary(double newSalary){</p>
<p>if(newSalary &gt;=0.0){</p>
<p>salary = newSalary;</p>
<p>}</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicdouble computePay(){</p>
<p>System.out.println("Computing salary pay for "+ getName());</p>
<p>return salary/52;</p>
<p>}</p>
<p>}</p>
<p>Here, you cannot instantiate the Employee class, but you can instantiate the Salary Class, and using this instance you can access all the three fields and seven methods of Employee class as shown below.</p>
<p>/* File name : AbstractDemo.java */</p>
<p>publicclassAbstractDemo{</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String[] args){</p>
<p>Salary s =newSalary("Mohd Mohtashim","Ambehta, UP",3,3600.00);</p>
<p>Employee e =newSalary("John Adams","Boston, MA",2,2400.00);</p>
<p>System.out.println("Call mailCheck using Salary reference --");</p>
<p>s.mailCheck();</p>
<p>System.out.println("\n Call mailCheck using Employee reference--");</p>
<p>e.mailCheck();</p>
<p>}</p>
<p>}</p>
<p>This produces the following result &minus;</p>
<h3>Output</h3>
<p>Constructing an Employee</p>
<p>Constructing an Employee</p>
<p>Call mailCheck using Salary reference --</p>
<p>Within mailCheck of Salary class</p>
<p>Mailing check to Mohd Mohtashim with salary 3600.0</p>
<p>&nbsp;</p>
<p>Call mailCheck using Employee reference--</p>
<p>Within mailCheck of Salary class</p>
<p>Mailing check to John Adams with salary 2400.0</p>
<h2>Abstract Methods</h2>
<p>If you want a class to contain a particular method but you want the actual implementation of that method to be determined by child classes, you can declare the method in the parent class as an abstract.</p>
<ul>
<li><strong>abstract</strong>keyword is used to declare the method as abstract.</li>
<li>You have to place the&nbsp;<strong>abstract</strong>keyword before the method name in the method declaration.</li>
<li>An abstract method contains a method signature, but no method body.</li>
<li>Instead of curly braces, an abstract method will have a semoi colon (;) at the end.</li>
</ul>
<p>Following is an example of the abstract method.</p>
<h3>Example</h3>
<p>publicabstractclassEmployee{</p>
<p>privateString name;</p>
<p>privateString address;</p>
<p>privateint number;</p>
<p>&nbsp;</p>
<p>publicabstractdouble computePay();</p>
<p>// Remainder of class definition</p>
<p>}</p>
<p>Declaring a method as abstract has two consequences &minus;</p>
<ul>
<li>The class containing it must be declared as abstract.</li>
<li>Any class inheriting the current class must either override the abstract method or declare itself as abstract.</li>
</ul>
<p><strong>Note</strong>&nbsp;&minus; Eventually, a descendant class has to implement the abstract method; otherwise, you would have a hierarchy of abstract classes that cannot be instantiated.</p>
<p>Suppose Salary class inherits the Employee class, then it should implement the&nbsp;<strong>computePay()</strong>&nbsp;method as shown below &minus;</p>
<p>/* File name : Salary.java */</p>
<p>publicclassSalaryextendsEmployee{</p>
<p>privatedouble salary;// Annual salary</p>
<p>&nbsp;</p>
<p>publicdouble computePay(){</p>
<p>System.out.println("Computing salary pay for "+ getName());</p>
<p>return salary/52;</p>
<p>}</p>
<p>// Remainder of class definition</p>
<p>}</p>
<h1><u>Java - Encapsulation</u></h1>
<p><strong>Encapsulation</strong>&nbsp;is one of the four fundamental OOP concepts. The other three are inheritance, polymorphism, and abstraction.</p>
<p>Encapsulation in Java is a mechanism of wrapping the data (variables) and code acting on the data (methods) together as a single unit. In encapsulation, the variables of a class will be hidden from other classes, and can be accessed only through the methods of their current class. Therefore, it is also known as&nbsp;<strong>data hiding</strong>.</p>
<p>To achieve encapsulation in Java &minus;</p>
<ul>
<li>Declare the variables of a class as private.</li>
<li>Provide public setter and getter methods to modify and view the variables values.</li>
</ul>
<h3>Example</h3>
<p>Following is an example that demonstrates how to achieve Encapsulation in Java &minus;</p>
<p>/* File name : EncapTest.java */</p>
<p>publicclassEncapTest{</p>
<p>privateString name;</p>
<p>privateString idNum;</p>
<p>privateint age;</p>
<p>publicint getAge(){</p>
<p>return age;</p>
<p>}</p>
<p>publicString getName(){</p>
<p>return name;</p>
<p>}</p>
<p>publicString getIdNum(){</p>
<p>return idNum;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid setAge(int newAge){</p>
<p>age = newAge;</p>
<p>}</p>
<p>publicvoid setName(String newName){</p>
<p>name = newName;</p>
<p>}</p>
<p>publicvoid setIdNum(String newId){</p>
<p>idNum = newId;</p>
<p>}</p>
<p>}</p>
<p>The public setXXX() and getXXX() methods are the access points of the instance variables of the EncapTest class. Normally, these methods are referred as getters and setters. Therefore, any class that wants to access the variables should access them through these getters and setters.</p>
<p>The variables of the EncapTest class can be accessed using the following program &minus;</p>
<p>/* File name : RunEncap.java */</p>
<p>publicclassRunEncap{</p>
<p>publicstaticvoid main(String args[]){</p>
<p>EncapTest encap =newEncapTest();</p>
<p>encap.setName("James");</p>
<p>encap.setAge(20);</p>
<p>encap.setIdNum("12343ms");</p>
<p>System.out.print("Name : "+ encap.getName()+" Age : "+ encap.getAge());</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Name : James Age : 20</p>
<h2>Benefits of Encapsulation</h2>
<ul>
<li>The fields of a class can be made read-only or write-only.</li>
<li>A class can have total control over what is stored in its fields.</li>
</ul>
<h1><u>Java &ndash; Interfaces</u></h1>
<p>An interface is a reference type in Java. It is similar to class. It is a collection of abstract methods. A class implements an interface, thereby inheriting the abstract methods of the interface.</p>
<p>Along with abstract methods, an interface may also contain constants, default methods, static methods, and nested types. Method bodies exist only for default methods and static methods.</p>
<p>Writing an interface is similar to writing a class. But a class describes the attributes and behaviors of an object. And an interface contains behaviors that a class implements.</p>
<p>Unless the class that implements the interface is abstract, all the methods of the interface need to be defined in the class.</p>
<p>An interface is similar to a class in the following ways &minus;</p>
<ul>
<li>An interface can contain any number of methods.</li>
<li>An interface is written in a file with a&nbsp;<strong>.java</strong>extension, with the name of the interface matching the name of the file.</li>
<li>The byte code of an interface appears in a&nbsp;<strong>.class</strong></li>
<li>Interfaces appear in packages, and their corresponding bytecode file must be in a directory structure that matches the package name.</li>
</ul>
<p>However, an interface is different from a class in several ways, including &minus;</p>
<ul>
<li>You cannot instantiate an interface.</li>
<li>An interface does not contain any constructors.</li>
<li>All of the methods in an interface are abstract.</li>
<li>An interface cannot contain instance fields. The only fields that can appear in an interface must be declared both static and final.</li>
<li>An interface is not extended by a class; it is implemented by a class.</li>
<li>An interface can extend multiple interfaces.</li>
</ul>
<h2>Declaring Interfaces</h2>
<p>The&nbsp;<strong>interface</strong>&nbsp;keyword is used to declare an interface. Here is a simple example to declare an interface &minus;</p>
<h3>Example</h3>
<p>Following is an example of an interface &minus;</p>
<p>/* File name : NameOfInterface.java */</p>
<p>import java.lang.*;</p>
<p>// Any number of import statements</p>
<p>&nbsp;</p>
<p>publicinterfaceNameOfInterface{</p>
<p>// Any number of final, static fields</p>
<p>// Any number of abstract method declarations\</p>
<p>}</p>
<p>Interfaces have the following properties &minus;</p>
<ul>
<li>An interface is implicitly abstract. You do not need to use the&nbsp;<strong>abstract</strong>keyword while declaring an interface.</li>
<li>Each method in an interface is also implicitly abstract, so the abstract keyword is not needed.</li>
<li>Methods in an interface are implicitly public.</li>
</ul>
<h3>Example</h3>
<p>/* File name : Animal.java */</p>
<p>interfaceAnimal{</p>
<p>publicvoid eat();</p>
<p>publicvoid travel();</p>
<p>}</p>
<h2>Implementing Interfaces</h2>
<p>When a class implements an interface, you can think of the class as signing a contract, agreeing to perform the specific behaviors of the interface. If a class does not perform all the behaviors of the interface, the class must declare itself as abstract.</p>
<p>A class uses the&nbsp;<strong>implements</strong>&nbsp;keyword to implement an interface. The implements keyword appears in the class declaration following the extends portion of the declaration.</p>
<h3>Example</h3>
<p>/* File name : MammalInt.java */</p>
<p>publicclassMammalIntimplementsAnimal{</p>
<p>&nbsp;</p>
<p>publicvoid eat(){</p>
<p>System.out.println("Mammal eats");</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid travel(){</p>
<p>System.out.println("Mammal travels");</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicint noOfLegs(){</p>
<p>return0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>MammalInt m =newMammalInt();</p>
<p>m.eat();</p>
<p>m.travel();</p>
<p>}</p>
<p>}</p>
<p>This will produce the following result &minus;</p>
<h3>Output</h3>
<p>Mammal eats</p>
<p>Mammal travels</p>
<p>When overriding methods defined in interfaces, there are several rules to be followed &minus;</p>
<ul>
<li>Checked exceptions should not be declared on implementation methods other than the ones declared by the interface method or subclasses of those declared by the interface method.</li>
<li>The signature of the interface method and the same return type or subtype should be maintained when overriding the methods.</li>
<li>An implementation class itself can be abstract and if so, interface methods need not be implemented.</li>
</ul>
<p>When implementation interfaces, there are several rules &minus;</p>
<ul>
<li>A class can implement more than one interface at a time.</li>
<li>A class can extend only one class, but implement many interfaces.</li>
<li>An interface can extend another interface, in a similar way as a class can extend another class.</li>
</ul>
<h2>Extending Interfaces</h2>
<p>An interface can extend another interface in the same way that a class can extend another class. The&nbsp;<strong>extends</strong>&nbsp;keyword is used to extend an interface, and the child interface inherits the methods of the parent interface.</p>
<p>The following Sports interface is extended by Hockey and Football interfaces.</p>
<h3>Example</h3>
<p>// Filename: Sports.java</p>
<p>publicinterfaceSports{</p>
<p>publicvoid setHomeTeam(String name);</p>
<p>publicvoid setVisitingTeam(String name);</p>
<p>}</p>
<p>// Filename: Football.java</p>
<p>publicinterfaceFootballextendsSports{</p>
<p>publicvoid homeTeamScored(int points);</p>
<p>publicvoid visitingTeamScored(int points);</p>
<p>publicvoid endOfQuarter(int quarter);</p>
<p>}</p>
<p>// Filename: Hockey.java</p>
<p>publicinterfaceHockeyextendsSports{</p>
<p>publicvoid homeGoalScored();</p>
<p>publicvoid visitingGoalScored();</p>
<p>publicvoid endOfPeriod(int period);</p>
<p>publicvoid overtimePeriod(int ot);</p>
<p>}</p>
<p>The Hockey interface has four methods, but it inherits two from Sports; thus, a class that implements Hockey needs to implement all six methods. Similarly, a class that implements Football needs to define the three methods from Football and the two methods from Sports.</p>
<h2>Extending Multiple Interfaces</h2>
<p>A Java class can only extend one parent class. Multiple inheritance is not allowed. Interfaces are not classes, however, and an interface can extend more than one parent interface.</p>
<p>The extends keyword is used once, and the parent interfaces are declared in a comma-separated list.</p>
<p>For example, if the Hockey interface extended both Sports and Event, it would be declared as &minus;</p>
<h3>Example</h3>
<p>publicinterfaceHockeyextendsSports,Event</p>
<h2>Tagging Interfaces</h2>
<p>The most common use of extending interfaces occurs when the parent interface does not contain any methods. For example, the MouseListener interface in the java.awt.event package extended java.util.EventListener, which is defined as &minus;</p>
<h3>Example</h3>
<p>package java.util;</p>
<p>publicinterfaceEventListener</p>
<p>{}</p>
<p>An interface with no methods in it is referred to as a&nbsp;<strong>tagging</strong>&nbsp;interface. There are two basic design purposes of tagging interfaces &minus;</p>
<p><strong>Creates a common parent</strong>&minus; As with the EventListener interface, which is extended by dozens of other interfaces in the Java API, you can use a tagging interface to create a common parent among a group of interfaces. For example, when an interface extends EventListener, the JVM knows that this particular interface is going to be used in an event delegation scenario.</p>
<p><strong>Adds a data type to a class</strong>&minus; This situation is where the term, tagging comes from. A class that implements a tagging interface does not need to define any methods (since the interface does not have any), but the class becomes an interface type through polymorphism.</p>
<h1><u>Java - Packages</u></h1>
<p>Packages are used in Java in order to prevent naming conflicts, to control access, to make searching/locating and usage of classes, interfaces, enumerations and annotations easier, etc.</p>
<p>A&nbsp;<strong>Package</strong>&nbsp;can be defined as a grouping of related types (classes, interfaces, enumerations and annotations ) providing access protection and namespace management.</p>
<p>Some of the existing packages in Java are &minus;</p>
<ul>
<li><strong>lang</strong>&minus; bundles the fundamental classes</li>
<li><strong>io</strong>&minus; classes for input , output functions are bundled in this package</li>
</ul>
<p>Programmers can define their own packages to bundle group of classes/interfaces, etc. It is a good practice to group related classes implemented by you so that a programmer can easily determine that the classes, interfaces, enumerations, and annotations are related.</p>
<p>Since the package creates a new namespace there won't be any name conflicts with names in other packages. Using packages, it is easier to provide access control and it is also easier to locate the related classes.</p>
<h2>Creating a Package</h2>
<p>While creating a package, you should choose a name for the package and include a&nbsp;<strong>package</strong>&nbsp;statement along with that name at the top of every source file that contains the classes, interfaces, enumerations, and annotation types that you want to include in the package.</p>
<p>The package statement should be the first line in the source file. There can be only one package statement in each source file, and it applies to all types in the file.</p>
<p>If a package statement is not used then the class, interfaces, enumerations, and annotation types will be placed in the current default package.</p>
<p>To compile the Java programs with package statements, you have to use -d option as shown below.</p>
<p>javac -d Destination_folder file_name.java</p>
<p>Then a folder with the given package name is created in the specified destination, and the compiled class files will be placed in that folder.</p>
<h3>Example</h3>
<p>Let us look at an example that creates a package called&nbsp;<strong>animals</strong>. It is a good practice to use names of packages with lower case letters to avoid any conflicts with the names of classes and interfaces.</p>
<p>Following package example contains interface named&nbsp;<em>animals</em>&nbsp;&minus;</p>
<p>/* File name : Animal.java */</p>
<p>package animals;</p>
<p>&nbsp;</p>
<p>interfaceAnimal{</p>
<p>publicvoid eat();</p>
<p>publicvoid travel();</p>
<p>}</p>
<p>Now, let us implement the above interface in the same package&nbsp;<em>animals</em>&nbsp;&minus;</p>
<p>package animals;</p>
<p>/* File name : MammalInt.java */</p>
<p>&nbsp;</p>
<p>publicclassMammalIntimplementsAnimal{</p>
<p>&nbsp;</p>
<p>publicvoid eat(){</p>
<p>System.out.println("Mammal eats");</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicvoid travel(){</p>
<p>System.out.println("Mammal travels");</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicint noOfLegs(){</p>
<p>return0;</p>
<p>}</p>
<p>&nbsp;</p>
<p>publicstaticvoid main(String args[]){</p>
<p>MammalInt m =newMammalInt();</p>
<p>m.eat();</p>
<p>m.travel();</p>
<p>}</p>
<p>}</p>
<p>Now compile the java files as shown below &minus;</p>
<p>$ javac -d . Animal.java</p>
<p>$ javac -d . MammalInt.java</p>
<p>Now a package/folder with the name&nbsp;<strong>animals</strong>&nbsp;will be created in the current directory and these class files will be placed in it as shown below.</p>
<p>You can execute the class file within the package and get the result as shown below.</p>
<p>Mammal eats</p>
<p>Mammal travels</p>
<h2>The import Keyword</h2>
<p>If a class wants to use another class in the same package, the package name need not be used. Classes in the same package find each other without any special syntax.</p>
<h3>Example</h3>
<p>Here, a class named Boss is added to the payroll package that already contains Employee. The Boss can then refer to the Employee class without using the payroll prefix, as demonstrated by the following Boss class.</p>
<p>package payroll;</p>
<p>publicclassBoss{</p>
<p>publicvoid payEmployee(Employee e){</p>
<p>e.mailCheck();</p>
<p>}</p>
<p>}</p>
<p>What happens if the Employee class is not in the payroll package? The Boss class must then use one of the following techniques for referring to a class in a different package.</p>
<ul>
<li>The fully qualified name of the class can be used. For example &minus;</li>
</ul>
<p>payroll.Employee</p>
<ul>
<li>The package can be imported using the import keyword and the wild card (*). For example &minus;</li>
</ul>
<p>import payroll.*;</p>
<ul>
<li>The class itself can be imported using the import keyword. For example &minus;</li>
</ul>
<p>import payroll.Employee;</p>
<p><strong>Note</strong>&nbsp;&minus; A class file can contain any number of import statements. The import statements must appear after the package statement and before the class declaration.</p>
<h2>The Directory Structure of Packages</h2>
<p>Two major results occur when a class is placed in a package &minus;</p>
<ul>
<li>The name of the package becomes a part of the name of the class, as we just discussed in the previous section.</li>
<li>The name of the package must match the directory structure where the corresponding bytecode resides.</li>
</ul>
<p>Here is simple way of managing your files in Java &minus;</p>
<p>Put the source code for a class, interface, enumeration, or annotation type in a text file whose name is the simple name of the type and whose extension is&nbsp;<strong>.java</strong>.</p>
<p>For example &minus;</p>
<p>// File Name :&nbsp; Car.java</p>
<p>package vehicle;</p>
<p>&nbsp;</p>
<p>publicclassCar{</p>
<p>// Class implementation.&nbsp;&nbsp;</p>
<p>}</p>
<p>Now, put the source file in a directory whose name reflects the name of the package to which the class belongs &minus;</p>
<p>....\vehicle\Car.java</p>
<p>Now, the qualified class name and pathname would be as follows &minus;</p>
<ul>
<li>Class name &rarr; vehicle.Car</li>
<li>Path name &rarr; vehicle\Car.java (in windows)</li>
</ul>
<p>In general, a company uses its reversed Internet domain name for its package names.</p>
<p><strong>Example</strong>&nbsp;&minus; A company's Internet domain name is apple.com, then all its package names would start with com.apple. Each component of the package name corresponds to a subdirectory.</p>
<p><strong>Example</strong>&nbsp;&minus; The company had a com.apple.computers package that contained a Dell.java source file, it would be contained in a series of subdirectories like this &minus;</p>
<p>....\com\apple\computers\Dell.java</p>
<p>At the time of compilation, the compiler creates a different output file for each class, interface and enumeration defined in it. The base name of the output file is the name of the type, and its extension is&nbsp;<strong>.class</strong>.</p>
<p>For example &minus;</p>
<p>// File Name: Dell.java</p>
<p>package com.apple.computers;</p>
<p>&nbsp;</p>
<p>publicclassDell{</p>
<p>}</p>
<p>&nbsp;</p>
<p>classUps{</p>
<p>}</p>
<p>Now, compile this file as follows using -d option &minus;</p>
<p>$javac -d . Dell.java</p>
<p>The files will be compiled as follows &minus;</p>
<p>.\com\apple\computers\Dell.class</p>
<p>.\com\apple\computers\Ups.class</p>
<p>You can import all the classes or interfaces defined in&nbsp;<em>\com\apple\computers\</em>as follows &minus;</p>
<p>import com.apple.computers.*;</p>
<p>Like the .java source files, the compiled .class files should be in a series of directories that reflect the package name. However, the path to the .class files does not have to be the same as the path to the .java source files. You can arrange your source and class directories separately, as &minus;</p>
<p>&lt;path-one&gt;\sources\com\apple\computers\Dell.java</p>
<p>&nbsp;</p>
<p>&lt;path-two&gt;\classes\com\apple\computers\Dell.class</p>
<p>By doing this, it is possible to give access to the classes directory to other programmers without revealing your sources. You also need to manage source and class files in this manner so that the compiler and the Java Virtual Machine (JVM) can find all the types your program uses.</p>
<p>The full path to the classes directory, &lt;path-two&gt;\classes, is called the class path, and is set with the CLASSPATH system variable. Both the compiler and the JVM construct the path to your .class files by adding the package name to the class path.</p>
<p>Say &lt;path-two&gt;\classes is the class path, and the package name is com.apple.computers, then the compiler and JVM will look for .class files in &lt;path-two&gt;\classes\com\apple\computers.</p>
<p>A class path may include several paths. Multiple paths should be separated by a semicolon (Windows) or colon (Unix). By default, the compiler and the JVM search the current directory and the JAR file containing the Java platform classes so that these directories are automatically in the class path.</p>
<h2>Set CLASSPATH System Variable</h2>
<p>To display the current CLASSPATH variable, use the following commands in Windows and UNIX (Bourne shell) &minus;</p>
<ul>
<li>In Windows &rarr; C:\&gt; set CLASSPATH</li>
<li>In UNIX &rarr; % echo $CLASSPATH</li>
</ul>
<p>To delete the current contents of the CLASSPATH variable, use &minus;</p>
<ul>
<li>In Windows &rarr; C:\&gt; set CLASSPATH =</li>
<li>In UNIX &rarr; % unset CLASSPATH; export CLASSPATH</li>
</ul>
<p>To set the CLASSPATH variable &minus;</p>
<ul>
<li>In Windows &rarr; set CLASSPATH = C:\users\jack\java\classes</li>
<li>In UNIX &rarr; % CLASSPATH = /home/jack/java/classes; export CLASSPATH</li>
</ul>


<p><strong><u>Note</u></strong><strong>: </strong>You can dig deeper from here if you want to know more about Java.</p>
<p><u>https://www.tutorialspoint.com/java/java_data_structures.htm</u></p>


</br>

<p> <b> <XMP> Comparison of C, C++ and Java </XMP>               </b></p>

<ul>

<li> <XMP>C & C++ support pointers and structures while Java do not.</XMP> </li>
<li> <XMP>The code of C and C++ are directly converted into machine level language and it is executed while the code of Java is converted into Java byte codes and then it is converted into machine level language and it is executed.</XMP> </li> 
<li> <XMP>C uses scanf as input function to read the character or integer entered through the keyboard and printf as output function to print the output on the screen.</XMP> </li>
<li> <XMP>C++ uses cin as input function to read the character or integer entered through the keyboard and cout as output function to print the output on the screen.</XMP> </li>
<li> <XMP>But Java uses scan.nextInt() or scan.nextFloat() as input method to read the variable entered through the keyboard and System.out.println as output method to print the output on the screen.</XMP> </li>
<li> <XMP>Functions are in C & C++ whereas methods are in Java.</XMP> </li>
<li> <XMP>C & C++ are platform dependent whereas Java is platform independent (Code written in Java can be taken from one computer to the other without having to worry about system configuration details).</XMP> </li>
<li> <XMP>In C & C++, program instruction codes are written and executed within the body of main function main() where as in Java -- program instruction codes are written and executed within the body of main method public static void main(String[] args).</XMP> </li>
<li> <XMP>data types like int float, char are same in C, C++ & Java.</XMP> </li>
<li> <XMP>C is structured language whereas C++ & Java is object oriented language (i.e., C++ & Java has the extensive power and immense extensibility to write large scale complex programs).</XMP> </li>
<li> <XMP>Operators such as %d, %f & %c are used in C whereas no operators are used in C++ & Java.</XMP> </li>
<li> <XMP>A program written in Java usually requires more memory space than the same program written in C & C++.</XMP> </li>
<li> <XMP>Java provides both high speed and high performance and reliability, flexibility and seamless integration with other frameworks and technologies -- compared to C & C++.</XMP> </li>
<li> <XMP>Java supports multithreading (a process of executing several codes concurrently) while C & C++ do not.</XMP> </li>




</ul>


</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>Thinking in Java </xmp></center></td>
                <td><center><xmp>Bruce Eckel</xmp></center></td>
                <td><a href="img/pdf34.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>Java For Dummies</xmp></center></td>
                <td><center><xmp>Barry Burd</xmp></center></td>
                <td><a href="img/pdf35.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Java: The Complete Reference </xmp></center></td>
                <td><center><xmp>Herbert Schildt </xmp></center></td>
                <td><a href="img/pdf36.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Head First Java</xmp></center></td>
                <td><center><xmp>Kathy Sierra</xmp></center></td>
                <td><a href="img/pdf37.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Java in a Nutshell</xmp></center></td>
                <td><center><xmp>Benjamin J. Evans</xmp></center></td>
                <td><a href="img/pdf38.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>The Java Language Specification</xmp></center></td>
                <td><center><xmp> James Gosling</xmp></center></td>
                <td><a href="img/pdf39.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Java How to Program</xmp></center></td>
                <td><center><xmp>Paul Deitel</xmp></center></td>
                <td><a href="img/pdf40.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp> Java</xmp></center></td>
                <td><center><xmp> TutorialsPoint</xmp></center></td>
                <td><a href="img/pdf41.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Programming with Java</xmp></center></td>
                <td><center><xmp>E. Balagurusamy</xmp></center></td>
                <td><a href="img/pdf42.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>Effective Java</xmp></center></td>
                <td><center><xmp>Joshua Bloch</xmp></center></td>
                <td><a href="img/pdf43.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Java Threads</xmp></center></td>
                <td><center><xmp>Scott Oaks</xmp></center></td>
                <td><a href="img/pdf44.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>



</br>










</div>
</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>



<div id="code40">
<h3>  <center> Linux</center>      </h3>

</br>
<center> <img src="images/li.jpg" alt="Smiley face" height="157" width="320"> </center>
</br>


<XMP>


                                                                           Introduction

Every desktop computer uses an operating system. The most popular operating systems in use today are: Windows, Mac OS, and LINUX. 
Linux is the best-known notoriously reliable and highly secure open source portable operating system -- very much like UNIX -- that has become 
very popular over the last several years -- originally created as a labor of love by Linus Torvalds -- computer science student at the University 
of Helsinki in Finland -- in the early 1990s and later developed by more than a thousand people around the world. Linux is fast, free and easy to use, 
that sits underneath all of the other software on a computer -- runs your computer -- handling all interactions between you and the hardware i.e., 
whether you're typing a letter, calculating a money budget, or managing your food recipes on your computer, the Linux operating system 
(similar to other Operating Systems, such as Windows XP, Windows 7, Windows 8, and Mac OS X) provides the essential air that your computer breathes. 
Linux is the most important technology advancement of the twenty-first century and Licensed under the General Public License (GPL) that Linux uses 
ensures that the software will always be open to anyone and whose source code is open and available for any user to review, which makes it easier 
to identify and repair vulnerabilities and it power the laptops, development machines and servers at Google, Facebook, Twitter, NASA, and New York 
Stock Exchange, just to name a few. Linux has many more features to amaze its users such as: Live CD/USB, Graphical user interface (X Window System) etc.


                                                                           Why LINUX?

Although Microsoft Windows (which is the most likely to be the victim of viruses and malware) has made great improvements in reliability in recent years, 
it is considered less reliable than Linux. Linux is notoriously reliable and secure and it is free from constant battling viruses and 
malware (which may affect your desktops, laptops, and servers by corrupting files, causing slow downs, crashes, costly repairs and taking 
over basic functions of your operating system) â€“ and it keep yourself free from licensing fees i.e., zero cost of entry ... as in free. 
You can install Linux on as many reliable computer ecosystems on the planet as you like without paying a cent for software or server licensing. 
While Microsoft Windows usually costs between $99.00 and $199.00 USD for each licensed copy and fear of losing data.

Below are some examples of where Linux is used today:
 1. Android phones and tablets
 2. Servers
 3. TV, Cameras, DVD players, etc.
 4. Amazon
 5. Google
 6. U.S. Postal service
 7. New York Stock Exchange


                                                                     Basic LINUX COMMANDS
										
																		
1.	$date â†’ display date and time
2.	$cal â†’ display calendar
3.	$date & cal â†’ display date , time and calendar
4.	$cal 8 2016 â†’ display August month 2016 year calendar
5.	$clear â†’ clear the screen
6.	$exit â†’ exit and get to login page
7.	$free â†’ displays information about RAM and swap space usage, showing the total and the used amount in both categories
8.	$free   -b â†’ displays the output in bytes
9.	$free   -k â†’ displays the output in kilobytes
10.	$free   -m â†’ displays the output in megabytes
11.	$passwd â†’ change password
12.	$uname â†’ display the name of the current operating system
13.	$echo "Hello World" â†’ print the word Hello World
14.	$hostname â†’ display the Kernel version
15.	$echo " my username is $USER " â†’ print the output: my username is root
16.	$shutdown â†’ shutdown the operating system
17.	$logname â†’ display the username
18.	$whoami â†’ display the username
19.	The commands: $logname and $whoami display the username
20.	$echo 'a =20; b =64; print (a+b)' | python â†’ print the output: 84
21.	$echo 'a =56; b =2; print (a / b)' | python â†’ print the output: 28
22.	$echo 'a =6; b =2; print (a * b)' | python â†’ print the output: 12
23.	$echo 'a =6; b =2; print (a - b)' | python â†’ print the output: 4
24.	$echo 'a =5; print (pow(a,2))' | python â†’ print the output: 25
25.	$echo 'a =4; print (format(a**0.5)) ' | python â†’ print the output: 2.0 (find square root)
26.	$date -- set 1998-11-02 â†’ to set current date as 02 Nov 1988
27.	$date -- set 12:11:02 â†’ to set current time as 12:11:02 IST
28.	$printf "hi computer" â†’ print the output: hi computer
29.	$du â†’ display the information of disk usage of files and directories
30.	$who â†’ display the user details
31.	$ifconfig â†’ view and change the configuration of the network interfaces on your system
32.	$pwd â†’ display the present working directory
33.	$uname  -a â†’ display the system architecture information
34.	$hostname  -i â†’ display the IP address of the hostname
35.	$ls â†’ display the list of files
36.	$ps â†’ display the process information
37.	$uptime â†’ display the system running information
38.	$netstat  -a â†’ display all ports (both TCP and UDP)
39.	$netstat  -at â†’ display only TCP (Transmission Control Protocol) port connections
40.	$netstat  -au â†’ display only UDP (User Datagram Protocol ) port connections
41.	$netstat  -I â†’ display all active listening ports connections
42.	$netstat  -It â†’ display all active listening TCP ports
43.	$netstat  -lu â†’ display all active listening UDP ports
44.	$netstat  -lx â†’ display all active UNIX listening ports
45.	$ifconfig â†’ display all the active interfaces details
46.	$ifconfig   -a â†’ display information of all network interfaces
47.	$df â†’ displays information about the total disk space, the disk space currently in use, and the free space on all the mounted drives
48.	$df   -H â†’ display the number of occupied blocks in gigabytes, megabytes, or kilobytes
49.	$du   -a â†’ displays the size of each individual file
50.	$du   -s â†’ displays only the calculated total size
51.	$top â†’ provides a quick overview of the currently running processes
52.	$shutdown   -h now â†’ shutdown the system and turn the power off immediately
53.	$shutdown   -h +10 â†’ shutdown the system after 10 minutes
			
										
While lots of organizations, corporations, and individuals have already been convinced for 20 years now that this is the way to go -- 
private users, training companies, universities, research centers, and commercial vendors needed applications like the Internet 
to make them realize they can profit from Open Source. Now Linux (successfully being used by several millions of users worldwide) 
has grown past the stage where it was almost exclusively an academic system, useful only to a handful of people with a technical background. 
It provides more than the operating system: there is an entire infrastructure supporting the chain of effort of creating an operating system, 
of making and testing programs for it, of bringing everything to the users, of supplying maintenance, updates and support and customizations, 
runs on numerous different platforms including the Intel and Alpha platform. Today, Linux is ready to accept the challenge of a fast-changing world 
to do various types of operations, call application programs etc.


</XMP>



</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>Linux Shell Scripting Tutorial </xmp></center></td>
                <td><center><xmp>Vivek G Gite</xmp></center></td>
                <td><a href="img/pdf45.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>Beginning Linux Programming</xmp></center></td>
                <td><center><xmp>Neil Matthew</xmp></center></td>
                <td><a href="img/pdf46.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Linux From Scratch </xmp></center></td>
                <td><center><xmp>Gerard Beekmans </xmp></center></td>
                <td><a href="img/pdf47.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Linux: a Portable Operating System</xmp></center></td>
                <td><center><xmp>Linus Torvalds</xmp></center></td>
                <td><a href="img/pdf48.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Linux For Dummies</xmp></center></td>
                <td><center><xmp>Richard Blum</xmp></center></td>
                <td><a href="img/pdf49.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Linux Pocket Guide</xmp></center></td>
                <td><center><xmp> Daniel J. Barrett</xmp></center></td>
                <td><a href="img/pdf50.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>The Linux Cookbook</xmp></center></td>
                <td><center><xmp>Michael Stutz</xmp></center></td>
                <td><a href="img/pdf51.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp> Linux Fundamentals</xmp></center></td>
                <td><center><xmp> Paul Cobbaut</xmp></center></td>
                <td><a href="img/pdf52.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Linux in a Nutshell</xmp></center></td>
                <td><center><xmp>Ellen Siever</xmp></center></td>
                <td><a href="img/pdf53.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>Linux Bible</xmp></center></td>
                <td><center><xmp>Christine Bresnahan</xmp></center></td>
                <td><a href="img/pdf54.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Sams Teach Yourself Linux in 24 Hours</xmp></center></td>
                <td><center><xmp>Stephen Smoogen</xmp></center></td>
                <td><a href="img/pdf55.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>



</br>



</div>

</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>


<div id="code41">
<h3>  <center> Python</center>      </h3>

</br>
<center> <img src="images/py.png" alt="Smiley face" height="203" width="603"> </center>
</br>


<XMP>
Python is a popular, very powerful high-level language (like C, C++, Perl, and Java â€“ and its name is derived from "Monty Python's Flying Circus" â€“ 
a British television series), object-oriented programming scripting language designed by Dutch programmer "Guido van Rossum" in the early 1990s 
(often referred to as a "glue" language, meaning that it is capable to work in mixed-language environment) which is easy to understand, 
easy to use, write, modify and debug and flexible and easy to implement and run on open source operating systems  like Linux, Windows, 
Macintosh, Solaris, FreeBSD, OS/2, Amiga, AROS, AS/400 and is employed to perform automated testing of applications 
(i.e., to execute tests of applications, report outcomes and compare results with earlier test runs) and to increase the effectiveness and speed of 
software testing and its other commercial uses include financial applications, educational software, games, production of special effects for such 
movies as The Phantom Menace and The Mummy Returns, and business software. And python might not be the best choice for building the following types of 
applications and systems: Graphics-intensive applications, such as action games -- where performance is important (because it is true that 
CODE WRITTEN IN Python, c# and visual basic etc. is far slower than the same code write in C++. Hence, C++ is necessarily preferred). 
And its support for Matlab-like array manipulation and plotting is a major reason to prefer it over other high level programming languages such as 
Perl and Ruby.
  

A simple python program to print the word "Hello World! " on screen:

# Hello World program in Python
print "Hello World!\n"

Output on the screen:
                                                   Hello World!

print "Hello World!\n" --> implies the statement that make provision to print: 
                                                   Hello World!
on the screen. 

# Hello World program in Python  â†’ the statement that implies: comment 


What will be the output on the screen:

(a)
print "Hello World!\n"
print "Hello World!\n"

Answer:
Hello World!
Hello World!

(b)

print "Hello World!"
print "Hello World!"

Answer:
Hello World! Hello World!


What is the mistake in the following program:

Hello World program in Python
print "Hello World!\n"

Answer:
                      # is not added to the statement:
Hello World program in Python

//---------------------------------------------------------------------------------------------------------------------------

#Hello World program in Python
print "Hello World!\n"
----------------------------------------------------------------------------------------------------------------------------//

Program 1.1

Python  program to add two numbers:

number1=2
number2=3
print "The sum of {0} and {1} is {2}".format(number1, number2, float (number1) + float (number2))

Output on the screen:
                                           The sum of 2 and 3 is 5.0

print "The sum of {0} and {1} is {2}".format(number1, number2, float (number1) + float (number2)) --> implies the statement that make provision to print the output: 
                                            The sum of 2 and 3 is 5.0
on the screen.

Note: 
If  you replace the statement: 
print "The sum of {0} and {1} is {2}".format(number1, number2, float (number1) + float (number2))
by the statement: 
print "The sum of {1} and {2} is {3}".format(number1, number2, float (number1) + float (number2))
Then 
                                     Runtime error or IndexError: tuple index out of range
will be displayed on the screen.

Note: 

Dot notation (.) in the statement: 
print "The sum of {0} and {1} is {2}".format(number1, number2, float (number1) + float (number2))
connects the two statements:
1.	"The sum of {0} and {1} is {2}"
2.	format(number1, number2, float (number1) + float (number2))

And if you forget to write dot notation in the statement: 
print "The difference of {0} and {1} is {2}" .format(number1, number2, float (number1) - float (number2))
i.e.,
print "The difference of {0} and {1} is {2}" format(number1, number2, float (number1) - float (number2))

Then 
Syntax error
will be displayed on the console screen.

In the statement: 

print "The sum of {0} and {1} is {2}".format(number1, number2, float (number1) + float (number2))

	{0} --> act as a placeholder for number1 in the format method
	{1} --> act as a placeholder for number2 in the format method
	{2} --> act as a placeholder for float (number1) + float (number2) in the format method

If you want to enter the values for number1 and number2 through keyboard, then you need to replace the statements: 
number1 = 2
number2 = 3
by the statements: 
                 number1=input(" Please Enter the First Number: ")
                 number2=input(" Please Enter the Second Number: ")

i.e., the above program should be rewritten as:
number1=input(" Please Enter the First Number: ")
number2=input(" Please Enter the Second Number: ")
print "The sum of {0} and {1} is {2}".format(number1, number2, float (number1) + float (number2))

Output on the screen:
Please Enter the First Number: 
If you enter 1 
Please Enter the Second Number: 
If you enter 2  
The sum of 1 and 2 is 3.0
will be displayed on the screen.  

Statements:

number1=input(" Please Enter the First Number: ")
number2=input(" Please Enter the Second Number: ")
ask the user to enter two integer numbers and stores the user entered values in variables number 1 and number 2.

Program 1.2

Python program to subtract two numbers: 

number1=input(" Please Enter the First Number: ")
number2=input(" Please Enter the Second Number: ")
print "The difference of {0} and {1} is {2}".format(number1, number2, float (number1) - float (number2))

Output on the screen:
Please Enter the First Number: 
If you enter 6
Please Enter the Second Number: 
If you enter 4 
The difference of 6 and 4 is 2.0
will be displayed on the screen. 

Program 1.3

Python program to divide two numbers:

number1=input(" Please Enter the First Number: ")
number2=input(" Please Enter the Second Number: ")
print "The division of {0} by {1} yields {2}".format(number1, number2, float (number1) / float (number2))

Output on the screen:
Please Enter the First Number: 
If you enter 6
Please Enter the Second Number: 
If you enter 2
The division of 6 by 2 is 3.0
 will be displayed on the screen. 

Program 1.4

Python program to multiply two numbers:
number1=input(" Please Enter the First Number: ")
number2=input(" Please Enter the Second Number: ")
print "The product of {0} and {1} is {2}".format(number1, number2, float (number1) * float (number2))

Output on the screen:
Please Enter the First Number: 
If you enter 6
Please Enter the Second Number: 
If you enter 2
The product of 6 and 2 is 12.0
will be displayed on the screen. 

Program 1.5
Python program to find the area of a circle:

number1=input(" Please Enter the radius: ")
print "The area of the circle is {0}".format(4*3.14* number1* number1)

Output on the screen:
Please Enter the radius: 
If you enter 2
The area of the circle is 50.24
will be displayed on the screen. 

Program 1.6

Python program to find the square root of a number:

number1=input(" Please Enter the number: ")
print "The square root of the entered number is {0}".format(number1 ** 0.5)

Output on the screen:
Please Enter the number: 
If you enter 4
The square root of the entered number is 2.0  will be displayed on the screen. 
1/2=0.5
** â†’ implies: exponent operator
number1 ** 0.5 â†’ implies:
number1 ** 1/2 (which implies number1 to the power of 1/2 )

Program 1.7

Python program to find the square of a number

number1=input(" Please Enter the number: ")
print "The square of the entered number is {0}".format(number1 * number1)

Output on the screen:
Please Enter the number: 
If you enter 4
The square of the entered number is 16.0
 will be displayed on the screen. 

Program 1.8

Python program to find the incremented and decremented values of the entered number:

number1=input(" Please Enter the number: ")
print "The increment of the entered number is {0}".format(number1 +1)
print "The decrement of the entered number is {0}".format(number1 - 1)

Output on the screen:
Please Enter the number: 
If you enter 6
The increment of the entered number is 7
The decrement of the entered number is 5
will be displayed on the screen

What will be the output of the following programs:

(a)

x = 13
if x < 10:
 print ("Good morning")
elif x<12: 
 print ("Soon time for lunch")
elif x<18: 
  print ("Good day")
elif x<22: 
 print ("Good evening")
else: 
  print ("Good night")

Answer:
                                Good day

(b)

n1 = [0 for i in range(15)]
print (n1)

Answer:
                      [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]

If you replace the statement: 
n1 = [0 for i in range(15)]
by the statement: 
n1 = ["computer" for i in range(15)]

Then the output on the screen is:

['computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer', 'computer']

(c)

for k in range(1,10):
    print(k)

Answer:
1
2
3
4
5
6
7
8
9

If the statement:
for k in range(1,10):

by the statement:
for k in range(0,10):

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

If the statement: 
print(k)

is replaced by the statement:
print("computer")
i.e., 
for k in range(0,10):
print("computer")
Then the output on the screen is:
computer
computer
computer
computer
computer
computer
computer
computer
computer
computer


(d)

for day in ["Sunday","Monday","Tuesday","Wednesday","Thursday", "Friday","Saturday"]:
    print(day)
Answer:
Sunday
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday

(e)
n = 10
sum = 0
for i in range(1,n): sum = sum + i
print sum

Answer:
45

                                        range(1,n) means: generate integers starting from 1 up to, but not including, n.

How the execution takes place?

i=1 (sum = 0 because the sum is initialized to 0 in the statement  sum = 0)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 0 +1 =1
Now
i=2 (now the sum = 1)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 1 +2 =3
Now
i=3 (now the sum = 3)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 3 +3 = 6
Now
i=4 (now the sum = 6)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 6 + 4= 10
Now
i=5 (now the sum = 10)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 10 + 5= 15
Now
i=6 (now the sum = 15)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 15 + 6 = 21
Now
i=7 (now the sum = 21)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 21 + 7 = 28
Now
i=8 (now the sum = 28)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 28 + 8 = 36
Now
i=9 (now the sum = 36)
Is i in range(1,n) true?
Yes, do this 
sum = sum + i = 36 + 9 = 45
stops because range(1,n) means: generate integers starting from i=1 up to, but not including, i=10.

If you want to enter the value for n through the keyboard, then the above program should take the form:

n =input("Please Enter the number:")
sum = 0
for i in range(1,n): sum = sum + i
print sum

Output on the screen:
Please Enter the number:
If you enter 10
Then 45 will be outputted on the console screen.

(f)

for k in range(1,11):
    print("5 x {0} = {1}".format(k, 5*k))

Answer:

5 x 1 = 5                                                                                                                                                                       
5 x 2 = 10                                                                                                                                                                      
5 x 3 = 15                                                                                                                                                                      
5 x 4 = 20                                                                                                                                                                      
5 x 5 = 25                                                                                                                                                                      
5 x 6 = 30                                                                                                                                                                      
5 x 7 = 35                                                                                                                                                                      
5 x 8 = 40                                                                                                                                                                      
5 x 9 = 45                                                                                                                                                                      
5 x 10 = 50  

If you replace the statement:
for k in range(1,11):
by the statement:
for k in range(0,11):
Then the output on the screen is:

5 x 0 = 0
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50

</XMP>




</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>Python for Kids </xmp></center></td>
                <td><center><xmp>Jason R. Briggs</xmp></center></td>
                <td><a href="img/pdf56.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>Dive Into Python</xmp></center></td>
                <td><center><xmp>Mark Pilgrim</xmp></center></td>
                <td><a href="img/pdf57.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Programming Python </xmp></center></td>
                <td><center><xmp>Mark Lutz </xmp></center></td>
                <td><a href="img/pdf58.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Learning Python</xmp></center></td>
                <td><center><xmp>Mark Lutz</xmp></center></td>
                <td><a href="img/pdf59.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Head First Python</xmp></center></td>
                <td><center><xmp>Paul Barry</xmp></center></td>
                <td><a href="img/pdf60.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Learn Python the Hard Way</xmp></center></td>
                <td><center><xmp> Zed A. Shaw</xmp></center></td>
                <td><a href="img/pdf61.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>The Quick Python Book</xmp></center></td>
                <td><center><xmp>Vernon L. Ceder</xmp></center></td>
                <td><a href="img/pdf62.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp> Python Essential Reference</xmp></center></td>
                <td><center><xmp> David Beazley</xmp></center></td>
                <td><a href="img/pdf63.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Python in a Nutshell</xmp></center></td>
                <td><center><xmp>Alex Martelli</xmp></center></td>
                <td><a href="img/pdf64.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>Python Pocket Reference</xmp></center></td>
                <td><center><xmp>Mark Lutz</xmp></center></td>
                <td><a href="img/pdf65.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Python For Dummies</xmp></center></td>
                <td><center><xmp>Stef Maruch</xmp></center></td>
                <td><a href="img/pdf66.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>



</br>






















</div>


</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>



<div id="code42">
<h3>  <center> PHP</center>      </h3>

</br>
<center> <img src="images/ph.jpg" alt="Smiley face" height="168" width="300"> </center>
</br>


<XMP>


PHP / Hypertext Preprocessor (designed by  an Greenlandic-Danish programmer "Rasmus Lerdorf" in 1994 âˆ’ as an efficient alternative to other scripting languages like Ruby, Perl  and Microsoftâ€™s ASP) is an relatively free (not licensed by a major corporation) popular efficient server side programming language (and  relatively easy one to master and quick to learn) that carries out common website duties like accepting passwords, authenticating users, and managing forum posts and guest books.

  


A simple PHP program to print the word "Hello World!" on screen:

<?php
echo "Hello World!";
?>

In the above example:

<?php
                       and ?> denote: opening and closing tags within which the execution of php codes takes place.

echo "Hello World!"; --> denote: the statement that makes provision to print the output:
Hello World!

on the screen.

Even If you replace the statement: 
                                         echo "Hello World!";

by the statement: 
                                        print "Hello World!";

i.e.,

<?php
print "Hello World!";
?>

There will be no change in the output on the screen (i.e., echo and print are more or less the same. They are both used to output data to the console  screen). 

If replace the opening tag <?php  by <?

Then the output on the screen is:

<?                                                                                                                                                                              
print "Hello World!";                                                                                                                                                           
?>

i.e., the entire program will be reflected on the console screen.

Even if you write the statement: 

print ( "Hello World!");

instead of the statement: 

print "Hello World!";

There will be no change in the output on the screen. 

 Note: Even if you omit the closing tag 
                                                ?>
in the above program. There will be no change in the output on the screen. But sometimes it reflects error. So omission of  ?> is discouraged.

Program 1.1

a)

<?php
echo "Hello World!";
echo "Hello World!";
?>

Output on the screen:

Hello World!Hello World!

b)

<?php
echo "\n Hello World!";
echo "\n Hello World!";
?>

Output on the screen:

Hello World!   
Hello World!

c)   

<?php
echo "Hello World!";
echo "\t Hello World!";
?>

Output on the screen:

Hello World!     Hello World!


Program 1.2

PHP program to add two numbers: 

<?php
  $num1 =1;
  $num2=5;
  $sum = $num1 + $num2;
  echo "Sum of the two numbers is : $sum";
   ?>

Output on the screen:
Sum of the two numbers is : 6

Equal sign implies: storage operator.

The statements:
$num1 =1;
$num2=5;
$sum = $num1 + $num2;
 imply: that we are creating the variables  $num1, $num2 and $sum and storing the values for created variables (i.e., 1 for $num1, 5 for $num1 and $sum for $num1 + $num2).

The statement: 
echo "Sum of the two numbers is : $sum";
make provision to print the output:
                               Sum of the two numbers is : 6 (which is 1+5)
on the screen.

Note: 

Suppose if you omit the $ symbol before a variable name (whose purpose is to make it clear that the word following the symbol $ is a variable âˆ’ the symbol $ distinguishes variables from other things) in the above program i.e., if you rewrite the above program as:

<?php
  num1 =1;
  num2=5;
  sum = num1 + num2;
   echo "Sum of the two numbers is : sum";
 ?>

Then 
                                    PHP Parse error:  syntax error, unexpected '='
will be displayed on the console screen.

If you want to supply the integer values for $num1 and $num2 through the key board, then the statements:
$num1 =1;
$num2=5;
should be  replaced by the statements:

echo "Please enter the first number : ";
fscanf(STDIN, â€œ%d\nâ€, $num1);
echo "Please enter the second number : ";
fscanf(STDIN, â€œ%d\nâ€, $num2);
i.e.,
<?php
echo "Please enter the first number : ";
fscanf(STDIN, "%d\n", $num1);
echo "Please enter the second number : ";
fscanf(STDIN, "%d\n", $num2);
$sum = $num1 + $num2;
echo "Sum of the two numbers is : $sum";
?>

Output on the screen:
Please enter the first number :
If you enter 5
Please enter the second number :
If you enter 6
Sum of the two numbers is: 11 will be outputted on the screen. 

	fscanf(STDIN, "%d\n", $num1); â†’ denote: the statement that make provision to enter a integer value for $num1 through the keyboard.
	fscanf(STDIN, "%d\n", $num2); â†’ denote: the statement that make provision to enter a integer value for $num2 through the keyboard.

Format string %d in the statement: 
fscanf(STDIN, "%d\n", $num1);
or in the statement: 
fscanf(STDIN, "%d\n", $num2);
tells the input function fscanf() to read the number entered through the keyboard (which is a integer) and STDIN (which stands for Standard input) means feed the number entered through the keyboard into the program.

	If you want to enter the floating values (say 1.6 & 1.9) for $num1 and $num2, then your program should take the form:

 <?php
echo "Please enter the first number : ";
fscanf(STDIN, "%f\n", $num1);
echo "Please enter the second number : ";
fscanf(STDIN, "%f\n", $num2);
$sum = $num1 + $num2;
echo "Sum of the two numbers is : $sum";
?>

Output on the screen:
Please enter the first number :
If you enter 1.6
Please enter the second number :
If you enter 1.9
Sum of the two numbers is: 3.5 
will be outputted on the screen. 

Program 1.3

PHP program to subtract two numbers: 

<?php
  $num1 =5;
  $num2=1;
  $sub = $num1 - $num2;
   echo "difference of the two numbers is : $sub";
   ?>

Output on the screen:
difference of the two numbers is : 4

Program 1.4

PHP program to divide two numbers: 

<?php
  $num1 =6;
  $num2=2;
  $div = $num1 / $num2;
   echo "the division of two numbers is : $div";
   ?>

Output on the screen:
the division of two numbers is : 3

Program 1.5

PHP program to multiply two numbers: 

<?php
  $num1 =6;
 $num2=2;
 $mult = $num1 * $num2;
 echo "the product of two numbers is : $mult";
  ?>
	
Output on the screen:

the product of two numbers is : 12

Program 1.6

PHP program to find the area of a circle:
 
<?php
$radius = 2.0;
$pi = 3.14159;
$area = $pi * $radius * $radius;
echo("\n radius = $radius centimeter");
echo("\n area = $area centimeter square");
?>

Output on the screen:

radius = 2 centimeter
area = 12.56636 centimeter square


Program 1.7

PHP program to find the square root of a number

<?php
$num1 = 4.0;
$num2 = sqrt($num1);
echo("The square root of a number = $num2");
?>

Output on the screen:

The square root of a number = 2

Program 1.8

PHP program to find the square of a number

<?php
$num1 = 2.0;
$num2 = $num1 * $num1;
echo("\n the square of a number = $num2");
?>

Output on the screen:

the square of a number = 4


If the statement:
$num2 = $num1 * $num1;
is replaced by:
$num2 = pow(($num1), 2);

i.e., if the above program is rewritten as:

<?php
$num1 = 2.0;
$num2 = pow(($num1), 2);
echo("\n the square of a number = $num2");
?>

Then  there will be no change in the output on the screen i.e.,
the square of a number = 4 
will be outputted on the screen.
Which means:
$num2 = pow(($num1), 2); is the same as $num2 = $num1 * $num1;


Program 1.9

PHP program to find the cube root of a number

<?php
$num1 = 6.0;
$num2 = pow(($num1), 1/3);
echo("\n the cube root of a number = $num2");
?>

Output on the screen:

the cube  root of a number = 1.8171205928321


Program 2.0

PHP program to round off a number

<?php
$num1 = 4.5;
$num2 = round ($num1);
echo("\n the round off of a number = $num2");
?>

Output on the screen:

the round off of a number = 5


Program 2.1

PHP program to find the incremented and decremented values of two numbers.

<?php
$num1 =2;
$num2=3;
$num3 = $num1 +1;
$num4 = $num1 - 1;
$num5 = $num2 +1;
$num6 = $num2 - 1;
echo ("\n The incremented value of  $num1 = $num3 ");
echo ("\n The decremented value of  $num1 = $num4 ");
echo ("\n The incremented value of  $num2 = $num5 ");
echo ("\n The decremented value of  $num2 = $num6 ");
?>

Output on the screen:

The incremented value of  2 = 3
The decremented value of  2 = 1
The incremented value of  3 = 4
The decremented value of  3 = 2

 
Program 2.2

PHP program to find the greatest of two numbers using if â€“ else statement

The syntax of if â€“ else statement is:

if (this condition is true)
{
print this statement;
}
else
{
print this statement;
}

<?php
$x = 4.5;
$y=5;
if($x>$y){
echo (" x is greater than y");
} else {
echo (" y is greater than x");
}
?>

Output on the screen:

y is greater than x


Note:  if the above program is rewritten as:

<?php
$x = 4.5;
$y=5;
if($x>$y){
echo (" $x is greater than $y");
} else {
echo (" $y is greater than $x");
}
?>

Then the output on the screen:

5 is greater than 4.5

Program 2.3

PHP program to find the greatest of three numbers using if â€“else if â€“ else statement

The syntax of if â€“else if â€“ else statement is:

if (this condition is true)
{
print this statement;
}
else if(this condition is true)
{
print this statement;
}
else
{
print this statement;
}

<?php
$x = 4.5;
$y=5;
$z=6;
if($x>$y && $x>z){
echo (" $x is greater than $y and $z");
} else if ($y>$z && $y>x){
echo (" $y is greater than $x and $z");
}
else 
{
echo (" $z is greater than $x and $y");
}
?>

Output on the screen:
6 is greater than 4.5 and 5


Program 2.4

PHP program to print the first ten natural numbers using for loop statement

<?php
for ($i=1; $i<=10; $i++)
echo (" \n $i");
?>

Output on the screen:

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
            
for ($i=1; $i<=10; $i++) denote the for loop statement for PHP and the syntax of the for loop statement is:
for (initialization; condition; increment)
Here:
$i=1 denote initialization (i.e., from where to start)
$i<=10 denote the condition (i.e., stop when the number 10 is reached)
$i++ imply increment (which tells the value of $i to increase by 1 each time the loop is executed) and $i++ is the same as $i+1.
Since the initialization i.e., $i=1
The statement:
echo (" \n $i");
make provision to print the output:
1
on the screen.

After this, the following execution takes place:
Now,
$i= 1
Is the condition ($i<=10) is true?
Yes because $i=1 
Do this
$i= 1+1 = 2
The statement 
echo (" \n $i");
make provision to print the output:
2
Now,
$i= 2
Is the condition ($i<=10) is true?
Yes because $i=2 
Do this
$i= 2+1 = 3
The statement 
echo (" \n $i");
make provision to print the output:
3
Now,
$i= 3
Is the condition ($i<=10) is true?
Yes because $i=3
Do this
$i= 3+1 = 4
The statement 
echo (" \n $i");
make provision to print the output:
4
Now,
$i= 4
Is the condition ($i<=10) is true?
Yes because $i=4
Do this
$i= 4+1 = 5
The statement
echo (" \n $i");
make provision to print the output:
5
Now,
$i= 5
Is the condition ($i<=10) is true?
Yes because $i=5
Do this
$i= 5+1 = 6
The statement 
echo (" \n $i");
make provision to print the output:
6
Now,
$i= 6
Is the condition ($i<=10) is true?
Yes because $i=6
Do this
$i= 6+1 = 7
The statement 
echo (" \n $i");
make provision to print the output:
7
Now,
$i= 7
Is the condition ($i<=10) is true?
Yes because $i=7
Do this
$i= 7+1 = 8
The statement
echo (" \n $i");
make provision to print the output:
8
Now,
$i= 8
Is the condition ($i<=10) is true?
Yes because $i=8
Do this
$i= 8+1 = 9
The statement 
echo (" \n $i");
make provision to print the output:
9
Now,
$i= 9
Is the condition ($i<=10) is true?
Yes because $i=9
Do this
$i= 9+1 = 10
The statement
echo (" \n $i");
 make provision to print the output:
10
stop because the condition $i<=10 is achieved.

If you replace the statement 
for ($i=1; $i<=10; $i++)
by the statement 
for ($i=1; $i==10; $i++)

Then there will be no display of output on the screen.

If the statement 
for ($i=1; $i<=10; $i++)
is replaced by the statement 
for ($i=1; $i=10; $i++)

Then the output on the screen is:
10
10
10
10
10
10
10
10
10
10
10
10
10 â€¦â€¦ continues


Program 2.5

PHP program to print the first ten natural numbers using while loop statement

The syntax of while loop statement is:

while (this is the condition)
{
execute this statement;
}

<?php  
$i = 1;
while($i <= 10) {
echo "\n  $i ";
$i++;
} 
?>  

Output on the screen:
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


Program 2.6

PHP program to print the first nine natural numbers using do while loop statement

The syntax of do while loop statement is:

do
{
execute this statement;
}
while(this is the condition);


<?php  
$i = 1;
 do {
  echo "\n $i ";
  $i++;
} while($i <= 9);
?>  

Output on the screen:
1
2
3
4
5
6
7
8
9

Program 2.7

PHP program to print the average of the first10 numbers using for loop statement

<?php
$i; 
$avg; 
$sum = 0;
for( $i=1; $i<=10; $i++)
$sum = $sum + $i;
$avg = $sum/10;
echo "\n sum of the first 10 numbers = $sum ";
echo"\n average of the first 10 numbers = $avg  ";
?>

Output on the screen:

sum of the first 10 numbers = 55
average of the first 10 numbers = 5.5


Program 2.8

Switch case method

a)

<?php
  $ch ='3';
switch($ch)
{
case '1':
echo "Red";
break;
case '2':
echo "White";
break;
case '3':
echo "Yellow";
break;
case '4':
echo "Green";
break;
default:
echo "Error";
break;
}
?>

Output on the screen:
Yellow

b)

<?php
 $ch ='birds';
switch($ch)
{
case 'animal':
echo "elephant";
break;
case 'reptiles':
echo "crocodile";
break;
case 'birds':
echo "parrot";
break;
case 'mammals':
echo "cow";
break;
default:
echo "Error";
break;
}
?>

Output on the screen:
parrot


Program 2.9

Addition of two numbers using PHP function

<?php
  function addition($a, $b) {
    return $a + $b;
}
$sum = addition(4, 3);
echo "the sum of two numbers = $sum ";
?>

Output on the screen:
                                             the sum of two numbers = 7


</XMP>




</br>
<center>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>


<table style="width:40%">
  <tr>
    <th><xmp>Book</xmp></th>
                <th><xmp>Author</xmp></th>
                <th> </th>
  </tr>
  
     <tr>

              
                <td><center><xmp>PHP Cookbook </xmp></center></td>
                <td><center><xmp>David Sklar</xmp></center></td>
                <td><a href="img/pdf67.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
             
            <tr>

              
                <td><center><xmp>PHP Master</xmp></center></td>
                <td><center><xmp>Lorna Mitchell</xmp></center></td>
                <td><a href="img/pdf68.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>PHP Hypertext Preprocessor </xmp></center></td>
                <td><center><xmp>TutorialsPoint </xmp></center></td>
                <td><a href="img/pdf69.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>PHP: A Beginner's Guide</xmp></center></td>
                <td><center><xmp>Vikram Vaswani</xmp></center></td>
                <td><a href="img/pdf70.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Modern PHP</xmp></center></td>
                <td><center><xmp>Josh Lockhart</xmp></center></td>
                <td><a href="img/pdf71.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>PHP Object-Oriented Solutions</xmp></center></td>
                <td><center><xmp> David Powers</xmp></center></td>
                <td><a href="img/pdf72.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>AJAX and PHP</xmp></center></td>
                <td><center><xmp>Cristian Darie</xmp></center></td>
                <td><a href="img/pdf73.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp> PHP for the Web</xmp></center></td>
                <td><center><xmp> Larry Ullman</xmp></center></td>
                <td><a href="img/pdf74.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
              <tr>

              
                <td><center><xmp>Programming PHP</xmp></center></td>
                <td><center><xmp>Kevin Tatroe</xmp></center></td>
                <td><a href="img/pdf75.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
           
            <tr>

              
                <td><center><xmp>Pro PHP Programming</xmp></center></td>
                <td><center><xmp>Peter MacIntyre</xmp></center></td>
                <td><a href="img/pdf76.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
             
<tr>

              
                <td><center><xmp>Beginning PHP 5.3 </xmp></center></td>
                <td><center><xmp>Matt Doyle</xmp></center></td>
                <td><a href="img/pdf77.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Download</xmp></center> </a></td>
                
            </tr>
  
</table>
</center>


</br>



<p>References: </p>


<a href="img/notes1.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Notes1 (pdf)</xmp></center> </a>

<a href="img/notes1.docx" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Notes1 (word)</xmp></center> </a>


<a href="img/notes2.pdf" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Notes2 (pdf)</xmp></center> </a>


<a href="img/notes2.doc" target="_blank" style="text-decoration:none"> <font color="blue"> <center> <xmp>Notes2 (word)</xmp></center> </a>












</div>

</br>
<a href="#top"><font color="#0074B4">Back to top</font></a>

<hr>








































</BODY>
</HTML>
