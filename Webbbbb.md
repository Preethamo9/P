Program 1.	Develop the HTML page named as “Myfirstwebpage.html”. Add the following tags with relevant content.
Set the title of the page as “My First Web Page”. Within the body use the following tags:
Moving text = “Basic HTML Tags”
Different heading tags (h1 to h6)
Paragraph
Horizontal line
Line Break
Block Quote
Pre tag
Different Logical Style (, , etc..)


<!DOCTYPE html>
<head>
<title>Anu’s First Web Page</title>
</head>
<body>
<!-- Moving text -->
<marquee><center>Welcome to Web Technology Lab</center></marquee>
<marquee><center>Basic HTML Tags</center></marquee>
<!-- Different heading tags -->
<h1>This is an H1 heading</h1>
<h2>This is an H2 heading</h2>
<h3>This is an H3 heading</h3>
<h4>This is an H4 heading</h4>
<h5>This is an H5 heading</h5>
<h6>This is an H6 heading</h6>

<!-- Paragraph -->
<p>This is a paragraph demonstrating the use of the paragraph tag in HTML.</p>
<!-- Horizontal line -->
<hr>
<!-- Line break -->
<p>This is a line of text before the break.<br>This is a line of text after the break.</p>
<!-- Block Quote -->
<blockquote>
This is a blockquote. It is used to display a quotation or excerpt from another source.
</blockquote>
<!-- Pre tag -->
<pre>
This is preformatted text.
It preserves spaces and line breaks.
</pre>

<!-- Different Logical Style tags -->
<p>This is <b>bold</b> text.</p>
<p>This is <i>italicized</i> text.</p>
<p>This is <u>underlined</u> text.</p>
<p>This is <sup>superscript</sup> text.</p>
<p>This is <sub>subscript</sub> text.</p>
<p>This is <em>emphasized</em> text.</p>
<p>This is <strong>strong</strong> text.</p>
<p>This is <mark>highlighted</mark> text.</p>
<p>This is <small>small</small> text.</p>
<p>This is <del>deleted</del> text.</p>
<p>This is <ins>inserted</ins> text.</p>
<p>This is <code>inline code</code> text.</p>
</body>
</html>

Output:

Program 2. Develop the HTML page named as “Table.html” to display your class time table.
Provide the title as Time Table with table header and table footer, row-span and col- span etc.
Provide various colour options to the cells (Highlight the lab hours and elective hours with different colors.)c) Provide colour options for rows.


<!DOCTYPE html>
<head>

<title>Time Table</title>

<style>
body {
font-family: 'Times New Roman';
}
table {
width: 80%; margin: 20px auto;
border-collapse: collapse;
}
th,
td {
border: 1px solid #ddd; padding: 8px;
text-align: center;
}

th {
background-color: #f4f4f4; color: #d63384;
}

tr:nth-child(even) { background-color: #f9f9f9;
}

tr:nth-child(odd) { background-color: #e6f7ff;
}

.lab-hour {

background-color: #ffcccc;
}
.elective-hour {
background-color: #ccffcc;
}
.highlight {
font-weight: bold; color: #d63384;
}
tfoot {
background-color: #e0e0e0; font-weight: bold;
}


</style>
</head>
<body>

<h1 style="text-align: center;">Time Table</h1>

<table>
<thead>
<tr>
<th>Day/Time</th>
<th>9:00 - 10:00</th>
<th>10:00 - 11:00</th>
<th>11:20 - 12:20</th>
<th>12:20 - 1:15</th>
<th>Lunch Break</th>
<th>2:10 - 3:00</th>
<th>3:00 - 3:45</th>
<th>3:45 - 4:35</th>
</tr>
</thead>
<tbody>
<tr>
<td>Monday</td>
Type in the Code for your class Time Table here
</tr>
<tr>
<td>Tuesday</td>
Type in the Code for your class Time Table here
</tr>
<tr>
<td>Wednesday</td>

Type in the Code for your class Time Table here
</tr>
<tr>
<td>Thursday</td>
Type in the Code for your class Time Table here
</tr>
<tr>
<td>Friday</td>
Type in the Code for your class Time Table here
</tr>
<tr>
<td>Saturday</td>
Type in the Code for your class Time Table here
</tr>
</tbody>
<tfoot>
<tr>
<td colspan="9">End of Timetable</td>
</tr>
</tfoot>
</table>

</body>

</html>

Output:

Program 3 Develop an external style sheet named as “style.css” and provide different styles for h2, h3, hr, p, div, span, time, img & a tags. Apply different CSS selectors for tags and demonstrate the significance of each.
Note: make two files style.css and index.html

