# Strings in JavaScript
It contains single character (or) a whole word which enclosed in single quotes (' ') | double quotes (" ")

#### Valid :heavy_check_mark:
```javascript
const country = "India";
const food = 'Rice';
```
#### Invalid :x:
```javascript
const badString1 = This is a test;
const badString2 = 'This is a test;
const badString3 = This is a test';
const badQuotes4 = 'What on earth?";
```
#### Concatenating
- To join together strings in JavaScript
```javascript
const name = 'Chris';
const greeting = `Hello, ${name}`;
console.log(greeting); // "Hello, Chris"
```
- You can also concatenate strings using the `+` operator
```javascript
const greeting = "Hello";
const name = "Chris";
console.log(greeting + ", " + name); // "Hello, Chris"
```
#### Template Literal
- A template literal looks just like a normal string, but instead of using single or double quote marks (`'` or `"`), you use backtick characters (`` ` ``)

## Few Strings Methods
```javascript
const greeting = "Hello";
```
| Methods | Usage| Results |
| --- | :--- | --- |
| `length` | greeting.length| 4 |
| `toLowerCase()` | greeting.toLowerCase() | hello |
| `toUpperCase()` | greeting.toUpperCase() | HELLO |
| `replace()` | greeting.replace('Hello','Hello World') | Hello World|

### References
JavaScript String Methods [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)
