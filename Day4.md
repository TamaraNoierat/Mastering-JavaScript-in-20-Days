# Function

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9bb22cca-2776-43ef-b051-4c4a898b8208">

A function is a block of code that can be executed when called (invoked).
Functions are used to perform specific tasks or calculations.
Functions can accept input values (parameters) and return an output value.


# Parameters:


Parameters are variables listed in the function's parentheses when defining it.
They act as placeholders for the values that the function will receive when it's called.
Parameters are like labels for values that a function needs to work with.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/0bae1135-8815-4b7f-b604-ad09129ca7b7">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4828897b-3987-4667-aff0-477e996bd17f">
بالحالتين رح يعطيني ايرور التانية لانو بلشت اسم الفاريابل برقم
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c457df04-7ade-4c20-a3f4-3b86c0cbb013">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/2806dbab-89b8-479a-93fc-21183d0affaf">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/58fdac88-60c8-42b5-8a9d-998fd4dd52f4">

### sol:
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/28df14d1-2bda-431a-8f6a-420130025542" width="444">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/023aeab2-a2e4-4c75-9f73-c46602c0180e" width="444">
  
# Arguments:

Arguments are the actual values that are passed to a function when it's called.
They are the real data that correspond to the parameters in the function definition.
When you call a function, you provide arguments that match the order and number of parameters.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/35d8c09e-ece6-4212-af75-3e4ef4974c1e">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/314ef6b8-f261-47ac-946f-77d42f2c2764">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/eb895c34-a95c-45a9-9814-d9e06c1e3abf">

# Arrow function

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/f851e575-e1e5-40ca-8302-832495561923" width="555">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/38ad7e99-7945-44cb-97a8-26b05437f496" width="555">

### Arrow functions are great when we just want to return a value

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b350dc7e-abd4-4a65-836b-a337aa7d2c10" width="555">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c62b0fcd-3862-4926-9340-f0f4bb5ad8d3" width="666">

An arrow function in JavaScript is a shorter way to write a function using the => syntax. It's great for concise functions and keeps the value of this consistent. Here's how it looks:

#### If we need to do more than just return a value,#### we can use curly braces for a "normal" function body
#### In that case, we still need a return.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/2e939e09-7f4c-41d8-8bbc-e15ec179c39a">

Or, for very short functions:

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/d8e80f82-337d-415a-b477-1729df9c99e6">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/19b1f734-6849-4317-916b-f8b942d07661">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/eb20c075-beb2-4c72-9161-d9fd5c2d7a2c" width="344">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8deb9fba-6156-4da0-85e5-748d21a73ece width="344">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/158876b5-5d96-430b-aa80-c9e0d4d7e410" width="455">

ex :
'''
const addAndLog = (x, y) => {
    let sum = x + y; 
    console.log('The sum is', sum);
    return sum;
}
'''



**************

The removeAttribute method in JavaScript is used to remove an attribute from an HTML element. Here's how it works:

Get the HTML element you want to remove the attribute from, using methods like document.getElementById().
Call the removeAttribute() method on the element and pass the name of the attribute you want to remove as an argument.

# scope
Scope in JavaScript refers to where you can access variables. It determines the visibility and lifespan of variables within your code.

### Global Scope:
Variables declared outside any function or block have global scope. They can be accessed from anywhere in your code, including inside functions.

### Local Scope:
(Function Scope): Variables declared inside a function have local scope. They are only accessible within that function and are not visible from outside.

### Block Scope:
Variables declared with let and const inside blocks (like loops or conditionals) have block scope. They are limited to that specific block.

## let and scope

In JavaScript, let is a keyword used to declare variables with block-level scope. This means that a variable declared with let is only accessible within the block of code where it's defined. 

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/98b4324d-7e43-4ba5-8fb0-7adb15db85a5">

## event
Events in JavaScript are things that happen on a webpage, like clicking a button, moving the mouse, or submitting a form. They allow you to make your webpage interactive and responsive.
Listening for Events: You can tell your code to "listen" for specific events on certain elements. When the event occurs, your code can respond.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/47ab250c-9607-4f3a-b9d9-80993f1a2e2c">

Event Handling: The code that runs when an event occurs is called the event handler. It's like a set of instructions for what to do when an event happens.

Event Objects: When an event occurs, it creates an object containing details about the event. This helps your code understand what happened.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/40e30276-e731-474f-bb9d-1484e6b80a84">

*********************
# Tsaks

## 1

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/612992f8-94e5-4e0d-b740-3fc29549601a">

## 2

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8d1eadb7-05b3-4e2e-b9d8-8d9e710f9fbc">

## 3

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/5f88dfb1-1ad3-4a5e-95ef-9bc70fbce457">

## 4

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c3132906-53fb-479b-8a6f-eb17c017e38d">

