<!-- omit in toc -->
# Understanding JavaScript Data Types: A Comprehensive Guide

- [Introduction](#introduction)
- [1. Primitive Types](#1-primitive-types)
  - [String:](#string)
  - [Number:](#number)
  - [Boolean:](#boolean)
  - [Undefined:](#undefined)
  - [Null:](#null)
  - [Symbol:](#symbol)
- [2. Object Type](#2-object-type)
- [3. Array Type](#3-array-type)
- [4. Function Type](#4-function-type)
- [5. Type Conversion](#5-type-conversion)
- [Key Takeaways](#key-takeaways)


## Introduction

JavaScript, as a dynamically-typed language, allows you to work with various data types. These data types are the building blocks of your code, helping you define, manipulate, and transform information efficiently. In this blog, we'll explore JavaScript's data types, making the concept easy to grasp for beginners.

## 1. Primitive Types

JavaScript has six primitive data types:

### String:

It represents sequences of characters and strings are immutable in JavaScript, which means that once a string is created, it cannot be changed.

```javascript
const greeting = "Hello, World!";
const name = 'Alice';
```

### Number:

It covers all numeric values, including integers and floating-point numbers.

```javascript
const age = 30;
const price = 9.99;
```

### Boolean:

Represents logical entities with two values: `true` and `false`.

```javascript
const isLogged = true;
const hasPermission = false;
```

### Undefined:

It represents the absence of a value. Variables that are declared but not assigned a value are automatically set to `undefined`.

```javascript
let username;
console.log(username); // Outputs: undefined
```

### Null:

It represents the intentional absence of any value. It's often used to indicate the absence of an object or value. It is usually assigned to variables as a way to clear their contents.

```javascript
let person = null;
console.log(person); // Outputs: null
```

### Symbol:

A unique and immutable value, frequently used as object property keys to prevent naming clashes.

```javascript
const id = Symbol('id');
const obj = {
  name: 'John',
  [id]: 123
};
```

## 2. Object Type

The object in JavaScript is a complex data type that can hold multiple values(property) in key-value pairs. The value of an object's property(key-value pairs) can be of any type.

```javascript
const person = {
  name: 'Alice',
  age: 30,
  isStudent: true
};
```

## 3. Array Type

An array is a special type of object that is used to store multiple values in a single variable. Each value in an array is called an element, and it is identified by an index(starts from 0). Arrays can accommodate elements of different types.

```javascript
const fruits = ['apple', 'banana', 'orange'];
const numbers = [1, 2, 3, 4, 5];
const mixed = ['John', 30, true, null];
```

## 4. Function Type

In JavaScript, functions are first-class objects, which means that they can be assigned to variables, passed as arguments to other functions, or returned as values from other functions. Functions can be defined using function declarations or function expressions.

```javascript
function sayHello(name) {
  console.log(`Hello, ${name}!`);
}

const add = function(a, b) {
  return a + b;
};
```

## 5. Type Conversion

JavaScript provides built-in functions to convert values from one type to another. These functions include:

- `String()`: Converts a value to a string.
- `Number()`: Converts a value to a number.
- `Boolean()`: Converts a value to a boolean.
- `parseInt()`: Converts a string to an integer.
- `parseFloat()`: Converts a string to a floating-point number.

```javascript
const num = 10;
const str = String(num);

console.log(typeof num); // Outputs: number
console.log(typeof str); // Outputs: string
```

## Key Takeaways

- JavaScript features primitive types like string, number, boolean, undefined, null, and symbol.
- Objects store data in key-value pairs.
- Arrays efficiently manage multiple values.
- Functions are versatile and can be used in various ways.
- JavaScript's type conversion functions aid in seamless data transformation.

Embrace the diversity of JavaScript types to become a proficient developer, crafting code that meets your project's unique needs.

---

[Previous](./statically-typed-vs-dynamically-typed.md) | [Next](./alert-prompt-and-confirm.md)