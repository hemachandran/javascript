# Callback function
- A callback function is a function passed into another function as an argument, which is then invoked.

**Example:**

```js
function greeting(name) {
  alert('Hello ' + name);
}

function processUserInput(callback) {
  var name = prompt('Please enter your name.');
  callback(name);
}

processUserInput(greeting); //passing greeting function as a arugument
```

Callback are synchronous, as it is executed immediately.

# Closures
- It provides access to an outer function's scope from an inner function
- In JavaScript, closures are created every time a function is created

```javascript
function printName() {
  var courseName = 'JavaScript 2015'; // local variable created by printName
  function displayName() { // displayName() is the inner function, a closure
    console.log(courseName); // use variable declared in the parent function
  }
  displayName();
}
printName();
```

### References
- Js Closures - [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)
