# What is JIT compiler? Is JavaScript compiled or interpreted or both?<!-- omit in toc -->

- [What is JIT compiler?](#what-is-jit-compiler)
- [So is JavaScript Compiled or Interpreted?](#so-is-javascript-compiled-or-interpreted)
- [Key Takeaways:](#key-takeaways)


## What is JIT compiler?

A **Just-In-Time (JIT)** compiler is a type of compiler that dynamically converts programming code into machine code at runtime, just before the code is executed. Unlike traditional compilers that convert the entire program ahead of time, a JIT compiler optimizes and compiles code on-the-fly, as it is needed.

The primary advantage of a JIT compiler is that it can make the execution of code significantly faster compared to an interpreter. It achieves this by analyzing the code at runtime, identifying hotspots (frequently executed portions of code), and applying various optimization techniques to generate highly efficient machine code specific to the underlying hardware.

JIT compilers are commonly used in programming languages such as Java and JavaScript, where the execution speed of the code is crucial.

## So is JavaScript Compiled or Interpreted?

JavaScript is generally considered an **interpreted language**. Traditionally, JavaScript code is executed by an interpreter, which reads each line of code sequentially and executes it immediately.

However, modern JavaScript engines, such as **V8 (used in Google Chrome)** or **SpiderMonkey (used in Mozilla Firefox)**, actually use a combination of interpretation and compilation techniques. These engines employ a JIT compiler to optimize and compile certain parts of the JavaScript code into machine code for faster execution.

For example, look at this program:

```javascript
console.log('Hello World');
oops oops; //SyntaxError: Unexpected identifier 'oops'
```

In theory, an interpreter would read the first line, print ***“Hello World”*** and only then throw a ***`Syntax Error`***. But for modern JavaScript’s runtime environments, this is not the case, immediately after running the program, before executing the log function, it crashes.

Another example is Hoisting, consider:

```javascript
console.log(max(1, 2));  // Output: 2
function max(num1, num2){
  return num1 > num2 ? num1 : num2;
}
```

How does the JS engine know about the ***‘max’*** Function before it reaches to the deceleration? Again, the only reasonable answer to this question is that the code must first be compiled before execution.

When running JavaScript code, the JavaScript engine initially interprets the code to quickly execute it. However, as the engine identifies hotspots or frequently executed portions of code, it may decide to compile them using the JIT compiler. The compiled code is then executed, resulting in improved performance.

Example:

```javascript
function add(a, b) {
  return a + b;
}
console.log(add(3, 5));
```

In this example, the JavaScript engine would interpret and execute the ***`add`*** function when it is called. However, if the ***`add`*** function is frequently used, the engine may decide to compile it using the JIT compiler for better performance.

> In summary, JavaScript can be seen as both interpreted and compiled, as it uses interpretation for quick execution and JIT compilation for optimizing performance when necessary.

## Key Takeaways:

- A JIT compiler dynamically converts programming code into machine code at runtime, just before execution.
- It optimizes and compiles code on-the-fly, leading to faster execution compared to an interpreter.
- JavaScript is primarily an interpreted language, but modern JavaScript engines use a combination of interpretation and JIT compilation techniques for improved performance.
- JavaScript engines interpret the code initially and may decide to compile frequently executed portions of code using the JIT compiler.

---

[Previous](./compilation-and-interpretation.md) | [Next](./jit-compiler-how-it-works-for-js.md)