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
