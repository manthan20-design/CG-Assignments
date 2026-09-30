1. Personal Information

let name = "Manthan";
let age = 17;
let city = "Gandhinagar";

console.log(name);
console.log(age);
console.log(city);

2. Change the Score

let score = 50;
score = 80;

console.log(score);

let is used because the value changes.

3. Constant Value

const PI = 3.14;

console.log(PI);

4. Uninitialized Variables

var num1;
let num2;

console.log(num1);
console.log(num2);

num1 = 10;
num2 = 20;

console.log(num1);
console.log(num2);

Output initially:

undefined
undefined
Part B

5. Choose the Correct Keyword

const studentName = "Manthan";
let marks = 75;
const schoolName = "ABC School";

marks = 90;

console.log(studentName);
console.log(marks);
console.log(schoolName);

6. Understand Scope

if (true) {
    var a = 10;
    let b = 20;
    const c = 30;
}

console.log(a); // 10
console.log(b); // Error
console.log(c); // Error

Explanation: var is function-scoped, while let and const are block-scoped.

7. Test Re-declaration

var user = "Manthan";
var user = "Rahul";

console.log(user);

Output:

Rahul

With let:

let user = "Manthan";
let user = "Rahul"; // Error

Answer: var allows re-declaration in the same scope; let does not.

8. Test Re-assignment

var a = 10;
let b = 20;
const c = 30;

a = 100;
b = 200;
c = 300; // Error

console.log(a);
console.log(b);
console.log(c);

var → re-assignment allowed
let → re-assignment allowed
const → re-assignment not allowed

Part C

9. Predict and Explain

Given:

var x = 10;

if (true) {
    var x = 20;
    let y = 30;
    const z = 40;
}

console.log(x);
console.log(y);
console.log(z);

Output:

20
ReferenceError
ReferenceError

Why?

x is declared using var, so it is accessible outside the if block. Its value becomes 20.
y uses let, so it is limited to the if block.
z uses const, so it is also limited to the if block.
10. Fix the Program

Original problems:

const name; → a const variable must be initialized.
let age is declared twice in the same scope.
country is declared inside the if block, so it can't be accessed outside.
const score cannot be reassigned.

Corrected program:

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
