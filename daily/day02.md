---
title: "Day 2: Variables and Data Types in JavaScript 📦"
tags: [javascript, variables, data types, basics, beginner]
level: beginner
day: 2
author: Ajay Dhangar
---

# 📅 Day 2: Variables and Data Types in JavaScript

Welcome to **Day 2** of your JavaScript journey! Today, we’ll learn how to **store and organize data** in JavaScript using variables and understand the different **data types** available.

---

## 📌 What You'll Learn Today

- What variables are and how to declare them
- Difference between `var`, `let`, and `const`
- Primitive vs Non-primitive data types
- Best practices for variable naming
- Common mistakes and how to avoid them

---

## 📦 What are Variables?

Variables are containers that store **data values**. In JavaScript, variables are essential to store, update, and retrieve information during the execution of a program. Variables allow you to **reuse** values without having to write them multiple times.

<center><b>OR</b></center>

<br/>


Variables are like **containers** that hold values we want to use or change later in our code.

> 💡 Think of a variable as a **box** in which you can store anything — your name, age, marks, status, etc.


### Example:

If you want to store your name, you can create a variable called `username` and assign it the value `"Ajay"`:

```js
let username = "Ajay";
let age = 25;
let isStudent = true;
```

---

## 🧠 Why Use Variables?

Imagine writing your name 10 times — instead, store it in a variable and reuse it!
Variables allow you to:

* Store data
* Reuse values
* Update values dynamically
* Write clean and readable code

---

## 🏷️ Naming Variables

When naming variables, follow these rules:

1. **Start with a letter, underscore (_), or dollar sign ($)**: `let _name;`, `let $age;`
2. **No spaces or special characters**: `let first name;` is invalid
3. **Case-sensitive**: `let Name;` and `let name;` are different
4. **Use meaningful names**: `let totalMarks;` is better than `let a;`
5. **Avoid reserved keywords**: `let let;` is invalid

## 🔁 Ways to Declare Variables

JavaScript gives you **three keywords** to declare variables:

| Keyword | Scope    | Reassignment | Hoisting | Use Case                                        |
| ------- | -------- | ------------ | -------- | ----------------------------------------------- |
| `var`   | Function | ✅ Yes        | ✅ Yes    |  Old-school JS; avoid if possible                |
| `let`   | Block    | ✅ Yes        | 🚫 No    | Recommended for variables that change           |
| `const` | Block    | ❌ No         | 🚫 No    | Recommended for constants (non-changing values) |

---

## 📌 Syntax

```js
// Using var
var VariableName = value;

// Using let
let VariableName = value;

// Using const
const VariableName = value;
```

### Examples:

```js
var city = "Delhi";       // Avoid using var
let score = 100;          // Preferred for values that may change
const country = "India";  // Preferred for fixed values
```

---

## 🔠 JavaScript Data Types

There are two main categories:

### 🟨 Primitive Data Types (Simple values)

| Type      | Example                |
| --------- | ---------------------- |
| String    | `"Hello"`              |
| Number    | `25`, `99.5`           |
| Boolean   | `true`, `false`        |
| Undefined | `let x;`               |
| Null      | `let y = null;`        |
| BigInt    | `1234567890123456789n` |
| Symbol    | `Symbol('id')`         |

### 🟩 Non-Primitive Data Types (Objects)

| Type     | Description     | Example                     |
| -------- | --------------- | --------------------------- |
| Object   | Key-value pairs | `{ name: "Ajay", age: 25 }` |
| Array    | List of items   | `[1, 2, 3, 4]`              |
| Function | Reusable block  | `function greet() {}`       |

---

## 🔥 Important Differences

```js
// var is function-scoped
function testVar() {
  var a = 10;
  if (true) {
    var a = 20;
    console.log("Inside if:", a); // 20
  }
  console.log("Outside if:", a); // 20
}
testVar();

// let is block-scoped
function testLet() {
  let b = 10;
  if (true) {
    let b = 20;
    console.log("Inside if:", b); // 20
  }
  console.log("Outside if:", b); // 10
}
testLet();

// const is also block-scoped

function testConst() {
  const c = 10;
  if (true) {
    const c = 20;
    console.log("Inside if:", c); // 20
  }
  console.log("Outside if:", c); // 10
}
testConst();
```

---

## 🔍 Real-life Example

```javascript
let username = "Ajay";
let greeting = "Hello, " + username + "!";

console.log(greeting); // Hello, Ajay!
```

---

## 🚫 Common Mistakes

| Mistake                           | What Happens?                        |
| --------------------------------- | ------------------------------------ |
| Reassigning a `const` variable    | ❌ Error                              |
| Using a variable before declaring | `var`: undefined; `let/const`: error |
| Declaring the same `let` twice    | ❌ Error                              |

---

## 💡 Best Practices

* Prefer `const` by default; use `let` when you need to reassign.
* Avoid `var` — it leads to confusing bugs.
* Use meaningful names: `let price = 100;` not `let p = 100;`

---

## ✍️ Mini Task

```javascript
const firstName = "Ajay";
let age = 22;
let course = "JavaScript for 200 Days";

console.log(`${firstName} is ${age} years old and learning ${course}.`);
```

**👉 Output:**

```
Ajay is 22 years old and learning JavaScript for 200 Days.
```

---

## 🧩 Coding Challenge

```javascript
// Create a price calculator

const price = 450;
const taxRate = 0.18;
let finalPrice = price + (price * taxRate);

console.log("Final Price with GST:", finalPrice);
```

---


## 🧠 Quiz Time

**Q1:** What will be the result of this code?

```js
let name;
console.log(name);
```

* a) Error
* b) `null`
* ✅ c) `undefined`

---

## 🧪 Practice Challenges

### 🟡 Task 1:

Declare 3 variables for:

* Your name (string)
* Your age (number)
* Whether you're learning JavaScript (boolean)

### 🟢 Task 2:

Create an object called `student` with:

```js
{
  name: "Ajay",
  age: 22,
  isStudent: true
}
```

Access the name using `student.name`

---

## 🚫 Common Mistakes to Avoid

* Using `var` (avoid it unless required)
* Forgetting `let` or `const` before a variable
* Trying to reassign a `const` variable

---



### 📚 Homework

1. Explain the difference between `var`, `let`, and `const` in your own words.
2. Try declaring a variable using all three and print them.
3. Explore what happens if you redeclare a `let` variable.

---

## 🔁 Recap

* JavaScript has **7 primitive** and **3 main non-primitive** data types
* Use `let` for reassignable variables and `const` for fixed ones
* Objects and Arrays are powerful ways to store grouped data

---

## 📚 Recommended Resources (🔗 Useful Resources)

* [JavaScript Variables – MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#declarations)
* [W3Schools: JavaScript Data Types](https://www.w3schools.com/js/js_datatypes.asp)
* [JavaScript Basics – JavaScript.info](https://javascript.info/)
* [MDN Docs: var, let, const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)
* [JavaScript Scope — W3Schools](https://www.w3schools.com/js/js_scope.asp)
* [Video: JavaScript Variables in Hindi](https://www.youtube.com/watch?v=Bv_5Zv5c-Ts)

---

## ⏭️ Next Day: [Day 3 → Operators in JavaScript](./day03.md)

---

> 💬 **Have questions?** Drop them in [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 **Found a bug or improvement?** [Open an Issue](https://github.com/ajay-dhangar/200-days-of-javascript/issues/new)
