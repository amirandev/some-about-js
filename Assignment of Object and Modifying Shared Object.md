### Explanation: Assignment of Object and Modifying Shared Object

When an object is assigned to a variable in JavaScript and then the same object is assigned to another variable, any changes made to the object through either variable will affect the shared object. This is due to the nature of reference types in JavaScript.

Let's examine an example to understand this behavior:

```javascript
let a = {name: 'John'};
let b = a;

b.name = 'Jane';

console.log(a.name); // Output: Jane
console.log(b.name); // Output: Jane
