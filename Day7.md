#  seventh Day  ✏️


## JavaScript Principles  🎯🚀 
When JavaScript code runs, it:
1. Goes through the code line-by-line and runs/ ’executes’ each line - known as the **thread of execution**
2. Saves ‘data’ like strings and arrays so we can use that data later - in its memory. We can even save code (‘functions’)
   
JavaScript principles are like the basic rules or ideas that help you understand how JavaScript works. Imagine you're learning to play a new game. The game has some fundamental principles that guide how you play and understand it. Similarly, JavaScript has principles that guide how you write and use code in this programming language. These principles make sure your code behaves as you expect and helps you build useful and interactive things on websites.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/037a20ed-01fb-4432-a86c-686a3035f44f">



**Execution context:**
Created to run the code of a 
function - has 2 parts (we’ve 
already seen them!)
- Thread of execution
- Memory











# Call stack

JavaScript keeps track of what
function is currently running
(where’s the thread of execution)
- Run a function - add to call stack
- Finish running the function - JS
removes it from call stack
- Whatever is top of the call stack
- that’s the function we’re
currently running

Call stack: 🔅
  is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function
**JavaScript keeps track of what function is currently running (where’s the thread of execution)**

e.g:
When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.


Run a function - add to call stack
Finish running the function - JS removes it from call stack
Whatever is top of the call stack - that’s the function we’re currently running





## Generalizing functions
By generalizing functions, you make your code more adaptable to different scenarios, reduce repetition, and create a more organized and modular codebase. This approach is essential for writing maintainable and scalable JavaScript applications.
----
----In our code we it is more readable and usable to make it follow the DRY "don't repeat yourself" concept, and avoid repetition
We can generalize the function to make it reusable, we use parameters to apply this principle
‘Parameters’ (placeholders) mean we don’t need to decide what data to run our 
functionality on until we run the function 
- Then provide an actual value (‘argument’) when we run the function



### We could generalize our function - So we pass in our specific
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/fb4c9491-a765-4d73-8789-4914581dce64">

## First class objects🤔

Functions in javascript = first-class objects
They can co-exist with and can be treated like any other javascript object
1. Assigned to variables and properties of other objects
2. Passed as arguments into functions
3. Returned as values from functions


### Higher Order Function VS callback function✨☄️:

| Term                   | Explanation                                                                                     |
|------------------------|-------------------------------------------------------------------------------------------------|
| Callback Function      | The function we insert and pass as an argument. It's the function that will be called later when certain conditions are met. |
| Higher-Order Function  | The outer function that accepts another function as an argument. It's a function that can manipulate or use the passed callback function. |


### Anonymous and arrow functions 🤔
- Improve immediate legibility of the code
- But at least for our purposes here they are ‘syntactic sugar
- we’ll see their full effects later - Understanding how they’re working under the hood is vital to avoid confusion













## How was this possible?
Functions in javascript = first class objects
They can co-exist with and can be treated like any other javascript object
1. Assigned to variables and properties of other objects
2. Passed as arguments into functions
3. Returned as values from functions


### it's like having a cooking recipe that you can use to prepare different dishes. You change the recipe, and you get a different meal using the same cooking techniques. Similarly, you change the instruction when using the generalized function, and you get different results without changing the main function.

## Higher-order functions

Takes in a function or passes out a function
Just a term to describe these functions - any function that does it we call that - but
there's nothing different about them inherently

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/39fdc060-1045-4212-8dc9-fce2b0e4848f">

### We can even pass in multiplyBy2 directly without a name

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/88004c89-84e1-4d23-ac99-3e1e5e97179f">

### Anonymous and arrow functions
anonymous functions are nameless functions often used temporarily, and arrow functions are a short and convenient way to write functions, especially for simple operations.


********************
# 1
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/ccc14bf1-717f-4a0c-b4c5-f68dce877c9a">

# 2

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/53e27edd-e0b9-4e9b-a455-b4eb54cfb3f0">

## Question 1: Functions and Callbacks

Implement a JavaScript function called mapAsync that takes an array and a callback function. 
The function should map each element of the array to a new value using the callback function 
asynchronously. 

The final result should be returned as a Promise.

## solve:
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/33bef53f-9572-44cc-b561-7ddb121da1b1">



**************

## Question 2: Call Stack and Recursion

Write a JavaScript function called sumRange that calculates the sum of all integers in a given range. 
The function should use recursion to handle the calculation and demonstrate understanding of the call stack.

## solve 

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/96ac5f64-7366-4b09-b8c2-197a032f1e00">
