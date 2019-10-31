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

# Working with arrays

To learn more about arrays:

- [Arrays - W3Schools](https://www.w3schools.com/js/js_arrays.asp)
- [Array methods - W3Schools](https://www.w3schools.com/js/js_array_methods.asp)

### Creating arrays

```js
var numbers = [1, 2, 3];
```

### Listing elements in an array

```js
var numbers = [1, 2, 3];
for (var i = 0; i < numbers.length; i++) {
  console.log(numbers[i]);
}
```

or

```js
var numbers = [1, 2, 3];
numbers.forEach(number => console.log(number));
```

### Adding items into an array

```js
var numbers = [1, 2, 3];
numbers.push(4); // adds 4 at the end of the array
numbers.unshift(0); // adds 0 to the beginning of the array
console.log(numbers);
```

### Changing an item in an array

```js
var numbers = [1, 2, 3];
numbers[1] = "Two"; // Changes 2 to 'Two'
console.log(numbers);
```

### Removing items from an array

```js
var numbers = [1, 2, 3];
numbers.splice(2, 1); // removes 1 item starting from position 2
console.log(numbers);
```

### Sorting items

```js
var numbers = [4, 5, 2, 3, 1];
numbers.sort();
console.log(numbers);
```

### Filtering arrays

```js
var numbers = [-1, 2, 9, -5, 3];
var positionNumbers = numbers.filter(number => number > 0);
console.log(positionNumbers);
```

### Mapping arrays

```js
var numbers = [-1, 2, 9, -5, 3];
var doubledNumbers = numbers.map(number => number * 2);
console.log(doubledNumbers);
```

> **Let's code together**
> Write a function that takes a list of names, and returns another list only with the names having more than 4 characters.
> Write a function that generates 6 lotto numbers, but it makes sure there are no duplicates.

# Homework

### Basic challenge

Write a function that takes as an arguments an array of numbers and returns the sum of the positive numbers.

**For example:**
For the array `[-2, 10, 2, 4, -6, 3]` it must return `10 + 2 + 4 + 3` which is `19`.

### Medium challenge

Write a function that generates a random name by combining `firstNames` and `lastNames` randomly.
Start from two hardcoded arrays `var firstNames = ['John', 'Matthew', 'Thomas', 'Christian', 'David']` and `var lastNames = ['Smith', 'Pitt', 'Cruise', 'Robinson']`. The function should generate a single random name like `John Cruise`, `Thomas Smith`, `David Pitt`, `Christian Smith`, etc.
