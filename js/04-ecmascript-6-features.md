# ES6 features

### Variable declaration

- Variables declared with `var` are function scoped, can be redeclared and reassigned.
- Variables declared with `let` are block scope, can not be redeclared, but can be reassigned.
- Variables declared with `const` are block scope, can not be redeclared, or reassigned.
- Variables declared with `let` or `const` are not hoisted.

```js
function varTest() {
  var x = 1;
  if (true) {
    var x = 2; // same variable!
    console.log(x); // 2
  }
  console.log(x); // 2
}
```

```js
function letTest() {
  let x = 1;
  if (true) {
    let x = 2; // different variable
    console.log(x); // 2
  }
  console.log(x); // 1
}
```

### Array functions

#### `forEach`

```js
[1, 2, 3, 4].forEach(number => {
  console.log(number);
});

// [1, 2, 3, 4]
```

#### `map`

```js
[1, 2, 3, 4].map(number => number * 2);

// [2, 4, 6, 8]
```

### `filter`

```js
[1, 2, 3, 4].filter(number => number % 2 === 0);

// [2, 4]
```

### `find`

```js
[1, 2, 3, 4].find(number => number % 2 === 0);

// 2
```

### Template literals

```js
const name = "Rex";
const age = 2;
const sentence = "My dog " + name + " is " + age * 7 + "years old.";
```

```js
const name = "Rex";
const age = 2;
const sentence = `My dog ${name} is ${age * 7} years old.`;
```

### Promises

To learn more about promises, follow these links:

- [Promises - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)
- [Promises - Javascript Info](https://javascript.info/promise-basics)

```js
const promise = new Promise((resolve, reject) => {
  resolve("Promise resolved. Cool!");
  //reject(Error('Promise rejected with an error. Not cool!'));
});

promise
  .then(data => {
    console.log(data);
  })
  .catch(error => {
    console.log(error);
  });
```

**Chaining promises**

```js
function double(number) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      if (number > 100) {
        reject("Number is too large.");
        return;
      }

      resolve(number * 2);
    }, 500);
  });
}

double(15)
  .then(result => {
    console.log(result);
    return double(result);
  })

  .then(result => {
    console.log(result);
    return double(result);
  })

  .then(result => {
    console.log(result);
    return double(result);
  })

  .catch(err => {
    console.error("Error", err);
  });
```

### Async/await

```js
function double(number) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      if (number > 100) {
        reject("Number is too large.");
        return;
      }

      resolve(number * 2);
    }, 500);
  });
}

async function doubleTreeTimes() {
  const result1 = await double(15);
  console.log(result1);
  const result2 = await double(result1);
  console.log(result2);
  const result3 = await double(result2);
  console.log(result3);
  const result4 = await double(result3);
  console.log(result4);
}

doubleTreeTimes().catch(error => {
  console.log(error);
});
```

### Classes

To learn more about classes follow these links:

- [Classes - W3Schools](https://www.w3schools.com/js/js_classes.asp)
- [Classes - Javascript Info](https://javascript.info/class)

### Creating classes

```js
class Dog {
  constructor(name, breed) {
    this.name = name;
    this.breed = breed;
  }

  bark() {
    console.log(`Bark Bark! My name is ${this.name}`);
  }

  static info() {
    console.log("A dog is better than a cat.");
  }
}

const snickers = new Dog("Snickers", "King Charles");
const sunny = new Dog("Sunny", "German Shepherd");

snickers.bark();
sunny.bark();
Dog.info();
```

### Extending classes

```js
class Animal {
  constructor(name) {
    this.name = name;
    this.thirst = 100;
    this.belly = [];
  }

  drink() {
    this.thirst = this.thirst - 10;
    return this.thirst;
  }

  eat(food) {
    this.belly.push(food);
    return this.belly;
  }
}

const elephant = new Animal("Dumbo");
elephant.drink();
elephant.eat();

class Dog extends Animal {
  constructor(name, breed) {
    super(name);
    this.name = name;
    this.breed = breed;
  }

  bark() {
    console.log(`Bark Bark! My name is ${this.name}`);
  }
}

const snickers = new Dog("Snickers", "German shepherd");

snickers.eat();
snickers.drink();
snickers.bark();
```

 >
 > **Let's code together**
 >
 > Implement a `Person` class with the following properties: `name`, `gender`, and the methods: `wakeUp`, `eat`, `work`, `sleep`.
 >
 > Then implement a `Student` class that extends `Person` but also has the properties: `year`, `university`, `courses[]` and the method `learn`.
 > Also implement a `Teacher` class that extends `Person` with the properties: `yearsOfExperience`, `university`, `courses` and the method `teach`.
 > Create multiple students and techers using the classes implemented.