<!-- omit in toc -->
# JavaScript's `typeof` Operator

- [Introduction](#introduction)
- [Examples](#examples)
  - [Numeric Insights](#numeric-insights)
  - [String Speculation](#string-speculation)
  - [The Boolean Breakdown](#the-boolean-breakdown)
  - [Object Orientation](#object-orientation)
  - [Arrays Unveiled](#arrays-unveiled)
  - [The Function Frontier](#the-function-frontier)
- [Caution](#caution)
- [Key Takeaways](#key-takeaways)


## Introduction

The `typeof` operator in JavaScript is like your digital detective, helping you identify the data type of a variable or value. It provides a neat way to peek into the nature of your data. Whether you're working with conditional statements or need to debug your code, `typeof` is your go-to tool.

Let's start with the syntax:

```javascript
typeof operand
```

The `operand` here is the value or variable you're curious about. It's as simple as that!

## Examples

Now, let's dive into some practical examples:

### Numeric Insights

```javascript
let age = 25;
console.log(typeof age); // Output: "number"
```

### String Speculation

```javascript
let name = "John";
console.log(typeof name); // Output: "string"
```

### The Boolean Breakdown

```javascript
 let isActive = true;
console.log(typeof isActive); // Output: "boolean"
```

### Object Orientation

```javascript
let person = { firstName: "John", lastName: "Doe" };
console.log(typeof person); // Output: "object"
```

### Arrays Unveiled

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(typeof fruits); // Output: "object"
```

### The Function Frontier

```javascript
let calculateArea = function(width, height) {
return width * height;
};
console.log(typeof calculateArea); // Output: "function"
```

## Caution

However, there are a few things to keep in mind when dealing with the `typeof` operator:

- **Null's Identity Crisis:** If your operand is `null`, JavaScript may play a trick on you by returning "object." It's a known quirk in JavaScript.

- **Function Foreshadowing:** Functions have a special place in JavaScript's heart. So, if your operand is a function, `typeof` will spill the beans and reveal "function."

- **Array Ambiguity:** Arrays, being a type of object in JavaScript, will also perplex you by showing "object" when you use `typeof`.

## Key Takeaways

- The `typeof` operator is used to determine the data type of a value or variable in JavaScript.
- It returns a string indicating the type of the operand.
- The `typeof` operator can help with conditional statements or debugging to check the data type of a variable.
- The `typeof` operator has some caveats, such as returning `"object"` for `null` and arrays, and returning `"function"` for functions.

---

[Previous](./javascript-ternary-operator.md) | [Next](./in-operator.md)