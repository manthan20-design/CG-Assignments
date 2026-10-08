// ==========================================
// ASSIGNMENT: JAVASCRIPT OPERATORS
// ==========================================


// ==========================================
// A] ARITHMETIC OPERATORS
// ==========================================


// ------------------------------------------
// 1. ADDITION +
// ------------------------------------------

// Q1
console.log(15000 + 12500); // 27500

// Q2
console.log(18 + 25); // 43

// Q3
console.log(125 + 178); // 303

// Q4
let a1 = "10";
let b1 = 5;
let result1 = a1 + b1;
console.log(result1); // 105

// Q5
let x1 = 5;
let y1 = "3";
let result2 = x1 + y1;
console.log(result2); // 53

// Q6
console.log(15 + 27); // 42

// Q7
console.log(350 + 45); // 395

// Q8
console.log("25" + 10); // 2510

// Q9
let spent = 750 + 320;
let balance = 2000 - spent;

console.log(spent);   // 1070
console.log(balance); // 930

// Q10
console.log(5 + "5" + 5); // 555
console.log(5 + 5 + "5"); // 105
console.log("5" + 5 + 5); // 555



// ------------------------------------------
// 2. SUBTRACTION -
// ------------------------------------------

// Q1
console.log(80 - 53); // 27

// Q2
console.log(500 - 35); // 465

// Q3
console.log(2500 - 875); // 1625

// Q4
let a2 = "10";
let b2 = 3;
let result3 = a2 - b2;
console.log(result3); // 7

// Q5
let x2 = "20";
let y2 = "5";
let result4 = x2 - y2;
console.log(result4); // 15

// Q6
console.log(100 - 37); // 63

// Q7
console.log(500 - 175); // 325

// Q8
console.log("50" - 20);   // 30
console.log("50" - "20"); // 30

// Q9
let apples = 240 - 95 - 67;
console.log(apples); // 78

// Q10
console.log("100" - 50); // 50
console.log("abc" - 10); // NaN
console.log(10 - "5" - "2"); // 3
console.log("10" - "5" - "2"); // 3



// ------------------------------------------
// 3. MULTIPLICATION *
// ------------------------------------------

// Q1
console.log(45 * 8); // 360

// Q2
console.log(120 * 6); // 720

// Q3
console.log(7 * 15); // 105

// Q4
let a3 = "5";
let b3 = 4;
let result5 = a3 * b3;
console.log(result5); // 20

// Q5
let x3 = "10";
let y3 = "2";
let result6 = x3 * y3;
console.log(result6); // 20

// Q6
console.log(12 * 8); // 96

// Q7
console.log(299 * 4); // 1196

// Q8
console.log("7" * 6);   // 42
console.log("7" * "6"); // 42

// Q9
let units = 45 * 8;
console.log(units); // 360

// Q10
console.log("5" * 3 * "2"); // 30
console.log("abc" * 4); // NaN
console.log(10 * "2.5"); // 25
console.log("10" * "2.5" * "0"); // 0



// ------------------------------------------
// 4. DIVISION /
// ------------------------------------------

// Q1
console.log(144 / 12); // 12

// Q2
console.log(360 / 6); // 60

// Q3
console.log(72000 / 9); // 8000

// Q4
let a4 = "20";
let b4 = 4;
let result7 = a4 / b4;
console.log(result7); // 5

// Q5
let x4 = "100";
let y4 = "5";
let result8 = x4 / y4;
console.log(result8); // 20

// Q6
console.log(144 / 12); // 12

// Q7
console.log(360 / 9); // 40

// Q8
console.log("100" / 4);   // 25
console.log("100" / "4"); // 25

// Q9
let share = 2400 / 6;
console.log(share); // 400

// Q10
console.log(10 / 0); // Infinity
console.log(-10 / 0); // -Infinity
console.log(0 / 0); // NaN
console.log("20" / "4" / 2); // 2.5
console.log("abc" / 5); // NaN



// ------------------------------------------
// 5. MODULUS %
// ------------------------------------------

// Q1
console.log(53 % 5); // 3

// Q2
console.log(128 % 10); // 8

// Q3
console.log(237 % 6); // 3

// Q4
console.log(185 % 40); // 25

// Q5
let a5 = 10;
let b5 = 0;
let result9 = a5 % b5;
console.log(result9); // NaN

// Q6
console.log(29 % 5); // 4

// Q7
console.log(23 % 4); // 3

// Q8
console.log(0 % 7); // 0
console.log(15 % 0); // NaN

// Q9
console.log(Math.floor(47 / 6)); // 7 full sheets
console.log(47 % 6); // 5 pages left

// Q10
console.log(17 % 5); // 2
console.log(-17 % 5); // -2
console.log(17 % -5); // 2
console.log(-17 % -5); // -2
console.log(10 % 0); // NaN



// ------------------------------------------
// 6. EXPONENTIATION **
// ------------------------------------------

// Q1
console.log(6 ** 3); // 216

// Q2
console.log(9 ** 2); // 81

// Q3
console.log(5 ** 4); // 625

// Q4
console.log(1024 ** 2); // 1048576

// Q5
let base = 2;
let power = -1;
let result10 = base ** power;
console.log(result10); // 0.5

// Q6
console.log(3 ** 4); // 81

// Q7
console.log(9 ** 2); // 81

// Q8
console.log(2 ** 5); // 32
console.log(5 ** 2); // 25

// Q9
console.log(2 ** 3 ** 2); // 512
console.log((2 ** 3) ** 2); // 64
console.log(2 ** -3); // 0.125

// console.log(-2 ** 2); 
// SyntaxError

console.log((-2) ** 2); // 4

console.log(4 ** 0.5); // 2

// Q10
let a6 = 10;
let b6 = 0;
let result11 = a6 ** b6;
console.log(result11); // 1
