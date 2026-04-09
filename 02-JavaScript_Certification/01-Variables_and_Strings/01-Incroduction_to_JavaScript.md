## What Is JavaScript, and How Does It Work with HTML and CSS?
 JavaScript is a programming language that brings interactivity and dynamic behavior to websites.
 While HTML and CSS are markup languages used to scructure content and style elements on a page, JavaScript goes beyong those by enabling more complex functionality, such as hanlding user input, animating elements, and even buildng full web applications.

### Example
```HTML
<!DOCTYPE html>
<html>
    <head>
        <style>
            h1 {
                color: green;
            }
        </style>
    </head>
<body>
    <h1>Hello, World!</h1>
    <!--inside button is JavScript code-->
    <button onclick="alert('Buttom clicked!')">Click me</button>
</body>
</html>
```
## What Is a Data Type, and What Are the Different Data Types in JavaScript?

 In JavaScript, a data type is the kind of value you store like a number or piece of text.

### Example
```JavaScript
// Examples of integers
console.log(3);
console.log(5);
console.log(-67);
// Examples of floating point numbers
conosle.log(3.14);
conosle.log(7.2);
console.log(-14.5);
// String
console.log("I love to code!");
```
 A `boolean` reoresents one of twu values: `true` or `false`.  
 A `undefined` means a variable has been declared but hasn't been given a value yet.  
 A `null` means the variable has been intentionally set to "nothing" and not hold any value.  

## What Are Variables, and What Are Guidelines for Naming JavaScript Variables?

 In JavaScript, variables act as containers for storing data that you cand access and modify throughout your program.  
 One way to declare a variable in JavaScript is to use the `let` keyword.  
 Example:
```JavaScript
let age;
console.log(age); // undefined
let age = 25;
console.log(age); // 25
age = 30;
console.log(age); // 30
```

 Variable names should describe what the data represents.  
 Example:
 ```JavaScript
 // Bad variable names
let x = 10;
let y = "John";

// Good variable names
let age = 10;

// Valid variable names
let age;
let _score;
let $total;

// Invalid variable names
let 1stPlace; // starts with a number
```
 Variable names are case-sensitive: `age` and `Age` are differents.  

## How Do let and const Work Differently When It Comes to Variable Declaration, Assignment, and Reassignment?

 The `let` keyword allows you to declare variables that can be updated or reassigned later. You can change that value as needed throughout your program.  
 The `const` is used to declare variables that are constant. Cannot be reassigned.  
Example:
```JavaScript
let score = 10;
console.log(score); // 10
score = 20;
console.log(score); // 20  

const maxScore = 100;
console.log(maxScore); // 100
```
## What Is a String in JavaScript, and What Is String Immutability?

 String are one of the primitive data types in the language.  
 To create a string in JavaScript, you can use single quotes ('), or double quotes (").  
 Example:
```JavaScript
let singleQuotes = 'This is a string';
console.log(singleQuotes);
let doubleQuotes = "This is also a string";
console.log(doubleQuotes);
```
 
# What Is String Concatenation, and How Can You Concatenate Strings with Variables?

Concatenate - meaning the acting of linking

Example `+` operator:  
```JavaScript
let firstName = "John";
let lastName = "Doe";

let fullName = firstName + " " + lastName; 
console.log(fullName); // John Doe

let fullName = firstName + lastName; 
console.log(fullName); // "JohnDoe"
```
 
Example `+=` operator:
```JavaScript
let greeting = 'Hello';
greeting += ', John';

console.log(greeting); // "Hello, John!"
```
 It is important to remember that strings are immutable which means once a string is created you can not alter it.  
 Another way: `concat()` method.
 
*Important part:*

- A **function** is a reusable block of code that performs a specific task and can be called with varios inputs.  
- A **method** is a type of function that is associated with an object, meaning it operates on the data contained within that object.

Example:
```JavaScript
let str1 = 'Hello';
let str2 = 'World';

let result = str1.concat(' ', str2); 
console.log(result); // Hello World
```
 To conclude:
 - Operator `+` for simple concatenation, especially to combine a few strings or variables.  
 - Operator `+=` for building up a string step by step or appedning new content to an exisitin string variable.
 - Method `concat()' for combining multiple strings together.

 # What Is console.log Used For, and How Does It Work?

 Method `console.log()` to display message to the browser's console.  
 For debuging or inspecting code.  
 Example:
 ```JavaScript
 console.log("Hello, world!");
 ```
 




