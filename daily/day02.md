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

Variables are like **containers** that hold values we want to use or change later in our code.

> 💡 Think of them as boxes where you store names, numbers, or anything you want your program to remember and use later.

### Example:

```js
let username = "Ajay";
let age = 25;
let isStudent = true;
````

---

## 🧾 Declaring Variables

### ✅ 3 Ways to Declare:

| Keyword | Scope    | Reassignment | Hoisting | Recommended? |
| ------- | -------- | ------------ | -------- | ------------ |
| `var`   | Function | ✅ Yes        | ✅ Yes    | ❌ No         |
| `let`   | Block    | ✅ Yes        | ❌ No     | ✅ Yes        |
| `const` | Block    | ❌ No         | ❌ No     | ✅ Yes        |

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

## 🔁 Recap

* JavaScript has **7 primitive** and **3 main non-primitive** data types
* Use `let` for reassignable variables and `const` for fixed ones
* Objects and Arrays are powerful ways to store grouped data

---

## 📚 Recommended Resources

* [JavaScript Variables – MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#declarations)
* [W3Schools: JavaScript Data Types](https://www.w3schools.com/js/js_datatypes.asp)
* [JavaScript Basics – JavaScript.info](https://javascript.info/)

---

## ⏭️ Next Day: [Day 3 → Operators in JavaScript](./day03.md)

---

> 💬 **Have questions?** Drop them in [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 **Found a bug or improvement?** [Open an Issue](https://github.com/ajay-dhangar/200-days-of-javascript/issues/new)
