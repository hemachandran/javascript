# Strings in JavaScript
It contains single character (or) a whole word which enclosed in single quotes (' ') | double quotes (" ")

#### Valid &check;
```javascript
const country = "India";
const food = 'Rice';
```
#### Invalid &Cross;
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
<table>
  <tbody>
    <tr>
      <td><strong>Methods</strong></td>
      <td><strong>Usage</strong></td>
      <td><strong>Results</strong></td>
    </tr>
    <tr>
      <td><code>length</code></td>
      <td>greeting.length</td>
      <td>4</td>
    </tr>
    <tr>
      <td><code>toLowerCase()</code></td>
      <td>greeting.toLowerCase()</td>
      <td>hello</td>
    </tr>
    <tr>
      <td><code>toUpperCase()</code></td>
      <td>greeting.toUpperCase()</td>
      <td>HELLO</td>
    </tr>
    <tr>
      <td><code>replace()</code></td>
      <td>greeting.replace('Hello','Hello World')</td>
      <td>Hello World</td>
    </tr>
   </tbody>
  </table>
    
### Js String References
JavaScript String Methods [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)