index.html
<html>

<head>
<title>Styled HTML Page </title>
<link rel="stylesheet" href="style.css">
</head>

<body>

<h2>Main Heading</h2>
<h3>Subheading</h3>	mmm
<hr>
<p>This is a paragraph demonstrating the basic text styling applied by CSS.</p>

<div>
This is a styled <strong>div</strong> element with padding and a light border. Inside the div, we can also use
<span>span elements</span> that have their own styles, like this bold and orange text.
</div>

<p>Current time: <time>10:30 AM</time></p>

<img src="Canara.jpg" alt="CEC logo">

<p>Visit <a href="https://www.w3schools.com/">w3schools</a> to learn about web programming.</p>

<p class="highlight">This paragraph is highlighted with a yellow background.</p>
<p class="center">This text is centered using a class selector.</p>

<p id="special-paragraph">This is a special paragraph with unique styles applied through an ID selector.</p>

</body>
</html> style.css
* {
margin: 0;

padding: 0;
box-sizing: border-box;
}

h2 {
color:red; font-size: 30;
margin-bottom: 10px;
}

h3 {
color: orange; font-size: 15;
margin-bottom: 8px;
}

hr {
border: 0; height: 2px;
background-color: blue; margin: 20px 0;
}

p {
font-family: 'Arial', sans-serif; line-height: 1.6;
margin: 10px 0;
}

div {
padding: 15px;
border: 1px solid black; background-color:blanchedalmond
}

span {
color: brown; font-weight: bold;
}

time::before { content: ''; color:greenyellow;
}
img {

margin-left: 15px; height: 100px; width: 100px; border-radius: 8px;
box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
max-width: 100%;
}

a {
text-decoration: none; color: purple;
}

a:hover { color: blue;
text-decoration: underline;
}

.highlight {
background-color: yellow; padding: 3px;
}

.center {
text-align: center;
}

#special-paragraph { font-size: 25; color: plum;
background-color:ghostwhite; padding: 10px;
border-left: 5px solid plum;
}

h2,
h3,
p {
margin-left: 20px;
}

Output:

Main Heading

1lisisa par")ra;tl-aingIlle basi:texsttytr,gappledbyCSS

Thisisastyleddn- lm:tmi:withpaddmgmidahghtborda_lnsldt di•;,wecanalsowsp.utlnantsdwbai"tdm011.uSl}ies.lihdnsboldmiorangeu:n

Cooentline: 10:30AM

.CAi ARA
Visitw3schoos tooamabootwebprogran,mg.


Thsparo,raph • h IJ>;ihtedwrtnayo11owbackgroooo
I


1listextiscenle!edusilgaclasssetoctor.

Program 4. Develop HTML page named as “registration.html” having variety of HTML input elements with background colors, table for alignment & provide font colors & size using CSS styles.
registration.html
<!DOCTYPE html>
<head>
<title>Registration Form</title>
<style>
body {
font-family: Arial, sans-serif; background-color: #f0f4f8; margin: 0;
padding: 20px; display: flex;
justify-content: center; align-items: center; min-height: 100vh;
}
.container { width: 100%;
max-width: 600px; background-color: #fff; padding: 20px;
border-radius: 8px;
box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); display: flex;
flex-direction: column; gap: 20px;
}
h2 {
text-align: center; color: #333;
margin: 0;
}
.form-group { display: flex;
flex-direction: column; gap: 5px;
margin-bottom: 10px;
}
label {
font-size: 14px; color: #555;
}
input[type="text"], input[type="email"],

input[type="password"], input[type="date"], select,
textarea { padding: 10px;
border: 1px solid #ccc; border-radius: 4px; font-size: 14px;
}
.gender-options { display: flex; gap: 10px;
align-items: center;
}
input[type="submit"], input[type="reset"] {
padding: 10px 20px; border: none; border-radius: 4px; cursor: pointer;
font-size: 16px; flex: 1;
}
.button-group { display: flex; gap: 10px;
justify-content: center;
}
input[type="submit"] { background-color: #4CAF50; color: white;
}
input[type="reset"] { background-color: #f44336; color: white;
}
.form-group textarea { margin-bottom: 10px;
}
</style>
</head>
<body>
<div class="container">
<h2>Registration Form</h2>
<form action="#" method="post">
<div class="form-group">

