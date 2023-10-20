<!-- omit in toc -->
# Understanding JavaScript Operators: A Beginner's Guide

- [Introduction](#introduction)
- [Assignment Operators](#assignment-operators)
  - [Example:](#example)
- [Arithmetic Operators](#arithmetic-operators)
  - [Example:](#example-1)
- [Comparison Operators](#comparison-operators)
  - [Example:](#example-2)
- [Logical Operators](#logical-operators)
  - [Example:](#example-3)
- [Conditional (Ternary) Operator](#conditional-ternary-operator)
  - [Example:](#example-4)
- [Key Takeaways](#key-takeaways)


## Introduction

JavaScript operators are fundamental symbols that allow you to work with variables and values in various ways. These symbols are like the building blocks of JavaScript, enabling you to assign values, perform mathematical operations, compare values, and more. Let's dive into the world of JavaScript operators and make them easy to grasp for beginners.

## Assignment Operators

Assignment operators are used to give values to variables. The most common operator for this is the equals sign (=). It assigns the value on the right to the variable on the left. For instance:

```javascript
let x = 5; // assigns the value 5 to the variable x
```

But there are also other assignment operators that combine an arithmetic operation with assignment. These include:

- `+=`: Adds the value on the right to the variable and assigns the result to the variable.
- `-=`: Subtracts the value on the right from the variable and assigns the result.
- `*=`: Multiplies the variable by the right value and assigns the result.
- `/=`: Divides the variable by the right value and assigns the result.

### Example:

```javascript
let x = 10;
x += 5; // This is the same as writing x = x + 5, and it assigns the value 15 to the variable x.
```

## Arithmetic Operators

Arithmetic operators are all about doing math with numbers. Here are some of the common ones:

- `+`: Addition
- `-`: Subtraction
- `*`: Multiplication
- `/`: Division
- `%`: Modulus (it gives you the remainder when you divide)
- `++`: Increment (adds 1 to a variable)
- `--`: Decrement (subtracts 1 from a variable)

### Example:

```javascript
let x = 5;
let y = 2;

console.log(x + y); // prints 7
console.log(x - y); // prints 3
console.log(x * y); // prints 10
console.log(x / y); // prints 2.5
console.log(x % y); // prints 1

let z = 3;
z++; // Now, z is 4, equivalent to z = z + 1
z--; // Now, z is 3, equivalent to z = z - 1
```

## Comparison Operators

Comparison operators help us compare values and provide a simple answer: true or false. Here are some of the common ones:

- `==`: Equal to
- `!=`: Not equal to
- `>`: Greater than
- `<`: Less than
- `>=`: Greater than or equal to
- `<=`: Less than or equal to
- `===`: Strict equal to (compares both value and type)
- `!==`: Strict not equal to

### Example:

```javascript
let x = 5;
let y = 2;

console.log(x == y); // prints false
console.log(x != y); // prints true
console.log(x > y); // prints true
console.log(x < y); // prints false
console.log(x >= y); // prints true
console.log(x <= y); // prints false
console.log(x === '5'); // prints false
console.log(x !== '5'); // prints true
```

## Logical Operators

Logical operators let us combine multiple conditions to make decisions in our code. We have:

- `&&`: Logical AND (returns true if both conditions are true)
- `||`: Logical OR (returns true if at least one condition is true)
- `!`: Logical NOT (reverses the logical state of a condition)

### Example:

```javascript
let x = 5;
let y = 2;

console.log(x > 3 && y > 1); // prints true
console.log(x > 3 || y > 1); // prints true
console.log(!(x > 3)); // prints false
console.log(!(x < 3)); // prints true
```

## Conditional (Ternary) Operator

The conditional operator is a shorthand way of writing an if-else statement. It's perfect for making decisions in your code. Here's how it works:

```javascript
condition ? expression1 : expression2;
```

If the condition is true, `expression1` is executed; if the condition is false, `expression2` is executed.

### Example:

```javascript
let x = 5;
let result = x > 3 ? 'x is greater than 3' : 'x is not greater than 3';
console.log(result); // prints 'x is greater than 3'
```

## Key Takeaways

- Assignment operators give values to variables.
- Arithmetic operators perform mathematical calculations.
- Comparison operators help compare values and return true or false.
- Logical operators combine multiple conditions for logical operations.
- The conditional operator is a handy shortcut for making decisions in your code.

Understanding these JavaScript operators is a key step in becoming proficient with the language. They are the tools that help you control the flow and behavior of your programs. So, keep practicing and experimenting to become a JavaScript pro!

---

[Previous](../basics/alert-prompt-and-confirm.md) | [Next](./javascript-ternary-operator.md)