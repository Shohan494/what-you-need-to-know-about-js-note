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

























