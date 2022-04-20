# Js Functions
- A function in JavaScript is similar to a procedu, a set of statements that performs a task

### Defining functions
- A function definition (also called a **function declaration**, or **function statement**) consists of the **`function`** keyword, followed by:
  - The name of the function
  - A list of parameters to the function, enclosed in parentheses `()` and separated by commas `,`
  - The JavaScript statements that define the function, enclosed in curly brackets, {...}
```javascript
function square(number) {
  return number * number;
}
```
### Calling the function
- By using the function name and pass the parameter within enclosed parentheses

```javascript
square(5); //25
square(3); //9
```


Function scope
Variables defined inside a function cannot be accessed from anywhere outside the function, because the variable is defined only in the scope of the function
