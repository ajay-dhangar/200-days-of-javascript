---
title: "Day 06: Data Types & Type Conversion"
tags: [javascript, data-types, type-conversion, beginner]
level: beginner
day: 06
author: Ajay Dhangar
---

# 📅 Day 06: [Data Types & Type Conversion]

> 🎯 **Goal**: Understand the different data types in JavaScript and how type conversion works implicitly and explicitly.

---

## 📌 What You'll Learn

* JavaScript primitive and non-primitive data types.
* How to check data types using `typeof`.
* Implicit vs. explicit type conversion.
* Common pitfalls with type coercion in JavaScript.

---

## 📖 Introduction

In JavaScript, **data types** define the kind of value a variable can hold. JavaScript is a **dynamically typed** language, meaning you don’t need to specify a type when declaring a variable. However, understanding data types is essential when writing robust programs and debugging type-related bugs.

---

## 🧱 JavaScript Data Types

JavaScript has two main categories of data types:

### ✅ Primitive Data Types (Immutable)

These hold a single value and are stored directly in the variable's memory location. They are immutable, meaning their values cannot be changed.

**Primitive data types include:**

1. **String**  
2. **Number**  
3. **BigInt**  
4. **Boolean**  
5. **Undefined**  
6. **Null**  
7. **Symbol**

```js
const str = "Hello";        // String
const num = 42;             // Number
const bigInt = 123n;        // BigInt
const isTrue = true;        // Boolean
let notDefined;             // Undefined
const nothing = null;       // Null
const unique = Symbol("id"); // Symbol
```

### ✅ Non-Primitive Data Types (Objects)

These can hold multiple values and are stored as references in memory. They are mutable, meaning their values can be changed.

**Non-primitive data types include:**

1. **Object**
2. **Array**
3. **Function**

```js
const obj = { name: "Ajay" };            // Object
const arr = [1, 2, 3];                   // Array
function greet() { return "Hello!"; }    // Function
```

---

## 📏 Checking Data Types: `typeof`

```js
console.log(typeof "hello");   // "string"
console.log(typeof 100);       // "number"
console.log(typeof true);      // "boolean"
console.log(typeof undefined); // "undefined"
console.log(typeof null);      // "object" (known quirk in JS)
console.log(typeof {});        // "object"
console.log(typeof []);        // "object"
console.log(typeof function() {}); // "function"
```

> ⚠️ Note: `typeof null` returns `"object"` due to a legacy bug in JavaScript.

---

## 🔄 Type Conversion

### Implicit Conversion (Type Coercion)

JavaScript automatically converts one data type to another when necessary. This can lead to unexpected results if not careful.

```js
console.log("5" + 1);     // "51" (number 1 is coerced to string)
console.log("5" - 1);     // 4 (string "5" is coerced to number)
console.log("5" * "2");   // 10
console.log(true + 1);    // 2 (true becomes 1)
```

### Explicit Conversion

You can manually convert data types using built-in functions.

#### To Number

```js
Number("123");       // 123
Number("abc");       // NaN
parseInt("123.45");  // 123
parseFloat("123.45");// 123.45
```

#### To String

```js
String(123);         // "123"
(123).toString();    // "123"
```

#### To Boolean

```js
Boolean(0);          // false
Boolean(1);          // true
Boolean("");         // false
Boolean("hello");    // true
Boolean(null);       // false
Boolean([]);         // true
```

---

## 🧪 Practice Tasks

### ✅ Task 1: Detect and Display All Data Types

```js
const variables = ["hello", 42, true, null, undefined, {}, [], function () {}];

variables.forEach((item) => {
  console.log(`${item} → ${typeof item}`);
});
```

### ✅ Task 2: Write a Function That Converts Input to All Types

```js
function convertTypes(value) {
  return {
    original: value,
    toString: String(value),
    toNumber: Number(value),
    toBoolean: Boolean(value),
  };
}

console.log(convertTypes("123")); // Try with numbers, booleans, null, etc.
```

### ✅ Task 3: Demonstrate Type Coercion Pitfalls

```js
console.log("10" + 5);  // "105"
console.log("10" - 5);  // 5
console.log(true + true); // 2
console.log(null + 1);  // 1
console.log(undefined + 1); // NaN
```

---

## ❗ Common Mistakes

* Using `==` instead of `===` which performs **type coercion**.

  ```js
  console.log(0 == "0");  // true
  console.log(0 === "0"); // false
  ```

* Expecting `typeof null` to return `"null"`.

  ```js
  console.log(typeof null); // "object"
  ```

* Confusing `parseInt("10px")` vs `Number("10px")`.

  ```js
  console.log(parseInt("10px")); // 10
  console.log(Number("10px"));   // NaN
  ```

---

## 💡 Interview Tips

* Know the **7 primitive types** and how they differ from objects.
* Be able to **explain coercion vs. conversion** with examples.
* Always prefer `===` over `==` unless you have a good reason.
* Understand how `typeof`, `instanceof`, and `Array.isArray()` help in type checking.

---

## 📚 Additional Resources

* [MDN: JavaScript Data Types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
* [MDN: Type Conversions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#type_conversions)
* [W3Schools: JavaScript Data Types](https://www.w3schools.com/js/js_datatypes.asp)

---

## 🔁 Recap

* JavaScript supports both primitive and non-primitive data types.
* Use `typeof` to check variable types, but beware of some quirks.
* Implicit and explicit type conversion are common in JS.
* Always check and convert data types explicitly to avoid bugs.

---

## ⏭️ Next Day: [Day 07 → Strings & String Methods](./day07.md)

---

> 💬 Have doubts? Ask in [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 Found a mistake? [Raise a Pull Request](https://github.com/ajay-dhangar/200-days-of-javascript/pulls)