---
title: "Day 07: Booleans, Truthy/Falsy & Comparison Operators"
tags: [javascript, booleans, comparison, truthy-falsy, beginner]
level: beginner
day: 07
author: Ajay Dhangar
---

# 📅 Day 07: Booleans, Truthy/Falsy & Comparison Operators

> 🎯 **Goal**: Learn how JavaScript handles true/false logic, what values are considered truthy/falsy, and how to compare different values using operators.

---

## 📌 What You'll Learn

* What Booleans are
* Truthy and Falsy values in JavaScript
* All comparison operators and how they work
* Real-world use in conditions and logic

---

## 📖 Introduction

In JavaScript, decision-making is handled through **Booleans** — values that are either `true` or `false`. You use Booleans to control the flow of your programs — for example, deciding whether a user can access a feature or whether a value meets certain criteria.

To evaluate these decisions, JavaScript uses **comparison operators** and relies on the concept of **truthy** and **falsy** values.

---

## ⚙️ Syntax / Examples

### Boolean Basics

```js
let isOnline = true;
let hasPaid = false;

console.log(isOnline); // true
console.log(typeof isOnline); // boolean
```

---

### 🧠 Truthy vs Falsy

In JavaScript, **truthy** values behave like `true`, and **falsy** values behave like `false` in a Boolean context (like `if` statements).

| Falsy Values        |
| ------------------- |
| `false`             |
| `0`                 |
| `-0`                |
| `""` (empty string) |
| `null`              |
| `undefined`         |
| `NaN`               |

Everything else is **truthy**, including:

* `"hello"` (non-empty string)
* `[]` (empty array)
* `{}` (empty object)
* `42`, `-1` (any non-zero number)

```js
if ("hello") {
  console.log("This is truthy!");
}

if (0) {
  console.log("This will NOT run.");
}
```

---

### 🔗 Comparison Operators

```js
console.log(10 > 5);   // true
console.log(3 < 2);    // false
console.log(5 == '5'); // true (loose equality)
console.log(5 === '5'); // false (strict equality)
console.log(10 != 5);  // true
console.log(10 !== '10'); // true
console.log(4 >= 4);   // true
console.log(8 <= 7);   // false
```

---

## 🔍 Deep Dive

### 🔄 `==` vs `===`

| Operator | Description                             | Example              |
| -------- | --------------------------------------- | -------------------- |
| `==`     | Loose equality (compares value only)    | `5 == '5' → true`    |
| `===`    | Strict equality (compares value & type) | `5 === '5' → false`  |
| `!=`     | Loose inequality                        | `10 != '10' → false` |
| `!==`    | Strict inequality                       | `10 !== '10' → true` |

### 🎯 Real-life Example

```js
const userAge = 18;

if (userAge >= 18) {
  console.log("You are eligible to vote.");
} else {
  console.log("You are too young.");
}
```

---

## 🧪 Practice Tasks

### ✅ Task 1:

Write a function that checks if a number is positive.

```js
function isPositive(num) {
  return num > 0;
}

console.log(isPositive(5));  // true
console.log(isPositive(-3)); // false
```

### ✅ Task 2:

Check if an input field is empty.

```js
const input = "";

if (!input) {
  console.log("Input is empty (falsy).");
}
```

---

## ❗ Common Mistakes

* Confusing `==` with `===` — prefer `===` to avoid bugs.
* Not knowing which values are falsy — leads to incorrect condition handling.
* Assuming `[]` or `{}` are falsy — they are **truthy** in JavaScript.

---

## 💡 Interview Tips

* Explain the difference between `==` and `===` with examples.
* Know and list all falsy values — this is a common rapid-fire question.
* Real-world: form validations, login checks, toggle logic.

---

## 📚 Additional Resources

* [MDN - Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)
* [MDN - Comparison Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Comparison_Operators)
* [JavaScript.info - Comparisons](https://javascript.info/comparison)

---

## 🔁 Recap

* Booleans represent `true` or `false`
* Learn which values are truthy or falsy
* Use `===` for safer comparisons

---

## ⏭️ Next Day: [Day 08 → Logical Operators (`&&`, `||`, `!`)](./day08.md)

---

> 💬 Have doubts? Ask in [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 Found a mistake? [Raise a Pull Request](https://github.com/ajay-dhangar/200-days-of-javascript/pulls)