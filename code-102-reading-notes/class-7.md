# Week 1 Class 7
- - - - - - - - - - - - - - -
- - - - - - - - - - - - - - -
## "What is control flow?"
- - - - - - - - - - - - - - -
Control flow in programming refers to the order in which statements are executed within a program. It determines how the program progresses from one instruction to the next, including conditionals (if/else statements) and loops (for/while loops), allowing for different execution paths based on conditions.
- - - - - - - - - - - - - - -
## "What is a JavaScript function?"
- - - - - - - - - - - - - - -
A JavaScript function is a reusable block of code that performs a specific task. Functions are defined using the function keyword, followed by a name, a set of parameters (if any), and a code block. They encapsulate logic and can be called multiple times with different inputs.

```
function greet(name) {
  console.log("Hello, (name)!");
}
```
- - - - - - - - - - - - - - -
## "What does it mean to 'invoke' 'call' a function?"
- - - - - - - - - - - - - - -
Invoking or calling a function means executing it to perform its defined task. You invoke a function by using its name followed by parentheses, optionally passing arguments **IF** the function expects them.
```
greet("Alice"); // Calling the greet function with the argument "Alice"
```
- - - - - - - - - - - - - - -
## "What are the parenthesis () for when you define a function?"
- - - - - - - - - - - - - - -
In a function definition, parentheses () are used to enclose the parameters that the function accepts. Parameters are placeholders for values that the function expects when it's called. For example, in function greet(name), (name) defines a parameter called name that can be used within the function.
```
function add(a, b) {
  return a + b;
}
```
These parameters allow you to pass data to the function when you call it, like add(3, 5), where 3 and 5 are passed as arguments and are accessible as a and b within the function's code.