<label for="firstName">First Name:</label>
<input type="text" id="firstName" name="firstName" required>
</div>
<div class="form-group">
<label for="lastName">Last Name:</label>
<input type="text" id="lastName" name="lastName" required>
</div>
<div class="form-group">
<label for="email">Email:</label>
<input type="email" id="email" name="email" required>
</div>
<div class="form-group">
<label for="password">Password:</label>
<input type="password" id="password" name="password" required>
</div>
<div class="form-group">
<label for="dob">Date of Birth:</label>
<input type="date" id="dob" name="dob">
</div>
<div class="form-group">
<label>Gender:</label>
<div class="gender-options">
<input type="radio" id="male" name="gender" value="male">
<label for="male">Male</label>
<input type="radio" id="female" name="gender" value="female">
<label for="female">Female</label>
</div>
</div>
<div class="form-group">
<label for="country">Country:</label>
<select id="country" name="country">
<option value="usa">USA</option>
<option value="canada">Canada</option>
<option value="uk">UK</option>
<option value="india">India</option>
</select>
</div>
<div class="form-group">
<label for="bio">Bio:</label>
<textarea id="bio" name="bio" rows="4"></textarea>
</div>
<div class="button-group">
<input type="submit" value="Register">
<input type="reset" value="Reset">
</div>
</form>

</div>
</body>
</html> Output:

Program 5. Develop HTML page named as “newpaper.html” having variety of HTML semantic elements with background colors, text-colors & size for figure, table, aside, section, article, header, footer… etc.
<!DOCTYPE html>
<head>
<title>Newspaper Page</title>
<style>
* {
margin: 0;
padding: 0;
box-sizing: content-box;
}

body {
padding: 20px;
font-family: 'Arial', sans-serif; color:black;
display: block;
flex-direction: row; min-height: 100vh;
}

header {
margin-bottom: 30px; border-radius: 10px; align-items: center; background-color:blue; color:whitesmoke; padding: 20px; display: flex;
justify-content:space-between; text-align: center;
}

header a {
font-size: 25px; font-weight: bold; color: white;
text-decoration: none;
}
nav {
display:flex; gap: 50px;
}
nav a {

font-size: 18px; color:black;
text-decoration: none; font-weight: bold;
}
nav a:hover {
text-decoration: underline;
}
.content {
display: flex;
justify-content: space-between; margin: auto;
padding: 20px 0; gap: 20px; position: relative;
}
.main-content { cursor: pointer; display:grid;
grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); gap: 20px;
background-color:white; border-radius: 12px; padding: 25px;
}
aside {
border: 1px solid brown;
padding: 25px;	width: 350px; border-radius: 8px;
position: sticky ; top: 20px; color:red;
right: 0;
margin-left: 10 px;	}
.related-news h3 { text-align: center; border-radius: 7px; padding: 8px; background:black; color: white;
margin-bottom: 15px;
}
.related-news ul { list-style: inside; padding: 7px; margin: 0;

}
.related-news li { margin-bottom: 12px;
}
.related-news a {
text-decoration: none; color: blueviolet;
font-weight: bold;
}
.related-news a:hover {
text-decoration: underline;
}
footer {
border-radius: 10px; background-color: brown; color: white;
padding: 20px; font-weight: 500; text-align: center; margin-top: auto; font-size: 18px;
}
article {
background-color: white; padding: 15px;
border-radius: 7px; color: black;
}
figure {
background-color: whitesmoke; padding: 10px;
border: 1px solid gray; border-radius: 8px; text-align: center; margin: 0;
}
figcaption {
font-size: 1.4em; color: palevioletred;
}
img {
max-width: 100%; height: auto; border-radius: 8px;
}
section {

padding: 20px; width: 100%;
background-color:white; border-radius: 8px;
}
section h2 { color:white;
background:burlywood; font-size: 24px;
border-radius: 10px; text-align: center; padding: 10px; margin-bottom: 30px;
}
table {
width: 100%;
border-collapse: separate;
}
caption {
font-size: 18px; margin-bottom: 10px; color: royalblue;
}
thead {
background-color: orangered; color: white;
}
th,
td {
padding: 12px; text-align: left;
}
th {
font-weight: bold;
}
tbody tr:nth-child(odd) { background-color: violet;
}

tbody tr:nth-child(even) { background-color:violet;
}

tbody tr:hover {
background-color: whitesmoke;
}

@media (max-width: 600px) { th,
td {
padding: 8px; font-size: 14px;
}
}

caption {
background-color: grey; padding: 10px;
font-weight: bold;
border-bottom: 2px solid powderblue; border-radius: 8px 8px 0 0;
font-size: 1.1em; color: black;
}
article h2 {
color: blueviolet; font-size: 1.3em;
margin-bottom: 12px;
}

