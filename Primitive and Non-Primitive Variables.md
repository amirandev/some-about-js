# Primitive and Non-Primitive Variables

In programming, variables are used to store and manipulate data. In JavaScript, variables can be categorized into two main types: primitive variables and non-primitive variables. This article will explain the differences between these two types of variables.

## Primitive Variables

Primitive variables are basic data types that store simple values directly. They include the following types:

### Number

The number type represents numeric values, both integers and floating-point numbers.

```javascript
let age = 25;
```

### String

The string type represents a sequence of characters.

```javascript
let message = "Hello, world!";
```

### Boolean

The boolean type represents logical values: `true` or `false`.

```javascript
let isRaining = true;
```

### Null

The null type represents the absence of any object value.

```javascript
let myVariable = null;
```

### Undefined

The undefined type represents the absence of a defined value.

```javascript
let myVariable;
```

### Symbol

The symbol type represents a unique identifier.

```javascript
let id = Symbol("uniqueId");
```

## Non-Primitive Variables

Non-primitive variables, also known as reference variables, store references to complex objects or data structures. They include the following types:

### Array

An array is an ordered list of values, which can be of any type.

```javascript
let numbers = [1, 2, 3, 4, 5];
```

### Object

An object is an unordered collection of key-value pairs, where each value can be of any type.

```javascript
let person = {
  name: "John",
  age: 30,
  city: "New York"
};
```

### Function

A function is a reusable block of code that can be invoked with given arguments.

```javascript
function sayHello(name) {
  console.log("Hello, " + name + "!");
}
```
