# Loops and iterations

To learn more about this topic visit the following links:

- [The For loop - W3Schools](https://www.w3schools.com/js/js_loop_for.asp)
- [The While loop - W3Schools](https://www.w3schools.com/js/js_loop_while.asp)
- [Loops and iterations - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

### The `for` loop

```js
var i;
for (i = 0; i < 10; i++) {
  console.log(i);
}
```

### The `while` loop

```js
var i = 0;
while (i < 10) {
  console.log(i);
  i--;
}
```

> **Let's code together**
> Write a function that finds the lowest element from an array of numbers.
> Write a function that accepts a number and returns `true` if the number is a prime number, otherwise it returns `false`.
> Write a function that lists the first `n` prime numbers.

# Homework

### Basic challenge

Implement a for loop that writes to the console every third number between 0 and 100.
It will write to the console: `3`, `6`, `9`, `12`, ..., `93`, `96`, `99`.

### Medium challenge

Implement a function that accepts two numbers as arguments: `a` and `b` and return the sum of numbers between `a` and `b`.
For example if we call the function with `a=6` and `b=9` it will return `30` (which is `6+7+8+9`).
