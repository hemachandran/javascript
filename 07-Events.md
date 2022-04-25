# Js Events
When user interacts with HTML Elements and triggers an action is known as events
- For example:
  1. On selects, clicks, or hovers the cursor over a certain element.
  2. The user presses a key on the keyboard.
  3. The user resizes or closes the browser window.
  4. A web page finishes loading.
  5. A form is submitted.
  6. A video is played, paused and more...

### Adding Event Listener
```html
<button>Change color</button>
```

```javascript
//Get button element by document function - querySelector
const btn = document.querySelector('button');

const changeBackground = () => {
document.body.style.backgroundColor = "blue";
}

//addEventListener - an event, which execute on click action to change colour

btn.addEventListener('click', changeBackground );
```
- `focus`, `dblclick`, `mouseover`, `mouseout` few events can be used in `addEventListener`

### Removing Event Listeners
```javascript
btn.removeEventListener('click', changeBackground);
```

### Multiple Events
```javascript
myElement.addEventListener('click', functionA);
myElement.addEventListener('click', functionB);
```

### Inline Events
```html
<button onclick="changeBackground()">Change</button>
```

### Event objects


### References
- Events [Click here](https://developer.mozilla.org/en-US/docs/Web/API/Event)
