This repo contains all important concepts of JavaScript which makes it unique and versatile.<br>
*"Time, Tide and JavaScript waits for none" - Akshay Saini*
<br><br><br>

# Important Concents

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

**Simple Functions :** The examples above which shows the syntax for function declaration can best describe Simple Functions.<br>
<br>

**Function() Constructor :** Functions can also be defined with a built-in JS function constructor called Function() <br>
Syntax:<br>
```js
const myFunction = new Function("a", "b", "return a * b");
let x = myFunction(4, 3);
```
<br>

**Self Invoking Functions :** Function expressions can be made Self-Invoking. Function expressions will execute (started)  automaticaly, without being called.<br>
Syntax: <br>
```js
(function(){
    let x = "Hello!" //I will invoke my self
})();
```
<br>

**Arrow Functions :** Arrow functions allows a short syntax for writing function expressions.You don't need the function keyword, the return keyword, and the curly brackets.

```js
// ES5
var x = function(x, y) {
  return x * y;
}

// ES6
const x = (x, y) => x * y;
```








