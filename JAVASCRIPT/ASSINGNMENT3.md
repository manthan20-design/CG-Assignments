A] Arithmetic Operators
1. Addition (+)

1. Total school collection:

₹15,000 + ₹12,500 = ₹27,500

2. Total pages read:

18 + 25 = 43 pages

3. Total items sold:

125 + 178 = 303 items

4. Predict the output:

Output: "105"

Explanation: When + is used with a string, JavaScript joins the values as strings instead of adding them numerically.

5. Predict the output:

Output: "53"

Explanation: The number 5 is converted to a string and joined with "3".

6. 15 + 27 = 42

7. Total price of a book and a pen:

₹350 + ₹45 = ₹395

8. "25" + 10 gives "2510" because the + operator performs string concatenation when one operand is a string.

9. Remaining wallet balance:

Total spent = ₹1,070. Remaining balance = ₹930.

10. Predict and explain the outputs:

First output: "555" — the first addition joins 5 and "5" into a string, then joins the last 5.

Second output: "105" — 5 + 5 is calculated first, giving 10, which is then joined with "5".

Third output: "555" — the string comes first, so the remaining values are joined to it.

2. Subtraction (-)

1. Empty bus seats:

80 − 53 = 27 seats

2. Final marks:

500 − 35 = 465 marks

3. Remaining boxes:

2,500 − 875 = 1,625 boxes

4. Predict the output:

Output: 7

Explanation: JavaScript converts the numeric string "10" into a number when using subtraction.

5. Predict the output:

Output: 15

6. 100 - 37 = 63

7. Water remaining:

500 − 175 = 325 litres

8. Both "50" - 20 and "50" - "20" produce 30. JavaScript converts the numeric strings into numbers before subtraction.

9. Remaining apples:

Answer: 78 apples.

10. Predict and explain:

First output: 50 — "100" is converted to 100.

Second output: NaN — "abc" cannot be converted into a valid number.

Third output: 3 — 10 - 5 = 5, then 5 - 2 = 3.

Fourth output: 3 — both strings are converted into numbers, and subtraction proceeds from left to right.

3. Multiplication (*)

1. Cost of 8 notebooks:

₹45 × 8 = ₹360

2. Production in 6 hours:

120 × 6 = 720 bottles

3. Total plants:

7 × 15 = 105 plants

4. Predict the output:

Output: 20

5. Predict the output:

Output: 20

Explanation: The multiplication operator converts numeric strings into numbers.

6. 12 * 8 = 96

7. Cost of 4 pizzas:

₹299 × 4 = ₹1,196

8. Both "7" * 6 and "7" * "6" produce 42.

9. Factory production:

Answer: 360 units.

10. Predict and explain:

First output: 30

Second output: NaN — "abc" is not a valid numeric value.

Third output: 25

Fourth output: 0

4. Division (/)

1. Pencils per student:

144 ÷ 12 = 12 pencils

2. Average distance per hour:

360 ÷ 6 = 60 kilometres per hour

3. Money per department:

₹72,000 ÷ 9 = ₹8,000

4. Predict the output:

Output: 5

5. Predict the output:

Output: 20

6. 144 / 12 = 12

7. Students per classroom:

360 ÷ 9 = 40 students

8. Both "100" / 4 and "100" / "4" produce 25.

9. Bill per friend:

Answer: ₹400 per friend.

10. Predict and explain:

First output: Infinity

Second output: -Infinity

Third output: NaN

Fourth output: 2.5

Fifth output: NaN

Explanation: Dividing a positive or negative nonzero number by zero produces positive or negative infinity. 0 / 0 is undefined mathematically and produces NaN in JavaScript. Invalid numeric strings also produce NaN.

5. Modulus (%)

The modulus operator returns the remainder after division.

1. Students left over:

53 % 5 = 3 students

2. Candies left unpacked:

128 % 10 = 8 candies

3. Toys left over:

237 % 6 = 3 toys

4. People left after filling full buses:

185 % 40 = 25 people

5. Predict the output:

Output: NaN

6. 29 % 5 = 4

7. 23 % 4 = 3 chocolates left over.

8. 0 % 7 gives 0, while 15 % 0 gives NaN because division by zero cannot produce a defined remainder.

9. Pages per sheet:

Answer: 7 full sheets and 5 pages left over.

10. Predict and explain the outputs:

First output: 2

Second output: -2

Third output: 2

Fourth output: -2

Fifth output: NaN

Explanation: In JavaScript, the remainder generally has the same sign as the dividend (the number on the left). Therefore, negative dividends produce negative remainders in these examples.

6. Exponentiation (**)

The exponentiation operator raises a base number to a power.

1. Volume of a cube:

6∗∗3=6×6×6=216 cm
3

