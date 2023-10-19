<!-- omit in toc -->
# Understanding Data Types in JavaScript: A Comprehensive Guide

- [Introduction](#introduction)
- [Primitive Data Types](#primitive-data-types)
- [Non-Primitive Data Types](#non-primitive-data-types)
- [Type Conversion](#type-conversion)
  - [Automatic Type Conversion](#automatic-type-conversion)
  - [Explicit Type Conversion](#explicit-type-conversion)
- [Type Coercion](#type-coercion)
- [Key Takeaways](#key-takeaways)


## Introduction
JavaScript is a versatile and widely used programming language known for its flexibility and dynamic nature. One fundamental aspect of JavaScript that every developer must grasp is data types. Data types in JavaScript categorize the different kinds of data that a program can handle. Each data type comes with its own set of rules, properties, and methods, making it crucial for effective programming in JavaScript. In this blog post, we'll explore the various data types in JavaScript, including primitive and non-primitive types, and delve into the concepts of type conversion and coercion.

## Primitive Data Types

**Primitive data types** are the building blocks of JavaScript. They are called "primitive" because they represent single values and do not reference existing objects. Here are the six primitive data types in JavaScript:

1. **Boolean**: Represents either `true` or `false`.

  ```javascript
   const boolValue = true;
  ```

2. **Null**: Represents the intentional absence of any object value.

  ```javascript
  const nullValue = null;
  ```

3. **Undefined**: Represents a variable that has been declared but has not been assigned a value.

  ```javascript
  let undefinedVar;
  ```

4. **String**: Represents a sequence of characters enclosed in single or double quotes.

  ```javascript
  const stringValue = "This is a string";
  ```

5. **Number**: Represents numeric values, including integers and floating-point numbers.

  ```javascript
  const numberValue = 100;
  ```

6. **Symbol**: Represents a unique and immutable value primarily used as object property keys.

  ```javascript
  const symbolValue = Symbol("This is a symbol value");
  ```

## Non-Primitive Data Types

**Non-primitive data types** in JavaScript are more complex and can refer to pre-existing objects. These data types include:

1. **Array**: Represents a collection of values, indexed by numeric keys.

  ```javascript
 const arrayValue = [1, 2, 3, 4, 5];
  ```

2. **Object**: Represents a collection of key-value pairs, where keys are strings (or Symbols) and values can be of any data type.

  ```javascript
const objectValue = { name: 'John', age: 22, email: 'john@example.com' };
  ```

3. **Function**: Represents a reusable block of code that can be executed when called.

  ```javascript
function myFunction() {
  console.log("This is a function");
}
  ```

## Type Conversion

Type conversion in JavaScript involves changing the data type of a variable into another data type. JavaScript supports both automatic and explicit type conversion.

### Automatic Type Conversion

Automatic type conversion happens when JavaScript itself converts the data type of a variable based on the operation being performed. For example:

```javascript
const stringValue1 = "10";   // string
const numberValue1 = 10;    // number
const sum = stringValue1 + numberValue1;
console.log(sum);           // Output: "1010"
```

### Explicit Type Conversion

Explicit type conversion, on the other hand, is done by the programmer using various JavaScript functions. For instance, you can convert a string to a number explicitly:

```javascript
const stringNumberValue = "100";
const numberValue2 = Number(stringNumberValue);
console.log(typeof numberValue2);    // Output: number
```

## Type Coercion

Type coercion is the process of converting one data type into another implicitly by the JavaScript interpreter. This occurs when JavaScript tries to perform operations between different data types. For example:

```javascript
const sumString = "10" + 20; // Sum is concatenated
console.log(sumString); // Output: "1020"
```

## Key Takeaways

- JavaScript encompasses six primitive data types (Boolean, Null, Undefined, String, Number, and Symbol) and three non-primitive data types (Array, Object, and Function).

- JavaScript provides mechanisms for both automatic and explicit type conversion, allowing developers to work with different data types effectively.

- Type coercion in JavaScript involves implicit conversion of data types by the interpreter, often occurring during operations involving different data types.

---

[Previous](./javascript-const.md) | [Next](./statically-typed-vs-dynamically-typed.md)
