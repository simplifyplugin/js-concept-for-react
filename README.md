# js-concept-for-react

Here’s the Markdown file content for your JavaScript concepts:

```markdown
# Arrow Functions In JavaScript

Arrow functions provide a more concise syntax for writing functions. Unlike regular functions, arrow functions do not have their own `this`, making them particularly useful in situations where preserving the context of `this` is important.

**Example:**
```javascript
const add = (a, b) => a + b;
console.log(add(2, 3)); // 5
```

# Template Literals In JavaScript

Template literals allow for embedded expressions and multi-line strings, making it easier to work with dynamic content.

**Example:**
```javascript
const name = "John";
const greeting = `Hello, ${name}!`;
console.log(greeting); // Hello, John!
```

# Ternary Operator In JavaScript

The ternary operator is a concise way to write an `if-else` statement. It takes three operands: a condition, an expression to execute if the condition is true, and an expression to execute if the condition is false.

**Example:**
```javascript
const age = 18;
const canVote = age >= 18 ? "Yes" : "No";
console.log(canVote); // Yes
```

# Objects In JavaScript

Objects in JavaScript are collections of key-value pairs, where keys are strings (or Symbols) and values can be any type of data, including other objects or functions.

**Example:**
```javascript
const person = {
  name: "Alice",
  age: 25,
  greet() {
    console.log(`Hello, my name is ${this.name}`);
  }
};
person.greet(); // Hello, my name is Alice
```

# Objects Destructuring

Object destructuring allows you to extract properties from objects and assign them to variables in a concise way.

**Example:**
```javascript
const person = { name: "Alice", age: 25 };
const { name, age } = person;
console.log(name); // Alice
console.log(age);  // 25
```

# Spread Operator In JavaScript

The spread operator (`...`) allows an iterable, such as an array, to be expanded in places where zero or more arguments or elements are expected.

**Example:**
```javascript
const numbers = [1, 2, 3];
const newNumbers = [...numbers, 4, 5];
console.log(newNumbers); // [1, 2, 3, 4, 5]
```

# Map In JavaScript

The `map` method creates a new array populated with the results of calling a provided function on every element in the calling array.

**Example:**
```javascript
const numbers = [1, 2, 3];
const doubled = numbers.map(num => num * 2);
console.log(doubled); // [2, 4, 6]
```

# Filter In JavaScript

The `filter` method creates a new array with all elements that pass the test implemented by the provided function.

**Example:**
```javascript
const numbers = [1, 2, 3, 4];
const evens = numbers.filter(num => num % 2 === 0);
console.log(evens); // [2, 4]
```

# Filter Method E-Commerce Example

Filtering a product list based on specific criteria, such as price.

**Example:**
```javascript
const products = [
  { name: "Laptop", price: 1000 },
  { name: "Phone", price: 500 },
  { name: "Tablet", price: 750 }
];
const affordable = products.filter(product => product.price < 800);
console.log(affordable); // [{ name: "Phone", price: 500 }, { name: "Tablet", price: 750 }]
```

# Reduce In JavaScript

The `reduce` method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.

**Example:**
```javascript
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((acc, curr) => acc + curr, 0);
console.log(sum); // 10
```

# Async/Await Syntax

`async/await` is a modern way to work with asynchronous code in JavaScript. It makes asynchronous code look and behave more like synchronous code.

**Example:**
```javascript
const fetchData = async () => {
  const response = await fetch('https://api.example.com/data');
  const data = await response.json();
  console.log(data);
};
fetchData();
```

# Import / Export syntax ES6

The `import` and `export` statements in ES6 allow you to modularize your code by exporting and importing variables, functions, and classes from different files.

**Example:**
```javascript
// In math.js
export const add = (a, b) => a + b;

// In main.js
import { add } from './math';
console.log(add(2, 3)); // 5
```