2. Cells in a square arrangement:

9∗∗2=9×9=81 cells.

3. 5∗∗4=5×5×5×5=625

4. Total pixels:

1024∗∗2=1,048,576 pixels.

5. Predict the output:

Output: 0.5

Explanation: A negative exponent gives the reciprocal. Thus, 2
−1
=1/2.

6. 3 ** 4 = 81

7. Area of a square:

Answer: 81 square units.

8. 2 ** 5 = 32 and 5 ** 2 = 25. They are not equal because their bases and exponents are different.

9. Predict and explain:

First output: 512 — exponentiation is right-associative, so this means 2∗∗(3∗∗2)=2∗∗9.

Second output: 64 — parentheses make it (2∗∗3)∗∗2=8∗∗2.

Third output: 0.125 — 2
−3
=1/8.

The commented-out expression produces no output. If uncommented, -2 ** 2 causes a SyntaxError because the unary minus cannot appear directly before exponentiation without parentheses.

Fifth output: 4 — (-2) ** 2 = 4.

Sixth output: 2 — 4 ** 0.5 calculates the square root of 4.

10. Predict the output:

Output: 1

Explanation: Any nonzero number raised to the power of zero equals 1.

B] Assignment Operators
1. Simple Assignment (=)

1. Store a student's name and marks:

2. Create a score variable with value 0:

3. Assign 50 to three variables using chained assignment:

4. Predict the output:

Output: 100

5. Predict the output:

Output: 15 30

Explanation: q receives a copy of the value of p. Changing q does not change p.

2. Add and Assign (+=)

1. Update the player's score:

2. Update the wallet balance:

3. Predict the output:

Output: 15

4. Predict the output:

Output: "Good Morning"

5. Final value of n:

Output: "205"

Explanation: Because "5" is a string, the += operation joins it to 20 instead of performing numeric addition.

3. Subtract and Assign (-=)

1. Update player health:

2. Update stock:

3. Predict the output:

Output: 3

4. Predict the output:

Output: 25

Explanation: The numeric string "40" is converted to a number before subtraction.

5. Result of x -= 5:

Output: NaN

Explanation: "abc" cannot be converted into a valid number, so the subtraction produces NaN.

4. Multiply and Assign (*=)

1. Apply 18% GST to an item costing ₹500:

Answer: ₹590

2. Triple a quantity of 8:

3. Predict the output:

Output: 220.00000000000003 is possible in JavaScript because of floating-point precision; the mathematical result is 220.

4. Predict the output:

Output: 21

5. Result of y *= 2:

Output: NaN

Explanation: "hello" is not a valid number, so multiplication produces NaN.

5. Divide and Assign (/=)

1. Divide 180 chocolates equally among 6 children:

Answer: 30 chocolates per child.

2. Calculate average speed:

Answer: 60 km/h

3. Predict the output:

Output: 50

4. Predict the output:

Output: 25

5. Result of dividing by zero:

Output: Infinity

Explanation: A positive, nonzero number divided by zero produces Infinity in JavaScript.

6. Modulus and Assign (%=)

1. Store the remainder when 47 is divided by 6:

2. Keep only the remainder when 23 is divided by 12:

3. Predict the output:

Output: 4

4. Predict the output:

Output: 2

5. Result when the divisor is zero:

Output: NaN

Explanation: The remainder operation with zero as the divisor is undefined in JavaScript.

7. Exponentiation and Assign (**=)

1. Calculate the volume of a cube with a side of 5:

Answer: 125 cubic units.

2. Square the number 4:

3. Predict the output:

Output: 32

4. Predict the output:

Output: 2

5. Result of p **= -1:

Output: 0.5

Explanation: A negative exponent returns the reciprocal of the base raised to the corresponding positive power.

C] Comparison Operators

Comparison operators return a Boolean value: true or false.

1. Loose Equality (==)

1. Check whether "25" is loosely equal to 25:

Output: true

Explanation: The loose equality operator allows type conversion before comparing values.

2. Check whether 0 == false:

Output: true

3. Predict the output:

Outputs:

true

true

4. Predict the output:

Outputs:

true

true

Explanation: Loose equality performs type conversions. An empty string and an empty array can both compare equal to false under these conversions.

5. Why does NaN == NaN return false?

Answer: NaN represents an invalid or unrepresentable numeric result. It is not equal to any value, including itself, so NaN == NaN returns false.

2. Loose Inequality (!=)

1. Check whether "18" != 18:

Output: false

Explanation: After type conversion, both values are equal.

2. A stored password is "1234" and the entered value is the number 1234. Will != return true?

Answer: No. "1234" != 1234 returns false because loose inequality converts the values before comparison.

3. Predict the output:

Outputs:

false
