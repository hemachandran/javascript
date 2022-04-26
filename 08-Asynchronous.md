# Introducing Asynchronous JavaScript
- Before we get to know about Asynchronous concept, we need to see **Synchronous programming**

**Example**

```javascript
function makeGreeting(name) {
  return `Hello, my name is ${name}!`;
}

const name = 'Mike';
const greeting = makeGreeting(name);
console.log(greeting);
// "Hello, my name is Mike!"

```

- `makeGreeting()` is a **synchronous function**, because the caller has to wait for the function to finish its work before the function returns.

- What if the synchronous function takes a long time?
  - Ex.: Gnerates a number of large prime numbers