</style>
</head>

<body>
<header>

<a href="#">Newspaper</a>

<nav>
<a href="#">Home</a>
<a href="#">About</a>
<a href="#">Contact</a>
<a href="#">Services</a>
<a href="#">Marketing</a>
<a href="#">Updates</a>
</nav>

</header>

<div class="content">
<main class="main-content">
<article>

<h2>Article Title 1</h2>
<figure>
<img src="https://diplo-media.s3.eu-central-1.amazonaws.com/2024/05/google- mobile-application-smart-phone-screen-1024x683.jpg" alt="Technology">
<figcaption>Google introduces compliance tool for apps and AI</figcaption>
</figure>
<p>First article</p>
</article>

<article>
<h2>Article Title 2</h2>
<figure>
<img src="https://iottechnews.com/wp-content/uploads/2024/10/samsung-knox- matrix-iot-security-smart-home-appliances-internet-of-things.jpeg" alt="Technology">
<figcaption> Knox expands to bolster IoT security</figcaption>
</figure>
<p>Second article</p>
</article>

<article>
<h2>Article Title 3</h2>
<figure>
<img src="https://www.financialexpress.com/wp- content/uploads/2024/10/rtatanchand.reuters.jpg?w=1024" alt="Business">
<figcaption>Chandrasekaran pays tribute to Ratan Tata</figcaption>
</figure>
<p>Third article</p>
</article>

</main>
<aside class="related-news">
<h3>Related News</h3>
<ul>
<li><a href="#">Related News 1</a></li>
<li><a href="#">Related News 2</a></li>
<li><a href="#">Related News 3</a></li>
</ul>
</aside>

</div>

<section>
<h2>Recent Posts</h2>
<div>
<table>
<caption>List of Posts</caption>

<thead>
<tr>
<th>Post Title</th>
<th>Date</th>
<th>Author</th>
</tr>
</thead>
<tbody>
<tr>
<td>Post 1</td>
<td>2024-08-30</td>
<td>Author 1</td>
</tr>
<tr>
<td>Post 2</td>
<td>2024-08-29</td>
<td>Author 2</td>
</tr>
</tbody>
</table>
</div>
</section>

<footer>
<p>© 2024 Newspaper. All rights reserved.</p>
</footer>
</body>

</html>

Output:


Newspaper	H<fflc At>c,o,tl Conu« S,:,,vi.;c-:; M1r1..11n11 IJl:d =





Att1cle Tflle 1	Ametent1e2	An1cle TIiie3





