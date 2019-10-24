# Getting started with Javascript

To learn more about media queries, read the following articles:

- [W3Schools - Javascript](https://www.w3schools.com/js/)
- [The modern Javascript tutorial](https://javascript.info/)
- [You don't know Javascript](https://github.com/getify/You-Dont-Know-JS)

We will cover the following topics:

### Integrating javascript code in HTML pages

**Inline**

```html
<script>
  console.log("Hello World!");
</script>
```

**External**

```html
<script src="./external-javascript-file.js" />
```

### Output options

- `document.write`
- `alert`
- `console.log`

### Variable declarations

- `var`
- `let`
- `const`

### Data types

- `Integer`
- `Float`
- `String`
- `Boolean`
- `Object`
- `Array`
- `undefined`
- `null`

### Operators

- Arithmetic (`+`, `-`, `*`, `/`, `%`, `++`, `--`)
- Assignment (`=`, `+=`, `-=`, `*=`, `/=`, `%=`)
- String operators (`+`, `+=`)
- Comparison operators (`==`, `===`, `!=`, `!==`, `<`, `<=`, `>`, `>=`)
- Logical operators (`&&`, `||`, `!`)
- Type operators (`typeof`, `instanceof`)

### Functions

**Using the `function` keyword**

```js
function add(a, b) {
  return a + b;
}
```

**As variable declaration**

```js
const add = function(a, b) {
  return a + b;
};
```

**As arrow function**

```js
const add = (a, b) => {
  return a + b;
};

// is the same as

const add = (a, b) => a + b;
```

### Conditional statements

```js
if (a > b) {
  console.log("a is greater than b.");
} else {
  console.log("b is greater than a.");
}
```

### Working with the Math class

- `Math.round()`
- `Math.ceil()`
- `Math.floor()`
- `Math.pow()`
- `Math.sqrt()`
- `Math.min()`
- `Math.max()`
- `Math.random()`

> **Let's code together**
> Let's write a recursive function that generates lotto numbers.

### Working with objects

- properties
- methods

> **Let's code together**
> Create a car object having properties like `name`, `model`, `color` and `speed`.
> Also it should have methods like: `start`, `accelerate`, `break`, `stop`.

# Homework

### Basic

1. Write a function that converts `meters` in `inches`.
2. Write a function that converts `celsius` in `fahrenheit`.

### Medium

Implement a function that writes to the console

- `Good morning` if the current time is less than 12 PM
- `Good afternoon` if the current is between 12 PM and 6 PM
- `Good evening` if the current time is more than 6PM

To get the current hour you can use `new Date().getHours()`.
