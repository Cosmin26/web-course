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
> Write a function that lists all elements from an array
>
> Write a function that adds up all elements from an array
>
> Write a function that finds the lowest element from an array of numbers.
>
> Write a function that accepts an array as an argument, and returns two arrays: one with the odd numbers, and one with the even numbers.
>
> Write a function that accepts a number and returns `true` if the number is a prime number, otherwise it returns `false`.

# Homework

### Basic challenge

Implement a for loop that writes to the console every third number between 0 and 100.
It will write to the console: `3`, `6`, `9`, `12`, ..., `93`, `96`, `99`.

### Medium challenge

Implement a function that accepts two numbers as arguments: `a` and `b` and return the sum of numbers between `a` and `b`.
For example if we call the function with `a=6` and `b=9` it will return `30` (which is `6+7+8+9`).

### Bonus challanges (optional)
These are some harder challenges. 

#### Rolling a dice
Write a function that will roll a dice (randomly generate numbers between 1 and 6) and then will count separately how many times we had 1, 2, 3, 4, 5, 6.

Use a `for` to roll the dice 10 times, 100 times, 1000 times and even 1000000 times.
The theory of big numbers says that if we roll the dice enough time the count of how many times we had 1, 2, 3, etc. will be very similar.

#### Rock paper scrissor
You surely know this game. Implement a function that gets a single argument which is a string: either `rock`, or `paper`, or `scrissor`. This argument will represent what the user had chosen. Then the function will randomly generate `rock`, `paper` or `scrissor`. The randomly generated value will represent what the program had chosen. 

As a final step the function will write the the console the winner of the game, either the user or the program, possibly none of them if they chose the same things. In this case write `No-one won. Even!`

**Note** If you are a Big-Bang theory fan and you are in the mood, implement: `Rock, Paper, Scrissor, Lizard, Spock`. Here is how it works: https://www.youtube.com/watch?v=x5Q6-wMx-K8

#### Find the first N prime numbers
Write a function that gets a single argument `n`, and writes to the console the first `n` prime numbers. 
For example: for `n=5` it will write the first 5 prime numbers to the console: `1, 2, 3, 5, 7`.
