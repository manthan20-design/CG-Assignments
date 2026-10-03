# Part I: Variables (let, var, const)

## Part A — 4 Questions

### 1. Personal Information

```javascript
let name = "Manthan";
let age = 17;
let city = "Gandhinagar";

console.log(name);
console.log(age);
console.log(city);
```

### 2. Change the Score

```javascript
let score = 50;
score = 80;

console.log(score);
```

### 3. Constant Value

```javascript
const PI = 3.14;

console.log(PI);
```

### 4. Uninitialized Variables

```javascript
var num1;
let num2;

console.log(num1);
console.log(num2);

num1 = 10;
num2 = 20;

console.log(num1);
console.log(num2);
```

---

## Part B — 4 Questions

### 5. Choose the Correct Keyword

```javascript
const studentName = "Manthan";
let marks = 75;
const schoolName = "ABC School";

marks = 90;

console.log(studentName);
console.log(marks);
console.log(schoolName);
```

### 6. Understand Scope

```javascript
if (true) {
    var a = 10;
    let b = 20;
    const c = 30;
}

console.log(a);
console.log(b);
console.log(c);
```

**Observation:**
`var` can be accessed outside the block, but `let` and `const` cannot be accessed outside the block.

### 7. Test Re-declaration

```javascript
var user = "Manthan";
var user = "Rahul";

console.log(user);
```

**Output:**

```text
Rahul
```

Using `let`:

```javascript
let user = "Manthan";
let user = "Rahul";
```

**Observation:**
`var` allows re-declaration, while `let` does not allow re-declaration in the same scope.

### 8. Test Re-assignment

```javascript
var a = 10;
let b = 20;
const c = 30;

a = 100;
b = 200;
c = 300;

console.log(a);
console.log(b);
console.log(c);
```

**Observation:**
`var` and `let` allow re-assignment, but `const` does not allow re-assignment and produces an error.

---

## Part C — 2 Questions

### 9. Predict and Explain

```javascript
var x = 10;

if (true) {
    var x = 20;
    let y = 30;
    const z = 40;
}

console.log(x);
console.log(y);
console.log(z);
```

**Output:**

```text
20
ReferenceError
ReferenceError
```

**Explanation:**
`x` is declared using `var`, so it can be accessed outside the `if` block. Its value becomes `20`.

`y` is declared using `let`, so it is limited to the `if` block.

`z` is declared using `const`, so it is also limited to the `if` block.

Therefore, `console.log(y)` and `console.log(z)` produce `ReferenceError`.

---

### 10. Fix the Program

```javascript
const name = "Manthan";

let age = 20;
age = 25;

if (true) {
    var city = "Delhi";
    let country = "India";
    console.log(country);
}

console.log(city);

let score = 50;
score = 80;

console.log(name);
console.log(age);
console.log(score);
```

# JavaScript Assignment Answers

## 1. Predict the Hoisting Behavior

```javascript
console.log(a);
console.log(b);
console.log(c);

var a = 10;
let b = 20;
const c = 30;
```

**Answer:**

* `console.log(a)` prints `undefined` because `var` declarations are hoisted and initialized with `undefined`.
* `console.log(b)` causes a `ReferenceError` because `let` is in the Temporal Dead Zone (TDZ) before declaration.
* `console.log(c)` causes a `ReferenceError` because `const` is also in the TDZ before declaration.

The first error stops normal execution, so the remaining statements do not execute.

## 2. Fix the Hoisting Errors

```javascript
var x = "Hello";
let y = "World";
const z = "!";

console.log(x);
console.log(y);
console.log(z);

console.log(x + " " + y + z);
```

**Output:**

```text
Hello
World
!
Hello World!
```

# Part E — Basic Identification

## 1. Classify the Types

```javascript
let wholeNumber = 10;
let decimalNumber = 10.5;
let text = "Hello World";
let isActive = true;

console.log(wholeNumber, typeof wholeNumber);
console.log(decimalNumber, typeof decimalNumber);
console.log(text, typeof text);
console.log(isActive, typeof isActive);
```

**Output:**

```text
10 number
10.5 number
Hello World string
true boolean
```

## 2. Undefined vs Null

```javascript
let a;
let b = null;

console.log(a, typeof a);
console.log(b, typeof b);
```

**Output:**

```text
undefined undefined
null object
```

**Explanation:** `undefined` means a variable has been declared but has not been assigned a value. `null` represents an intentional empty value. JavaScript returns `"object"` for `typeof null` due to a historical language quirk.

## 3. Number Special Values

