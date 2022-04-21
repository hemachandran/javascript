# Js Functions
- A function in JavaScript is similar to a procedure, a set of statements that performs a task
- Reuse code: Define the code once, and use it many times.

### Defining functions
- A function definition (also called a **function declaration**, or **function statement**) consists of the **`function`** keyword, followed by:
  - The name of the function
  - A list of parameters to the function, enclosed in parentheses `()` and separated by commas `,`
  - The JavaScript statements that define the function, enclosed in curly brackets, {...}

```javascript
function square(number) {
  return number * number;
}

/* Syntax
function - reversed keyword in js
square - name of the function
(number) - parameter
return - reversed keyword in js & something will be returned
*/

```
### Calling the function
- By using the function name and pass the parameter within enclosed parentheses

```javascript
square(5); //25
square(3); //9
```
### Function scope
- Variables defined inside a function cannot be accessed from anywhere outside the function, because the variable is defined only in the scope of the function

```javascript
// The following variables are defined in the global scope
var num1 = 20,
    num2 = 3,
    name = 'Peter';

// This function is defined in the global scope
function multiply() {
  return num1 * num2;
}

multiply(); // Returns 60

// A nested function example
function getScore() {
  var num1 = 2,
      num2 = 3;

  function add() {
    return name + ' scored ' + (num1 + num2);
  }

  return add();
}

getScore(); // Returns "Peter scored 5"
```

### Recursion
- A function can refer to and call itself. There are three ways for a function to refer to itself:

```javascript
function countDown(fromNumber) {
    console.log(fromNumber);
    countDown(fromNumber-1);
}

countDown(3);

Uncaught RangeError: Maximum call stack size exceeded.
```

### Function Invocation
- The code inside the function will execute when "something" invokes (calls) the function:
  - When an event occurs (when a user clicks a button)
  - When it is invoked (called) from JavaScript code
  - Automatically (self invoked)

<h3 align="left"><a href="04-Arrays">Prev: Arrays</a></h3>
<h3 align="right"><a href="06-Objects">Next: Objects</a></h3>
