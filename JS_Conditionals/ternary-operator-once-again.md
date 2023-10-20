<!-- omit in toc -->
# Mastering the JavaScript Ternary Operator: Once Again

- [Introduction:](#introduction)
- [Understanding the Syntax:](#understanding-the-syntax)
- [Handling Multiple Conditions:](#handling-multiple-conditions)
- [Non-Traditional Usage:](#non-traditional-usage)
- [Benefits of Using the Ternary Operator:](#benefits-of-using-the-ternary-operator)
- [Key Takeaways](#key-takeaways)


## Introduction:

The JavaScript ternary operator is a powerful tool that allows developers to write more concise and readable code when dealing with conditional statements. This operator is often used as a compact alternative to if-else statements, making your code more elegant and easier to understand. In this blog, we'll explore the syntax, examples, and benefits of the JavaScript ternary operator to help you master this essential concept in JavaScript programming.

## Understanding the Syntax:

The syntax of the JavaScript ternary operator is quite straightforward:

```javascript
condition ? expression1 : expression2;
```

`condition` This is the test that gets evaluated. If it's true, `expression1` is executed; otherwise, `expression2` is executed.

**Examples:*

Let's dive into some practical examples to see how the JavaScript ternary operator works.

**Example 1: Voting Eligibility**

```javascript
const age = 22;
const canVote = (age >= 18) ? 'Yes' : 'No';
console.log(canVote); // Output: Yes
```

In this example, if the condition `age >= 18` is true, the string `Yes` is assigned to the `canVote` variable; otherwise, it's assigned `No`.

**Example 2: Checking for Even Numbers**

```javascript
const number = 7;
const isEven = (number % 2 === 0) ? true : false;
console.log(isEven); // Output: false
```

Here, the condition `number % 2 === 0` is checked. If it's true, `true` is assigned to `isEven`; otherwise, it's `false`.

**Example 3: Greeting Based on Time**

```javascript
const greeting = 'Good ' + ((new Date().getHours() < 12) ? 'morning' : 'afternoon');
console.log(greeting); // Output: Good morning or Good afternoon, depending on the current time
```

In this case, the condition checks if it's before noon. If it is, it appends the string `morning` to `Good `. Otherwise, it appends `afternoon`.

## Handling Multiple Conditions:

The JavaScript ternary operator is not limited to just two conditions; you can chain multiple conditions together for more complex scenarios.

```javascript
let age = prompt('age?', 18);

let message = (age < 3) ? 'Hi, baby!' :
  (age < 18) ? 'Hello!' :
  (age < 100) ? 'Greetings!' :
  'What an unusual age!';

alert(message);
```

Here, the code evaluates different age ranges and returns an appropriate message. It's equivalent to using an `if-else` statement, but in a more compact form.

## Non-Traditional Usage:

While the ternary operator is incredibly versatile, it's best suited for returning values based on conditions. It can also be used to execute different code based on conditions, but this isn't recommended for readability purposes.

**Non-recommended Usage:**

```javascript
let company = prompt('Which company created JavaScript?', '');

(company == 'Netscape') ?
   alert('Right!') : alert('Wrong.');
```

This example executes different code based on the condition `company == 'Netscape'`, but it's less readable than the equivalent `if` statement.

**Recommended Usage:**

```javascript
let company = prompt('Which company created JavaScript?', '');

if (company == 'Netscape') {
  alert('Right!');
} else {
  alert('Wrong.');
}
```

In this case, an `if` statement is more readable for simple branching.

## Benefits of Using the Ternary Operator:

The JavaScript ternary operator offers several advantages:

1. **Conciseness:** It allows you to express conditional logic in a more compact and readable manner.
2. **Flexibility:** You can use it for various scenarios, from basic assignments to complex expressions.
3. **Reduced Repetition:** It helps you avoid repeating similar code blocks found in lengthy `if-else` statements.

## Key Takeaways

- The JavaScript ternary operator is a concise way to write conditional statements.
- Its syntax consists of a condition, followed by a question mark, an expression for the true case, a colon, and an expression for the false case.
- It can be used for simple assignments or more complex expressions.
- The ternary operator can help write more readable and concise code, reducing repetition.

[Previous Ternary Operator Note](../JS_Operators/javascript-ternary-operator.md)

---
[Previous](./javascript-if-else.md) | [Next]()