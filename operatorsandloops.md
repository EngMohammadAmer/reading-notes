[HOME](README.md)

# Read: 05 - Operators and Loops

## Comparison and logical operators

* Comparison operators — operators that compare values and return true or false. The operators include: >, <, >=, <=, ===, and !==.
* Logical operators — operators that combine multiple boolean expressions or values and provide a single boolean output. The operators include: &&, ||, and !.

### Comparison Operators

Less than (<) — returns true if the value on the left is less than the value on the right, otherwise it returns false.
Greater than (>) — returns true if the value on the left is greater than the value on the right, otherwise it returns false.
Less than or equal to (<=) — returns true if the value on the left is less than or equal to the value on the right, otherwise it returns false.
Greater than or equal to (>=) — returns true if the value on the left is greater than or equal to the value on the right, otherwise it returns false.
Equal to (===) — returns true if the value on the left is equal to the value on the right, otherwise it returns false.
Not equal to (!==) — returns true if the value on the left is not equal to the value on the right, otherwise it returns false.

### Logical Operators

Comparison operators allow us to assert the equality of a statement with JavaScript. For example, we can assert whether two values or expressions are equal with ===, or, whether one value is greater than another with >.

There are scenarios, however, in which we must assert whether multiple values or expressions are true. In JavaScript, we can use logical operators to make these assertions.

&& (and) — This operator will be truthy (act like true) if and only if the expressions on both sides of it are true.
|| (or) — This operator will be truthy if the expression on either side of it is true. Otherwise, it will be falsy (act like false).

# Loops: while and for
We often need to repeat actions.

## The “while” loop
The while loop has the following syntax:

while (condition) {
  // code
  // so-called "loop body"
}

While the condition is truthy, the code from the loop body is executed.

For instance, the loop below outputs i while i < 3:

let i = 0;
while (i < 3) { // shows 0, then 1, then 2
  alert( i );
  i++;
}
A single execution of the loop body is called an iteration. The loop in the example above makes three iterations.

If i++ was missing from the example above, the loop would repeat (in theory) forever. In practice, the browser provides ways to stop such loops, and in server-side JavaScript, we can kill the process.

Any expression or variable can be a loop condition, not just comparisons: the condition is evaluated and converted to a boolean by while.

For instance, a shorter way to write while (i != 0) is while (i):

let i = 3;
while (i) { // when i becomes 0, the condition becomes falsy, and the loop stops
  alert( i );
  i--;
}

## The “for” loop
The for loop is more complex, but it’s also the most commonly used loop.

It looks like this:

for (begin; condition; step) {
  // ... loop body ...
}
Let’s learn the meaning of these parts by example. The loop below runs alert(i) for i from 0 up to (but not including) 3:

for (let i = 0; i < 3; i++) { // shows 0, then 1, then 2
  alert(i);
}
Let’s examine the for statement part-by-part:

part		
begin	i = 0	Executes once upon entering the loop.
condition	i < 3	Checked before every loop iteration. If false, the loop stops.
body	alert(i)	Runs again and again while the condition is truthy.
step	i++	Executes after the body on each iteration.
The general loop algorithm works like this:

Run begin
→ (if condition → run body and run step)
→ (if condition → run body and run step)
→ (if condition → run body and run step)
→ ...
That is, begin executes once, and then it iterates: after each condition test, body and step are executed.

If you are new to loops, it could help to go back to the example and reproduce how it runs step-by-step on a piece of paper.

Here’s exactly what happens in our case:

// for (let i = 0; i < 3; i++) alert(i)

// run begin
let i = 0
// if condition → run body and run step
if (i < 3) { alert(i); i++ }
// if condition → run body and run step
if (i < 3) { alert(i); i++ }
// if condition → run body and run step
if (i < 3) { alert(i); i++ }
// ...finish, because now i == 3

# Summary
We covered 2 types of loops:

while – The condition is checked before each iteration.
for (;;) – The condition is checked before each iteration, additional settings available.
