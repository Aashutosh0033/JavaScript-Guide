JavaScript often abbreviated JS, is a programming language that is one of the core technologies of the World Wide Web, alongside HTML and CSS.Over 97% of websites use JavaScript on the client side for web page behavior, often incorporating third-party libraries.[13] All major web browsers have a dedicated JavaScript engine to execute the code on users' devices.

<br>

This repo contains all important concepts of JavaScript which makes it unique and versatile.<br>
*"Time, Tide and JavaScript waits for none" - [Akshay Saini](https://www.youtube.com/c/akshaymarch7)*

<br><br>

# Important Concepts

 * Functions
 * Classes and Objects 
 * Objects
 * Asychronous JS
 * ES6
 
 <br><br>

## Introduction to JavaScript

JavaScript is a **Synchronous Single Threaded language**. <br>
Everything inside JavaScript happens inside the **Execution Context**. <br>
<br>

![Screenshot (92)](https://user-images.githubusercontent.com/83531337/161437117-85c3f422-95bb-44fa-9804-cdf26b0c67f9.png)


**Phases of Execution Code**
* Memory Allocation - In this 
* Code Execution 

<br><br>


## Functions

JavaScript function is a block of code which performs a particular task. It is executed only when it is invoked (call).<br>
<br>
Syntax: <br>
```js 
function function_name(parameters){
    //code 
}
```
<br>

**Function Expressions:**

In JS Funtions can be stored in variables. <br>
For Ex. <br>
```js
let x = function(7,8) {return a+b};

console.log(x(4,5);)
```
After the function has been stores in the variable, the variable then can be used to call the function.<br>
<br>
<br>
**Types of JS function definitions :** <br>
* Simple Functions
* Function() Constructor
* Self invoking Functions
* Arrow Functions
<br>

**Simple Functions :** 

The examples above which shows the syntax for function declaration can best describe Simple Functions.<br>
<br>

**Function() Constructor :** 

Functions can also be defined with a built-in JS function constructor called Function() <br>
Syntax:<br>
```js
const myFunction = new Function("a", "b", "return a * b");
let x = myFunction(4, 3);
```
<br>

**Self Invoking Functions :** 

Function expressions can be made Self-Invoking. Function expressions will execute (started)  automaticaly, without being called.<br>
Syntax: <br>
```js
(function(){
    let x = "Hello!" //I will invoke my self
})();
```
<br>

**Arrow Functions :** 

Arrow functions allows a short syntax for writing function expressions.You don't need the function keyword, the return keyword, and the curly brackets.

```js
// ES5
var x = function(x, y) {
  return x * y;
}

// ES6
const x = (x, y) => x * y;
```

<br><br>


## Classes and Objects

JavaScript is an Object Oriented Programming Language.<br>
It has got the features of Classes and Objects.<br>
<br>
Syntax to declare a Class :<br>
```js
class Class_Name{
    constructor(){...}
}
```

For Ex. <br>
```js
class Cars{
    constructor(model,company){
    this.model = model;
    this.company = company;
    }
}
```
<br>

**Using a Class:**

```js
let myCar1 = new Cars("Forturner", "Toyota");
```
<br>

**Class Inheritance:**

Inheritance example : 
```js

class Model extends Cars{
    constructor(model,company, color){
    super(Model);
    this.color = color;
    }
}
```
<br>
A class created with class Inheritance inherits all the methods from base class.<br>
The super() method refers to the parent class.<br>
By calling the super() method in the constructor method, we call the parent's constructor method and gets access to the parent's properties and methods.<br>
<br>

<br><br>


## Objects


An object is a standalone entity, which has property and values.<br>
<br>
An example of an object : <br>
```js
const Cars = {
    model : "Fortuner",
    company : "Toyota",
    engine : 2.0,
    color : "white",
    horn : sound() 
}
```
<br>

**Accessing Values:**

Accessing Object Properties :-
```js
Cars[model];
Cars[company];
Cars[color];
```
<br>
Accessing Object Methods :-
```js
Cars.sound();
```

<br>
<br>

**Destruturing of Objects:**

```js
let {model, company, color} = Cars; 
```
<br>


**this keyword:**

this keyword refers to an object. this keyword refers to different objects depending on how it is used.<br>
<br>
Note: <br>
* In an object method, this refers to object.
* Alone, this refers to the global object.
* In a function, this refers to the global object.
* In a function, in strict mode, this is undefined.
* In an event, this refers to the element that received the event.
* Methods like call(), apply(), and bind() can refer this to any object.

<br><br>



    









