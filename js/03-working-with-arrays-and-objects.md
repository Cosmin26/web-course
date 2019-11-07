# Arrays

To learn more about these topics visit the following links:

- [JS Arrays - W3Schools](https://www.w3schools.com/js/js_arrays.asp)
- [JS Arrays - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

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
> 1. Write a function that takes a list of names, and returns another list only with the names having more than 4 characters.
>
> 2. Write a function that generates 6 lotto numbers, but it makes sure there are no duplicates.

# Objects

To learn more about this topics visit the following links:

- [JS Objects loop - W3Schools](https://www.w3schools.com/js/js_objects.asp)
- [JS Objects - MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

### Defininf object properties

```js
var car = {
  type: "Fiat",
  model: "500",
  color: "white"
};
```

### Accessing object properties

```js
console.log(car.type);
console.log(car["type"]);
```

### Object methods

```js
var person = {
  firstName: "John",
  lastName: "Doe",
  age: 23,
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
};
```

### Accessing object methods

```js
console.log(person.fullName());
```

> **Let's code together**
> Implement a car object with the following properties: type, model, color, isEngineStarted, distance, startEngine, stopEngine, travel.

# Homework

### Basic challenge - Arrays

Write a function that takes as an arguments an array of numbers and returns the sum of the positive numbers.

**For example:**
For the array `[-2, 10, 2, 4, -6, 3]` it must return `10 + 2 + 4 + 3` which is `19`.

### Basic challenge - Objects

Implement an `animal` object with the following properties: `type` (e.g. `Dog`), `name` (e.g. `Rex`), `gut` (an array of items that the animal ate, e.g. `['Bones', 'Meat']`), and the following method: `eat(food)` which adds the food the animals `gut`.

### Medium challenge

Write a function that generates a random name by combining `firstNames` and `lastNames` randomly.
Start from two hardcoded arrays `var firstNames = ['John', 'Matthew', 'Thomas', 'Christian', 'David']` and `var lastNames = ['Smith', 'Pitt', 'Cruise', 'Robinson']`. The function should generate a single random name like `John Cruise`, `Thomas Smith`, `David Pitt`, `Christian Smith`, etc.
