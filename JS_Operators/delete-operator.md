<!-- omit in toc -->
# Mastering the JavaScript `delete` Operator

- [Introduction](#introduction)
- [Deleting Object Properties](#deleting-object-properties)
- [Deleting Array Elements](#deleting-array-elements)
- [Deleting Variables](#deleting-variables)
- [Deleting Built-in Object Properties](#deleting-built-in-object-properties)
- [Key Takeaways](#key-takeaways)


## Introduction

In the world of JavaScript, the `delete` operator is your dynamic companion. It empowers you to modify the structure of objects and arrays by removing specific properties and elements. Let's dive into the world of property vanishing acts and element evictions.

## Deleting Object Properties

Deleting a property from an object is a breeze. Just use the `delete` operator followed by the object's property name. For example:

```javascript
const person = { name: 'John', age: 30 };
delete person.age;
console.log(person); // { name: 'John' }
```

In this example, the `age` property vanishes from the `person` object, leaving only the `name` property.

## Deleting Array Elements

Similar to object properties, you can use the `delete` operator to remove elements from an array. However, it's important to note that using `delete` won't change the array's length:

```javascript
const numbers = [1, 2, 3, 4, 5];
delete numbers[2];
console.log(numbers); // [1, 2, empty, 4, 5]
console.log(numbers.length); // 5
```

Here, the element at index 2 is removed, but the length of the array remains the same. To fully remove an element and adjust the length, you can use the `splice` method:

```javascript
const numbers = [1, 2, 3, 4, 5];
numbers.splice(2, 1);
console.log(numbers); // [1, 2, 4, 5]
console.log(numbers.length); // 4
```

## Deleting Variables

It's important to understand that the `delete` operator cannot be used to delete variables declared with `var`, `let`, or `const`:

```javascript
let x = 10;
var y = 20;
delete x; // false
delete y; // false
console.log(x); // 10
console.log(y); // 20
```

As seen in the example, attempting to delete variables `x` and `y` returns `false`, and the variables remain unaffected.

## Deleting Built-in Object Properties

The `delete` operator is versatile—it can also be used to delete properties of built-in JavaScript objects, such as the `global` object (`window` in browsers). For example:

```javascript
delete window.document; // true
console.log(window.document); // undefined
```

Here, the `document` property of the `window` object is deleted, rendering it inaccessible.

## Key Takeaways

- The `delete` operator is used to delete properties from objects or remove elements from arrays.
- When used with objects, the `delete` operator removes the specified property.
- When used with arrays, the `delete` operator removes the specified element but does not change the array's length.
- Variables declared with `var`, `let`, or `const` cannot be deleted using the `delete` operator.
- The `delete` operator can also be used to delete properties of built-in JavaScript objects.

---

[Previous](./in-operator.md) | [Next](../JS_Conditionals/javascript-if-else.md)