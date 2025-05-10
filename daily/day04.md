---
title: "Day 04: Strings & String Methods (length, slice, replace, etc.)"
tags: [javascript, strings, string-methods]
level: beginner
day: 04
author: ajay-dhangar
---

# 📅 Day 04: [Strings & String Methods (length, slice, replace, etc.)]

> 🎯 **Goal**: By the end of this day, you'll understand how to work with strings in JavaScript and use various string methods like `length`, `slice()`, `replace()`, and more.

---

## 📌 What You'll Learn

* How to use the `length` property to get the length of a string.
* How to extract substrings using the `slice()` method.
* How to replace parts of a string using `replace()`.
* How to manipulate case with methods like `toUpperCase()` and `toLowerCase()`.
* Common mistakes to avoid when working with strings.

---

## 📖 Introduction

Strings are one of the most commonly used data types in JavaScript. A string is a sequence of characters used to represent text. JavaScript provides several built-in methods to manipulate strings efficiently. In this lesson, we will explore some of the essential string methods that will help you work with strings in your code.

For example, you might need to extract a portion of a text or change the case of the text in real-world applications, like handling user inputs or manipulating messages.

---

## ⚙️ Syntax / Examples

Here are some of the most commonly used string methods:

### `length` Property

The `length` property returns the number of characters in a string. It is a read-only property.

```js
const text = "Hello, World!";
console.log(text.length); // Output: 13
```

### `slice(start, end)`

The `slice()` method extracts a section of a string and returns it as a new string. The `start` parameter is the index at which to begin extraction, and the `end` parameter is the index at which to end extraction (not included). If `end` is omitted, it extracts to the end of the string.

```js
const text = "JavaScript is awesome!";
console.log(text.slice(0, 10)); // Output: "JavaScript"
```

### `replace(searchValue, newValue)`

The `replace()` method searches for a specified value in a string and replaces it with a new value. The first argument can be a string or a regular expression.

```js
const text = "I love JavaScript!";
const newText = text.replace("love", "enjoy");
console.log(newText); // Output: "I enjoy JavaScript!"
```

### `toUpperCase()` and `toLowerCase()`

The `toUpperCase()` method converts a string to uppercase letters, while `toLowerCase()` converts it to lowercase letters.

```js
const text = "JavaScript";
console.log(text.toUpperCase()); // Output: "JAVASCRIPT"
console.log(text.toLowerCase()); // Output: "javascript"
```

### `trim()`

The `trim()` method removes whitespace from both ends of a string. This is useful for cleaning up user input.

```js
const text = "   Hello, World!   ";
console.log(text.trim()); // Output: "Hello, World!"
```

---

## 🔍 Deep Dive (If applicable)

### String Immutability

Strings in JavaScript are **immutable**, which means once a string is created, it cannot be modified. If you try to change a string's character, you won't see any effect.

**For example:**

```js
let str = "Hello";
str[0] = "h";  // This will not change the string, it remains "Hello"
console.log(str);  // Output: "Hello"
```

To modify strings, you'll need to create a new string with the desired changes. 

**For example:**

```js
let str = "Hello";
str = "h" + str.slice(1);  // Create a new string
console.log(str);  // Output: "hello"
```

### String Methods and Regular Expressions

The `replace()` method can also accept a regular expression as the first argument. This allows for more complex search patterns.

```js
const text = "I love JavaScript! JavaScript is awesome!";
const newText = text.replace(/JavaScript/g, "JS");
console.log(newText); // Output: "I love JS! JS is awesome!"
```

### String Interpolation

String interpolation allows you to embed expressions inside string literals. This is often done using template literals (backticks).

```js
const name = "Ajay Dhangar";
const age = 25;
const greeting = `Hello, my name is ${name} and I am ${age} years old.`;
console.log(greeting); // Output: "Hello, my name is Ajay Dhangar and I am 25 years old."
```

---

## 🧪 Practice Tasks

### ✅ Task 1:

Write a function that takes a string as an argument and returns a substring containing the first 5 characters of the string.

```js
function getFirstFiveChars(str) {
  return str.slice(0, 5);
}
console.log(getFirstFiveChars("JavaScript")); // Output: "JavaS"
```

### ✅ Task 2:

Write a function that takes a string and replaces all occurrences of "JavaScript" with "JS".

```js
function replaceJavaScript(str) {
  return str.replace(/JavaScript/g, "JS");
}
console.log(replaceJavaScript("I love JavaScript! JavaScript is awesome!")); 
// Output: "I love JS! JS is awesome!"
```

---

## ❗ Common Mistakes

* **Mistake 1**: Forgetting to handle the case of the string when replacing text.

  * **Wrong**: Using `replace("love", "enjoy")` without considering case.
  * **Correct**: Use a case-insensitive regular expression: `replace(/love/i, "enjoy")`.
* **Mistake 2**: Confusing `slice()` and `substring()`.

  * `slice()` allows negative indices, which count from the end of the string. `substring()` does not support negative indices.
  * Example: `slice(-5)` returns the last 5 characters, but `substring(-5)` returns the full string.

---

## 💡 Interview Tips

* In interviews, you may be asked to reverse a string or manipulate the text in various ways. Always use the most efficient string methods.
* One common question is how to check if a string contains a substring, and `includes()` is often the best way to do so.

---

## 📚 Additional Resources

* [MDN Reference: String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)
* [W3Schools: JavaScript String Methods](https://www.w3schools.com/js/js_string_methods.asp)
* [JavaScript.info: String Basics](https://javascript.info/string)

---

## 🔁 Recap

* Strings are sequences of characters, and JavaScript provides various methods to manipulate them.
* Key string methods include `length`, `slice()`, `replace()`, `toUpperCase()`, `toLowerCase()`, and `trim()`.
* Strings are immutable, meaning any changes create a new string.

---

## ⏭️ Next Day: [Day 05 → Arrays](./day05.md)

---

> 💬 Have doubts? Ask in [GitHub Discussions](https://github.com/ajay-dhangar/200-days-of-javascript/discussions)
> 🛠 Found a mistake? [Raise a Pull Request](https://github.com/ajay-dhangar/200-days-of-javascript/pulls)
