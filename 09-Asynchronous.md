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

# Asynchronous 
- A `Promise` is an object representing the eventual completion or failure of an asynchronous operation

**Example of Callback**
```javascript
function successCallback(result) {
  console.log("Audio file ready at URL: " + result);
}

function failureCallback(error) {
  console.error("Error generating audio file: " + error);
}

createAudioFileAsync(audioSettings, successCallback, failureCallback);
```

### Promises
```javascript
createAudioFileAsync(audioSettings).then(successCallback, failureCallback);
```
- `.then()` a method returns a Promise. It takes up to two arguments: callback functions for the **success** and **failure** cases of the Promise.

**Example**
```javascript
//Method - 1
doSomething()
.then(result => doSomethingElse(result))
.then(newResult => doThirdThing(newResult))
.then(finalResult => console.log(`Got the final result: ${finalResult}`))
.catch(failureCallback);

//Method - 2 (try, catch)
try {
  const result = syncDoSomething();
  const newResult = syncDoSomethingElse(result);
  const finalResult = syncDoThirdThing(newResult);
  console.log(`Got the final result: ${finalResult}`);
} catch(error) {
  failureCallback(error);
}

```

![promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/promises.png)

## Async / Await
- An async function is a function declared with the async keyword, and the await keyword is permitted within it. The async and await keywords enable asynchronous, promise-based behavior to be written in a cleaner style

```javascript
async function foo() {
  try {
    const result = await doSomething();
    const newResult = await doSomethingElse(result);
    const finalResult = await doThirdThing(newResult);
    console.log(`Got the final result: ${finalResult}`);
  } catch(error) {
    failureCallback(error);
  }
}
```

### References
- Js Promise - [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