l!» ('(<'fl("'Ml !Wa-«
U• lfCl.fld) .,.1:1
.	ta'. (lo)
.-. '-"-"J°·"•'""tr'".."'	"""'

Attltlll Tfllll 4
f'M• Wltfli/'t
Mll:le- l-l"'-""' ­
_	_.,,,J.-h)Ol $H60
--f,lll'n(lolt...-111-
#1_,r.	,H:;,"'


Arllc.k TitlllS
ft-.ll"-00,,ICnl<lll!th-,.:.":k
.-.F,_.t.'.l_t,,.,.)..,.,j,(.,l,,o,u).,..
.,_,,_	,






		




n»i. «lffllH.Ol"'twlf
- .-:;:"""'
----oln!••---·
fl'l1i,1•, •-C111t
...'--"'"-'"'CIOICI_<..
.•.•-•.•...,:.u..,	,;e1u,1>i.::,.
,,..., //C/flefll/f l)l,m
ll«atU•- -t'III­
-.W  tc.-•.:Sltl_.\1..1._




Program 6:
Apply HTML, CSS and JavaScript to design a simple calculator to perform the following operations: sum, product, difference, remainder, quotient, power, square-root and square.
<html> <head>
<title>Simple Calculator</title>
<style>
body {
font-family: 'Times New Roman'; display: flex;
justify-content: center; align-items: center; height: 100vh; margin: 0;
}
.calculator { background: white; padding: 20px; border-radius: 12px; width: 320px;
text-align: center; h1 {
border-radius: 8px; background: black; font-size: 24px; padding: 10px; color: white;
margin-bottom: 30px;
}
input, select, button {
width: 100%;
margin: 10px 0; padding: 12px;
border: 1px solid green; border-radius: 8px;
font-size: 16px;
box-sizing: border-box;
}
input:focus, select:focus, button:focus {
outline: none; border-color:black;
}

button {
background-color: green; color: white;
border: none; cursor: pointer; font-size: 18px;
}
#result.error { background: orange; border-color: red;
}
#result.success { font-size: 17px; font-weight: bold; color: black;
background: lightpink; border-color: darkcyan; border-radius: 20px; border:1px solid black; padding:15px;
}
</style> </head>
<body>
<div class="calculator">
<h1>Simple Calculator</h1>
<form id="calculator-form">
<input type="number" id="num1" placeholder="Enter first number" required>
<input type="number" id="num2" placeholder="Enter second number" required>
<select id="operation" required>
<option value="">Select Operation</option>
<option value="sum">Sum</option>
<option value="product">Product</option>
<option value="difference">Difference</option>
<option value="remainder">Remainder</option>
<option value="quotient">Quotient</option>
<option value="power">Power</option>
<option value="sqrt">Square Root</option>
<option value="square">Square</option>
</select>
<button type="button" onclick="calculate()">Calculate</button>
</form>
<div id="result"></div>
</div>
<script>
function calculate() {
const num1 = parseFloat(document.getElementById('num1').value);

const num2 = parseFloat(document.getElementById('num2').value); const operation = document.getElementById('operation').value;
let result = '';
let resultClass = 'success';

if (isNaN(num1) || isNaN(num2)) { result = 'Please enter valid numbers.'; resultClass = 'error';
} else {
switch (operation) { case 'sum':
result = `Sum: ${num1 + num2}`; break;
case 'product':
result = `Product: ${num1 * num2}`; break;
case 'difference':
result = `Difference: ${num1 - num2}`; break;
case 'remainder':
result = `Remainder: ${num1 % num2}`; break;
case 'quotient':
if (num2 == 0) {
result = 'Cannot divide by zero'; resultClass = 'error';
} else {
result = `Quotient: ${num1 / num2}`;
}
break; case 'power':
result = `Power: ${Math.pow(num1, num2)}`; break;
case 'sqrt':
if (num1 < 0 || num2 < 0) {
result = 'Square root is not defined for negative numbers'; resultClass = 'error';
} else {
result = `Square Root of ${num1}: ${Math.sqrt(num1)} <br> Square Root of ${num2}: ${Math.sqrt(num2)}`;
}
break;
case 'square':
result = `Square of ${num1}: ${Math.pow(num1, 2)} <br> Square of ${num2}: ${Math.pow(num2, 2)}`;
break;

default:
result = 'Please select an operation.'; resultClass = 'error';
}
}

const resultDiv = document.getElementById('result'); resultDiv.innerHTML = result; resultDiv.classList.remove('show', 'error', 'success'); resultDiv.classList.add(resultClass, 'show');
}
</script>
</body>
</html>



Output:











Program 7: Develop JavaScript program (with HTML/CSS) for:
Converting JSON text to JavaScript Object
Convert JSON results into a date
Converting From JSON To CSV and CSV to JSON
Create hash from string using crypto.createHash() method
<html> <head>
<script src="https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto- js.min.js">
</script> <title>Simple Converter</title>
<style>
* { padding: 0;
margin: 0;
box-sizing: border-box;
}
body {
font-family: Arial, sans-serif; color: black;
}
.container {
width: 60%;
margin: 0 auto; padding: 20px;
}
.head-title h1 { font-size: 28px; width:100%;
background: pink; padding: 10px; color:black;
margin-bottom: 50px; border-radius: 10px; text-align: center;
}
.section {
margin-bottom: 40px;

padding: 20px; border-radius: 8px;
background: whitesmoke; color:black;
font-size: 20px;
}
textarea {
font-size: 30px; width: 100%; height: 120px;
margin-bottom: 15px; padding: 12px; border-radius: 8px;
border: 1px solid grey; box-sizing: border-box;
}
input[type="text"] { width:100%; padding: 12px; border-radius: 8px;
border: 1px solid blueviolet; box-sizing: border-box;
}
button {
display: inline-block; padding: 15px 15px; margin: 10px 0;
font-weight: bold; border: none; border-radius: 7px;
background-color:blue; color: white;
cursor: pointer; font-size: 16px;
}
.error {
margin-top: 10px; font-size: 14px; color: black; background: plum; border-color: red; padding: 10px;
}
.success {
margin-top: 10px; font-size: 14px;

color:black;
background: powderblue; border-color: brown; padding: 10px;
}
</style> </head> <body>
<div class="container">
<div class="head-title">
<h1>Simple Converter</h1>
</div>
<div class="section">
<h2>1. Convert JSON Text to JavaScript Object</h2>
<textarea id="jsonInput" placeholder="Enter JSON here..."></textarea>
<button oncli