```javascript
let positiveInfinity = Infinity;
let negativeInfinity = -Infinity;
let notANumber = NaN;
let scientificNumber = 2.5e3;
let largeNumber = 1_000_000;

console.log(positiveInfinity, typeof positiveInfinity);
console.log(negativeInfinity, typeof negativeInfinity);
console.log(notANumber, typeof notANumber);
console.log(scientificNumber, typeof scientificNumber);
console.log(largeNumber, typeof largeNumber);
```

**Output:**

```text
Infinity number
-Infinity number
NaN number
2500 number
1000000 number
```

## 4. String Styles

```javascript
let singleQuote = 'Hello World';
let doubleQuote = "JavaScript";
let name = "Manthan";
let templateString = `Hello, ${name}!`;

console.log(singleQuote);
console.log(doubleQuote);
console.log(templateString);
```

**Output:**

```text
Hello World
JavaScript
Hello, Manthan!
```

# Part F — Advanced Primitive Types

## 5. Symbol Uniqueness

```javascript
let symbol1 = Symbol("id");
let symbol2 = Symbol("id");

console.log(symbol1 === symbol2);

let student = {
    [symbol1]: "First ID",
    [symbol2]: "Second ID"
};

console.log(student[symbol1]);
console.log(student[symbol2]);
```

**Output:**

```text
false
First ID
Second ID
```

**Explanation:** Each call to `Symbol()` creates a unique value, even when both symbols have the same description.

## 6. BigInt Precision

```javascript
let regularNumber = 9007199254740991;

console.log(regularNumber + 1);
console.log(regularNumber + 2);
console.log(regularNumber + 3);

let bigNumber = 9007199254740991n;

console.log(bigNumber + 1n);
console.log(bigNumber + 2n);
console.log(bigNumber + 3n);
```

**Output:**

```text
9007199254740992
9007199254740992
9007199254740994
9007199254740992n
9007199254740993n
9007199254740994n
```

**Explanation:** JavaScript's `Number` type cannot represent every integer exactly beyond `Number.MAX_SAFE_INTEGER`. `BigInt` allows exact integer arithmetic for much larger integers.

## 7. Choose the Correct Type

**a) A unique identifier**

```javascript
let id = Symbol("uniqueId");
```

**b) A very large integer with exact precision**

```javascript
let bigNumber = 12345678901234567890n;
```

**c) A declared variable without a value**

```javascript
let value;
```

**d) An intentional empty value**

```javascript
let emptyValue = null;
```

# Part G — Prediction & Fixing

## 8. Predict the Output

```javascript
let a;
let b = null;
let c = 42;
let d = "Hello";
let e = true;
let f = Symbol("key");
let g = 123n;

console.log(typeof a, a);
console.log(typeof b, b);
console.log(typeof c, c);
console.log(typeof d, d);
console.log(typeof e, e);
console.log(typeof f, f);
console.log(typeof g, g);
```

**Output:**

```text
undefined undefined
object null
number 42
string Hello
boolean true
symbol Symbol(key)
bigint 123n
```

**Explanation:** The `typeof` operator identifies the type of each value. `typeof null` returns `"object"` because of a historical JavaScript quirk.

## 9. Fix the Code

```javascript
let num = 10;
let text = "Hello";
let flag = true;
let empty;
let nothing = null;
let unique = Symbol("id");
let big = 9007199254740991n;

console.log(num, text, flag, empty, nothing, unique, big);
```

**Output:**

```text
10 Hello true undefined null Symbol(id) 9007199254740991n
```

## 10. Primitive vs Non-Primitive

**a) What is the main difference between Primitive and Non-Primitive data types?**

Primitive types represent individual values, while non-primitive types represent collections of values or more complex structures.

Example:

```javascript
let age = 18;
let student = { name: "Riya", age: 18 };
```

**b) Why are Numbers, Strings, Booleans, Undefined, Null, Symbol, and BigInt called Primitive?**

They are called primitive types because they represent individual values and are not objects.

Example:

```javascript
let number = 10;
let text = "Hello";
let active = true;
```

**c) Give one example of a Non-Primitive data type.**

An object is a non-primitive type because it groups related properties and values.

```javascript
let student = {
    name: "Riya",
    age: 18
};
```

# Part H — Non-Primitive Data Types: Basic Creation & Usage

## 1. Create an Object

```javascript
let student = {
    name: "Riya",
    age: 18,
    isEnrolled: true
};

console.log(student);
console.log(student.name);
console.log(student.age);
console.log(student.isEnrolled);
```

**Output:**

