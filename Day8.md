# Pair programming
is when two programmers work together on the same computer to write code. One person types (the "driver"), and the other person gives ideas, catches mistakes, and helps (the "observer"). It's like teamwork for writing computer programs, making the code better and reducing errors.
  
<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/5475ea14-d29e-4e9e-b770-f0937f936200">

### A closure:
closure in JavaScript is like a little backpack that a function carries with it. Inside the backpack, the function can keep special things, like variables from its parent function, even after the parent function is done running. This lets the function remember stuff for later when it's used again.

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/ac0a6a9b-0c52-42c9-bc88-7467fc0d7daf">

### A function with "memory"
in JavaScript is like a special function that remembers things from the past. Imagine it's like a toy that counts and remembers how many times you play with it, even after you stop playing. So, you can ask the toy later, "Hey, how many times did we play?" and it still knows the count. In JavaScript, you can create functions that remember stuff like this using closures.

*************
<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/bc6fc258-0efe-40db-89ab-de744acf396f">

*************
### Calling a function in the same function call as it was defined

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/90d09ff1-5dcb-4728-84e7-433d3a3279ea">

### Calling a function outside of the function call in which it was defined

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/7dcff3f9-1306-4cfc-9d54-f432878fbb05">

## The bond
When a function is defined, it gets a bond to the surrounding Local Memory
(“Variable Environment”) in which it has been defined

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/3a2f106d-d30e-47ca-8b7c-60a39e426d3b">

The ‘backpack’ (or ‘closure’) of live data is attached incrementCounter (then to
myNewFunction) through a hidden property known as [[scope]] which persists
when the inner function is returned out

## Closure gives our functions persistent memories and entirely new toolkit for writing professional code





Helper functions: Everyday professional helper functions like ‘once’ and ‘memoize’

Iterators and generators: Which use lexical scoping and closure to achieve the
most contemporary patterns for handling data in JavaScript

Module pattern: Preserve state for the life of an application without polluting the
global namespace

Asynchronous JavaScript: Callbacks and Promises rely on closure to persist state
in an asynchronous environment


*********************

## Question 1:
Write a closure named createCounter that takes an initial value start and returns a function. The returned function, when invoked, should increment the counter by 1 and return the updated value.

## solve 

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/63b24952-23cb-4011-a3dd-0998cdc72ad4">

************
## Question 2:
Write a closure named calculateAverage that takes an array of numbers, nums, and returns a function. The returned function, when invoked, should calculate and return the average of the numbers in the array.
## solve 

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/2f8f27e7-8087-4eee-8027-4df2767f52c4">


***********
## Question 3:
Write a closure named powerOf that takes a base number base and returns a function. The returned function, when invoked with an exponent exp, should calculate and return the result of base raised to the power of exp.

## solve 

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/ef6db48f-5436-4c50-8b03-21be89d391b1">



*************
## Question 4:
Write a closure named compose that takes multiple functions as arguments and returns a new function. The returned function should apply the provided functions in reverse order, passing the result of each function as an argument to the next function.
  return calculatePower;
}

## solve

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/d263e4d3-a08e-4215-8d6d-821bce62c2c9">

