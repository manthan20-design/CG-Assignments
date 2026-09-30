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

**Explanation:**
`const name` is initialized when declared.

`age` is declared only once and then its value is changed.

`country` is printed inside the `if` block because `let` is block-scoped.

`city` can be accessed outside the block because it is declared using `var`.

`score` is changed from `50` to `80`, so it uses `let` instead of `const`.