```text
{ name: 'Riya', age: 18, isEnrolled: true }
Riya
18
true
```

## 2. Work with Arrays

```javascript
let scores = [85, 92, 78, 90];
let mixedData = [25, "Hello", true, null];

console.log(scores);
console.log(mixedData);
console.log(scores[0]);
console.log(scores[scores.length - 1]);
```

**Output:**

```text
[85, 92, 78, 90]
[25, 'Hello', true, null]
85
90
```

## 3. Declare and Call a Function

```javascript
function calculateArea(length, width) {
    return length * width;
}

console.log(calculateArea(10, 5));
console.log(calculateArea(8, 4));
```

**Output:**

```text
50
32
```

## 4. Check Types with typeof

```javascript
let number = 10;
let text = "Hello";
let booleanValue = true;
let nullValue = null;
let objectValue = { name: "Riya" };
let arrayValue = [1, 2, 3];

function greet() {
    return "Hello";
}

console.log(number, typeof number);
console.log(text, typeof text);
console.log(booleanValue, typeof booleanValue);
console.log(nullValue, typeof nullValue);
console.log(objectValue, typeof objectValue);
console.log(arrayValue, typeof arrayValue);
console.log(greet, typeof greet);
```

**Output:**

```text
10 number
Hello string
true boolean
null object
{ name: 'Riya' } object
[1, 2, 3] object
[Function: greet] function
```

# Part I — Naming Rules & Best Practices

## 5. Valid vs Invalid Variable Names

```javascript
let userName;       // Valid
// let 2ndPlace;    // Invalid: cannot start with a number
let _privateData;   // Valid
let $price;         // Valid
// let my-age;      // Invalid: hyphens are not allowed
// let function;    // Invalid: reserved keyword
let totalCount;     // Valid
// let const;       // Invalid: reserved keyword
```

## 6. Apply Best Practices

```javascript
const length = 10;
const width = 5;
let area = length * width;
const MAX_SCORE = 100;

console.log(area);
console.log(MAX_SCORE);
```

**Output:**

```text
50
100
```

# 7. Declaration & Assignment

```javascript
let age;
age = 18;

let name = "Manthan";

const country = "India";

console.log(age);
console.log(name);
console.log(country);
```

**Output:**

```text
18
Manthan
India
```

# Part J — Prediction & Fixing

## 8. Predict the Output

```javascript
let person = { name: "Amit", age: 22 };
let colors = ["red", "green", "blue"];

function sayHi() {
    return "Hi!";
}

let empty = null;

console.log(typeof person);
console.log(typeof colors);
console.log(typeof sayHi);
console.log(typeof empty);
console.log(person.name);
console.log(colors[1]);
console.log(sayHi());
```

**Output:**

```text
object
object
function
object
Amit
green
Hi!
```



## 9. Fix the Program

```javascript
let student1 = { name: "Neha", age: 19 };

let scores = [90, 85, 88];

function greet(name) {
    return "Hello " + name;
}

const maxScore = 100;

console.log(student1.name);
console.log(scores[0]);
console.log(greet("Neha"));
console.log(maxScore);
```

**Output:**

```text
Neha
90
Hello Neha
100
```

**Explanation:** Variable names cannot begin with a number. Arrays must use square brackets to contain multiple values. Functions require parentheses and a parameter list. A `const` variable cannot be reassigned.

## 10. Concept Questions

**a) What is the main difference between an Object and an Array?**

An object stores data using named properties, while an array stores an ordered list of elements accessed using indexes.

Example:

```javascript
let person = {
    name: "Amit",
    age: 22
};

let colors = ["red", "green", "blue"];

console.log(person.name);
console.log(colors[0]);
```

**b) Why does typeof null return "object"? Is null really an object?**

`typeof null` returns `"object"` because of a historical JavaScript implementation quirk. However, `null` is actually a primitive value that represents an intentional absence of a value.

Example:

```javascript
let emptyValue = null;

console.log(typeof emptyValue);
console.log(emptyValue === null);
```

**Output:**

```text
object
true
```

**c) Why is it recommended to keep arrays with a single data type?**

Keeping arrays with a single data type makes code easier to read, understand, maintain, and process. It also reduces unexpected errors.

Example:

```javascript
let marks = [85, 90, 78, 92];

console.log(marks);
```

**d) When should you use const and when should you use let?**

Use `const` when a variable should not be reassigned. Use `let` when its value needs to change.

Example:

```javascript
const country = "India";

let score = 50;
score = 80;

console.log(country);
console.log(score);
```

**Output:**

```text
India
80
```
