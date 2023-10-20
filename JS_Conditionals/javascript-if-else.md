<!-- omit in toc -->
# Mastering If-Else: Navigating JavaScript's Conditional Statements

- [Introduction](#introduction)
- [`if` Statement](#if-statement)
- [`if else` Statement](#if-else-statement)
- [`if else if` Statement](#if-else-if-statement)
- [Key Takeaways](#key-takeaways)


## Introduction

Conditional statements in JavaScript act as the guiding principles, enabling your code to adapt, make decisions, and execute specific actions based on varying conditions. In this blog, we'll explore the three main types of conditional statements: `if`, `if else`, and `if else if`. These tools are crucial for ensuring your code behaves intelligently and responds to different scenarios.

## `if` Statement

The `if` statement serves as your code's gatekeeper. It checks a specified condition and, if the condition is true, allows a specific code block to run. The syntax is as follows:

```javascript
if (condition) {
  // code to be executed if the condition is true
} 
```

Here, `condition` can be any JavaScript expression that results in a boolean value (`true` or `false`). When the condition evaluates to `true`, the code within the curly braces is executed; otherwise, it's skipped.

**Example:**

```javascript
let age = 18;

if (age >= 18) {
  console.log("You are old enough to vote");
}
```

In this example, if the `age` variable is 18 or older, the message "You are old enough to vote" is printed to the console.

## `if else` Statement

The `if else` statement is your code's compass. It steers in two directions, executing different code blocks based on a condition. If the condition in the `if` statement is true, the code block within the `if` block is executed; otherwise, the code block within the `else` block takes charge. The syntax looks like this:

```javascript
if (condition) {
  // code to be executed if the condition is true
} else {
  // code to be executed if the condition is false
}
```

**Example:**

```javascript
let age = 16;

if (age >= 18) {
  console.log("You are old enough to vote");
} else {
  console.log("You are too young to vote");
}
```

In this example, the `age` variable determines the path. If the age is 18 or older, it's one way; otherwise, it's another.

## `if else if` Statement

The `if else if` statement is your code's multilayered decision maker. It allows you to test multiple conditions and execute different code blocks based on the outcomes. You can have as many `else if` blocks as needed between the `if` and `else` blocks. The syntax follows this structure:

```javascript
if (condition1) {
  // code to be executed if condition1 is true
} else if (condition2) {
  // code to be executed if condition2 is true
} else {
  // code to be executed if none of the conditions are true
}
```

Conditions are evaluated in sequence. If the first condition (`condition1`) is true, the code block within its associated block runs. If it's false but the next condition (`condition2`) is true, the code block in the `else if` block takes over. If none of the conditions are true, the code within the `else` block is executed.

**Example:**

```javascript
let grade = 75;

if (grade >= 90) {
  console.log("You got an A");
} else if (grade >= 80) {
  console.log("You got a B");
} else if (grade >= 70) {
  console.log("You got a C");
} else {
  console.log("You got an F");
}
```

Here, the `grade` variable determines the message printed to the console, depending on its value.

## Key Takeaways

- Conditional statements in JavaScript allow you to make decisions and execute different code blocks based on conditions.
- The `if` statement is used to execute a code block if a condition is true.
- The `if else` statement is used to execute one code block if a condition is true, and another code block if the condition is false.
- The `if else if` statement allows you to test multiple conditions and execute different code blocks based on the outcome of those conditions.

Conditional statements are your JavaScript allies, enabling your code to adapt to various scenarios. The `if` statement checks a condition and executes code when it's true. The `if else` statement chooses one path or another based on a condition. The `if else if` statement is your tool for intricate decision-making.

---
[Previous](../JS_Operators/delete-operator.md) | [Next](./ternary-operator-once-again.md)
