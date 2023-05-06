Sure, here's a comprehensive guide to every event in JavaScript.

# Every Event in JavaScript

JavaScript provides a wide range of events that you can listen for, including events related to user input, page loading, and network activity. Here's a list of every event in JavaScript, along with a brief description of each.

## Mouse Events

Mouse events are events that are triggered by user interaction with the mouse.

- `click`: Occurs when the element is clicked.
- `dblclick`: Occurs when the element is double-clicked.
- `mousedown`: Occurs when the mouse button is pressed down on the element.
- `mouseup`: Occurs when the mouse button is released on the element.
- `mousemove`: Occurs when the mouse pointer moves over the element.
- `mouseover`: Occurs when the mouse pointer enters the element.
- `mouseout`: Occurs when the mouse pointer leaves the element.

```javascript
let button = document.querySelector("button");

button.addEventListener("click", function() {
  console.log("Button clicked!");
});

button.addEventListener("mousemove", function() {
  console.log("Mouse move!");
});
```

In the example above, we add event listeners for the `click` and `mousemove` events on a button element. When the button is clicked or the mouse pointer moves over the button, the corresponding event listener is called and logs a message to the console.

## Keyboard Events

Keyboard events are events that are triggered by user interaction with the keyboard.

- `keydown`: Occurs when a key is pressed down while the element has focus.
- `keyup`: Occurs when a key is released while the element has focus.
- `keypress`: Occurs when a key is pressed down and then released while the element has focus.

```javascript
let input = document.querySelector("input");

input.addEventListener("keydown", function() {
  console.log("Key down!");
});

input.addEventListener("keyup", function() {
  console.log("Key up!");
});
```

In the example above, we add event listeners for the `keydown` and `keyup` events on an input element. When a key is pressed down or released while the input element has focus, the corresponding event listener is called and logs a message to the console.

## Form Events

Form events are events that are triggered by user interaction with form elements.

- `submit`: Occurs when the form is submitted.
- `reset`: Occurs when the form is reset.
- `change`: Occurs when the value of a form element is changed.
- `focus`: Occurs when a form element receives focus.
- `blur`: Occurs when a form element loses focus.

```javascript
let form = document.querySelector("form");

form.addEventListener("submit", function(event) {
  event.preventDefault();
  console.log("Form submitted!");
});

form.addEventListener("change", function() {
  console.log("Form changed!");
});
```

In the example above, we add event listeners for the `submit` and `change` events on a form element. When the form is submitted or a form element's value is changed, the corresponding event listener is called and logs a message to the console. Note that we also call `preventDefault` on the `submit` event to prevent the form from actually submitting.

## Window Events

Window events are events that are triggered by changes to the browser window.

- `load`: Occurs when the page finishes loading.
- `unload`: Occurs when the page is unloaded.
- `resize`: Occurs when the window is resized.
- `scroll`: Occurs when the window is scrolled.

```javascript
window.addEventListener("load", function() {
  console.log("Page loaded!");
});

window.addEventListener("resize", function() {
  console.log("Window resized!");
});
```

In the example above, we add event listeners for the `load` and `resize` events on the window object. When the page finishes loading or the window is resized, the corresponding event listener is called and logs a message to the console.

## Network Events

Network events are events that are triggered by network activity, such as loading resources from a server.

- `readystatechange`: Occurs when the readyState property of an XMLHttpRequest object changes.
- `loadstart`: Occurs when the browser starts to load a resource.
- `progress`: Occurs when the browser is downloading a resource.
- `abort`: Occurs when the browser aborts the loading of a resource.
- `error`: Occurs when the browser encounters an error while loading a resource.
- `load`: Occurs when the browser finishes loading a resource.
- `timeout`: Occurs when the browser times out while loading a resource.

```javascript
let xhr = new XMLHttpRequest();

xhr.addEventListener("load", function() {
  console.log("Resource loaded!");
});

xhr.addEventListener("error", function() {
  console.log("Error loading resource!");
});

xhr.open("GET", "https://example.com/resource");
xhr.send();
```

In the example above, we create an XMLHttpRequest object and add event listeners for the `load` and `error` events. When the resource is successfully loaded or an error occurs while loading the resource, the corresponding event listener is called and logs a message to the console.

## Conclusion

Events in JavaScript are a powerful tool for creating interactive web applications. By listening for events and responding to them with code, you can create dynamic and engaging user experiences. With this comprehensive guide to every event in JavaScript, you should be able to handle any event-related task that comes your way.
