## What You Need To Know About JavaScript
###### Collection of key points and notes on this book

#### Some common uses of JavaScript

- If you need to create a contact form where some fields are required, you can
rely on JavaScript to alert the user if he has missed some of these fields and
to validate or sanitize their contents. You don't have to rely on alert windows
anymore as the Document Object Model (DOM) can be accessed through
JavaScript to manipulate its look, content, and attributes.

- You can populate search boxes with common terms as you type into them;
this is a feature known as autocomplete.

- Displaying or hiding information on demand and animating elements on a
page is a walk in the park using JavaScript.

- Using JavaScript, you can pass requests to a backend server and handle
responses without reloading the page.

#### Variables, mathematical operations and string concatenation

A variable can be declared and given a value in two separate steps, which are
displayed as follows:

```
var myTeam;
myTeam = 'Chicago Bulls';
```

They can also be given a value in a single step, as follows:

```
var myTeam = 'Chicago Bulls';
```

> JavaScript allows us to declare variables without the var keyword (the variable will
be global). Anyway, this practice is not recommended, and most developers will
advise against it and think that it should be deprecated.

> When building a string variable as the result of the concatenation of two or more
values, it is recommended that you be consistent with the use of single or double
quotes. Many JavaScript developers prefer to use double quotes to enclose string
values as this allows you to use single quotes within the variable without the need
to escape them.

> While others prefer to use single quotes, the principle that should be followed is this:
if you need to use one form of quote in the string, you might want to use the other
one as the literal.

#### Arrays and objects

You can easily create an object variable with properties.
Using this approach, you can think of an object as a thing. For example, let's create an
object variable named dog with three properties: color , age , and breed , as follows:

```
var dog= {color: 'Brown', age: 4, breed: 'Boxer'};
```

You can then query the object variable as a whole or each property using the dot
notation (the object name followed by a dot and the property name):

```
dog;
dog.color;
dog.age;
dog.breed;
```

> Properties cannot only be fixed values, but they can also be methods that represent
an action that is associated with the object. Using the dog object, let's redefine it and
add a method property called bark :

```
var dog= {
color: 'Brown',
age: 4,
breed: 'Boxer',
bark: function(){
console.log('Guau guau')
}
};
```

A method property can be invoked like a regular property as explained previously,
and then followed by a set of parentheses that denote an action:

```
dog.bark();
```

#### Functions

You can think of a JavaScript function as a procedure that performs a task, manipulates
variables, and calculates a result.


#### Libraries

> In order to provide more complex functionality with little extra effort, you can
combine JavaScript statements and functions into a single file that is invoked in
a web page. These files use the .js (for JavaScript) extension, and they are called
libraries.

Save the following code into a file named test.js :

```
/* Function declaration
====================

The SayHi project requires 3 parameters: your name , age , and profession
(in that order).
In the function definition, these three parameters are named a , b , and c .
The function returns a greeting using these values:
*/

function SayHi(a,b,c){
var person = {name: a, age: b, profession: c};
return 'My name is ' + person.name + ' and am ' + person.age + '
years old. I am a ' + person.profession + '.';
}

/* Object definition
=================

The introducingMyself object is an object variable that gets the first h3 element
in the document. This element has a property called textContent where we will
display the result of calling SayHi with the following indicated parameters:
*/

var introducingMyself = document.querySelector('h3');
introducingMyself.textContent = SayHi('Gabriel', 33,
'programmer');
```

We will then create a file named index.html in the same directory where you saved
test.js . Note that, in order to reference the external file test.js , you need to place
the reference inside <script> tags as indicated in the following:

```
<!DOCTYPE html>
<html lang = "en-US">
<head>
<meta charset = "UTF-8">
<title>Chapter 1</title>
</head>
<body>
<h1>First example</h1>
<h3></h3>
<script src="test.js"></script>
</body>
</html>
```















