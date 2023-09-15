# Week 1 Class 8
- - - - - - - - - - - - - - - -
- - - - - - - - - - - - - - - -
## "What is an expression in JavaScript?"
- - - - - - - - - - - - - - - -
An expression in JavaScript is a combination of values, variables, operators, and functions that produces a result. It can be as simple as a single value or as complex as a multi-step computation. For example, 3 + 5 is an expression that evaluates to 8.
- - - - - - - - - - - - - - - -
## "Why would we use a loop in our code?"
- - - - - - - - - - - - - - - -
We use loops in our code to repeat a block of code multiple times, automating tasks that require iteration. Loops are essential for processing arrays, lists, and performing repetitive operations like calculating the sum of numbers or iterating through object properties. For example:
```
// Using a for loop to iterate through an array
const numbers = [1, 2, 3, 4, 5];
for (let i = 0; i < numbers.length; i++) {
    console.log(numbers[i]);
}
```
- - - - - - - - - - - - - - - -
## "When does a loop stop executing?"
- - - - - - - - - - - - - - - -
A for loop stops executing when the condition specified in the loop header evaluates to false. In the following example, the loop stops when i becomes greater than or equal to 5:

```
for (let i = 0; i < 5; i++) {
    console.log(i);
}
// Outputs: 0 1 2 3 4
```
- - - - - - - - - - - - - - - -
## "How many times will a while loop execute?"
- - - - - - - - - - - - - - - -
A while loop executes as long as its specified condition remains true. The number of times it executes depends on when the condition becomes false. For example, in this code, the while loop executes five times:

```
let count = 0;
while (count < 5) {
    console.log(count);
    count++;
}
// Outputs: 0 1 2 3 4
```
It's crucial to ensure that the loop's condition eventually becomes false, or you risk creating an infinite loop that can crash your program.
- - - - - - - - - - - - - - - - 