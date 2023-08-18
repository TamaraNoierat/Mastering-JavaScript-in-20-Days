# Pair programming
is when two programmers work together on the same computer to write code. One person types (the "driver"), and the other person gives ideas, catches mistakes, and helps (the "observer"). It's like teamwork for writing computer programs, making the code better and reducing errors.
  
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9a7493d5-a496-4e41-9dc8-bad62830d8b0">

### A closure:
closure in JavaScript is like a little backpack that a function carries with it. Inside the backpack, the function can keep special things, like variables from its parent function, even after the parent function is done running. This lets the function remember stuff for later when it's used again.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/00227e61-9010-40cc-bace-6689c88695ef">

### A function with "memory"
in JavaScript is like a special function that remembers things from the past. Imagine it's like a toy that counts and remembers how many times you play with it, even after you stop playing. So, you can ask the toy later, "Hey, how many times did we play?" and it still knows the count. In JavaScript, you can create functions that remember stuff like this using closures.

*************
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/0bf4d764-1c1a-4752-a12c-dc7d49f6ee9f">

*************
### Calling a function in the same function call as it was defined

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/31411a30-551a-483f-9b6b-7a619fa59830">

### Calling a function outside of the function call in which it was defined

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/7401b013-8232-4ebc-b284-f9e99045a237">

## The bond
When a function is defined, it gets a bond to the surrounding Local Memory
(“Variable Environment”) in which it has been defined

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/adb00c33-50c4-4332-a127-1794d3771094">

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

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/32f8e82f-7184-45d4-ada4-c59428087613">

************
## Question 2:
Write a closure named calculateAverage that takes an array of numbers, nums, and returns a function. The returned function, when invoked, should calculate and return the average of the numbers in the array.
## solve 

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/ade0a7a6-922e-410e-a635-0d74f159df29">


***********
## Question 3:
Write a closure named powerOf that takes a base number base and returns a function. The returned function, when invoked with an exponent exp, should calculate and return the result of base raised to the power of exp.

## solve 

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/35a7b11a-c7a8-4577-abc1-392742dffb7f">



*************
## Question 4:
Write a closure named compose that takes multiple functions as arguments and returns a new function. The returned function should apply the provided functions in reverse order, passing the result of each function as an argument to the next function.
  return calculatePower;
}

## solve

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/21ba8029-5201-44f9-86a4-8960550cc6ad">

