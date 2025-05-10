---
title: "Day 3: Operators in JavaScript ⚙️"
tags: [javascript, operators, arithmetic, comparison, logical, beginner]
level: beginner
day: 3
author: Ajay Dhangar
---

# 📅 Day 3: JavaScript Operators Explained with Examples

Welcome to **Day 3** of your JavaScript learning path! Today we’ll dive deep into **operators** — the tools that let us perform actions on variables and values.

---

## 📌 What You'll Learn

- What are operators in JavaScript?
- Types of operators:
  - Arithmetic
  - Assignment
  - Comparison
  - Logical
  - Bitwise (Intro)
  - Ternary
- Real-world use cases

---

## ⚙️ What Are Operators?

> Operators are **symbols** used to **perform operations** on variables and values.  
They help us compute results, compare values, assign variables, and make decisions.

Example:

```js
let a = 10 + 5; // '+' is an operator
console.log(a); // 15
```

---

## ➕ Arithmetic Operators

Used to perform basic mathematical operations.

| Operator | Description         | Example (`a = 10, b = 3`) | Result |
| -------- | ------------------- | ------------------------- | ------ |
| `+`      | Addition            | `a + b`                   | `13`   |
| `-`      | Subtraction         | `a - b`                   | `7`    |
| `*`      | Multiplication      | `a * b`                   | `30`   |
| `/`      | Division            | `a / b`                   | `3.33` |
| `%`      | Modulus (Remainder) | `a % b`                   | `1`    |
| `**`     | Exponentiation      | `a ** 2`                  | `100`  |
| `++`     | Increment           | `a++`                     | `11`   |
| `--`     | Decrement           | `b--`                     | `2`    |

---

## 📝 Assignment Operators

Assign values to variables.

```js
let x = 5;
x += 2; // x = x + 2 => 7
x *= 3; // x = x * 3 => 21
```

| Operator | Meaning             |
| -------- | ------------------- |
| `=`      | Assign              |
| `+=`     | Add and assign      |
| `-=`     | Subtract and assign |
| `*=`     | Multiply and assign |
| `/=`     | Divide and assign   |
| `%=`     | Modulus and assign  |

---

## ⚖️ Comparison Operators

Used to compare two values and return a **boolean** (`true/false`).

```js
let age = 18;
console.log(age >= 18); // true
```

| Operator | Description           |
| -------- | --------------------- |
| `==`     | Equal (loose)         |
| `===`    | Equal (strict type)   |
| `!=`     | Not equal (loose)     |
| `!==`    | Not equal (strict)    |
| `>`      | Greater than          |
| `<`      | Less than             |
| `>=`     | Greater than or equal |
| `<=`     | Less than or equal    |

---

## 🔗 Logical Operators

Used for decision making with **true/false** conditions.

```js
let hasInternet = true;
let hasLaptop = false;

console.log(hasInternet && hasLaptop); // false
```

| Operator | Name | Meaning   | Example  |
| -------- | ---- | --------- | -------- |
| `&&`     | AND  | Both conditions must be true    | `true && true` = `true`   |
| `\|\|`     | OR   | At least one condition must be true | `true \|\| false` = `true`  |
| `!`      | NOT  | Inverts the boolean value       | `!true` = `false`          |

---

## ❓ Ternary Operator (Shortcut for if-else)

```js
let score = 80;
let result = score >= 50 ? "Pass" : "Fail";
console.log(result); // "Pass"
```

---

## 🧠 Practice Tasks

### ✅ Task 1:

Check if a user is eligible to vote:

```js
let age = 16;
let canVote = age >= 18 ? "Eligible" : "Not Eligible";
```

### ✅ Task 2:

Calculate and log the square of a number using the exponent operator `**`.

---

## 💡 Interview Tip:

Always use `===` instead of `==` for comparisons, because `===` checks both **value** and **type**.

```js
console.log(5 == "5");   // true (not safe)
console.log(5 === "5");  // false ✅ (recommended)
```

---

## 🛑 Common Mistakes

* Using `==` instead of `===`
* Forgetting parentheses in logical conditions
* Misusing increment (`a++` vs `++a`) — they behave differently!

---

## 📚 Recommended Resources

* [MDN Web Docs: Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
* [W3Schools: JavaScript Operators](https://www.w3schools.com/js/js_operators.asp)
* [JavaScript.info – Operators](https://javascript.info/operators)

---

## 🔁 Recap

* JavaScript provides a wide variety of operators
* Use arithmetic for math, comparison for decision-making, and logical for flow control
* Mastering operators is **essential for writing real-world logic**

---

## ⏭️ Next Day: [Day 4 → Conditional Statements](./day04.md)

---

> 💬 Have questions? Drop them in [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 Want to contribute or fix something? [Open a Pull Request](https://github.com/ajay-dhangar/200-days-of-javascript/pulls)