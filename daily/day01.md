---
title: "Day 1: Introduction to JavaScript 🔰"
tags: [javascript, introduction, basics, beginner]
level: beginner
day: 1
author: Ajay Dhangar
---

# 📅 Day 1: Introduction to JavaScript

Welcome to **Day 1** of your **200 Days of JavaScript** journey! Today is all about laying a solid foundation by understanding what JavaScript is and how to start using it.

---

> JavaScript is the language of the web that brings life to websites.

## 📌 What You'll Learn Today

* What JavaScript is and why it's important
* How it works in the browser
* Writing your first JavaScript code
* The different ways to include JavaScript in a webpage
* Declaring variables using `var`, `let`, and `const`

---

## 🧠 What is JavaScript?

JavaScript is a popular programming language used to make websites interactive, dynamic, and user-friendly.

In simple terms:

> Just like HTML is used to structure a webpage, and CSS is used to style it, JavaScript is used to bring it to life — by adding features like sliders, popups, forms, animations, live updates, and more.


## For Example

Imagine visiting a website that only has text and images — like a newspaper. It's static and non-interactive. Now, think of your favorite apps like Zomato, Paytm, or Flipkart — where you can click buttons, see animations, type in search boxes, or get real-time updates.

All of this magic is possible because of JavaScript (JS).

### 🛠️ Uses of JavaScript:
* Manipulating HTML/CSS (DOM)
* Fetching APIs and handling data
* Form validation
* Creating animations
* Building full-stack apps (with Node.js)

---

## 🚀 Getting Started

You don’t need to install anything to start! Open your browser and right-click → **Inspect → Console**.

Try this:

```js
console.log("Welcome to Day 1 of JavaScript!");
````

---

## 🖼️ Embedding JavaScript in HTML

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First JS Program</title>
  </head>
  <body>
    <h1>Hello World!</h1>
    <script>
      console.log("JavaScript is running!");
    </script>
  </body>
</html>
```

✅ This shows how JS can be directly included inside `<script>` tags.

---

## 🧾 Variables in JavaScript

Variables are used to **store data** in memory. You can declare them using:

| Keyword | Scope    | Reassignment | Hoisting | Use Case                     |
| ------- | -------- | ------------ | -------- | ---------------------------- |
| `var`   | Function | ✅ Yes        | ✅ Yes    | Legacy code                  |
| `let`   | Block    | ✅ Yes        | ❌ No     | Most common                  |
| `const` | Block    | ❌ No         | ❌ No     | Constants (unchanged values) |

### Example:

```js
var name = "Ajay";
let age = 25;
const language = "JavaScript";

console.log(name, age, language);
```

---

## 🧪 Practice Task

### ✅ Task: Declare and log user details

```js
// Task
let firstName = "John";
let lastName = "Doe";
let isStudent = true;

console.log("Name:", firstName + " " + lastName);
console.log("Is Student?", isStudent);
```

🔍 Try changing the values, combine them into a sentence, and log them!

---

## 🧠 Quiz of the Day

1. Which keyword should you use to declare a constant value?

   * a) var
   * b) let
   * c) const ✅
2. What does `console.log()` do?

   * a) Declares a variable
   * b) Logs output to the browser console ✅
   * c) Runs HTML

---

## 🧱 Today’s Summary

* JavaScript adds interactivity to web pages
* You can write JS in the browser or embed in HTML
* Use `let` and `const` for modern JavaScript
* Practice logging different types of data

---

## 📚 Recommended Resources

* 📘 [JavaScript Guide – MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
* 📘 [W3Schools JS Introduction](https://www.w3schools.com/js/js_intro.asp)
* 📘 [JavaScript for Beginners (freeCodeCamp)](https://www.freecodecamp.org/news/javascript-beginners-handbook/)

---

## ⏭️ Next Day: [Day 2 → Variables & Data Types](./day02.md)

---

> 💬 **Join Discussions**: [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 **Found a mistake?** [Open an Issue](https://github.com/ajay-dhangar/200-days-of-javascript/issues/new)
