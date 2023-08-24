


### 1. Scope:

What it is: Scope defines where variables and functions are accessible in your code.
Imagine: Think of scope like different rooms in a house. Each room has its own things (variables/functions) that are only accessible in that room.
Example: If you declare a variable inside a function, you can only use it within that function.

### 2. Nested Scope:
What it is: Nested scope means having scopes inside other scopes, like rooms within rooms.
Imagine: It's like having smaller rooms inside bigger rooms. Things from the big room might not be easily accessible in the smaller rooms.
Example: If you have a function inside another function, the inner function can access its own variables and the variables of the outer function, but not the other way around.


### 3. Hoisting:
What it is: Hoisting moves declarations (not assignments) to the top of their scope during compilation.
Imagine: It's like reading a storybook. You know the main characters' names before you start reading about them in the story.
Example: You can use a variable before you declare it, but only if the declaration is hoisted to the top of the scope.


### 4. Closure:
What it is: A closure is when a function "remembers" its surrounding variables even after the function has finished running.
Imagine: Think of a lunchbox. It keeps your food safe and warm until you're ready to eat, even if you're far from the kitchen.
Example: A function inside another function can still access the variables of the outer function even after the outer function has completed.


### 5. Modules:
What it is: Modules let you organize your code into separate files and use only what you need in each part of your program.
Imagine: Imagine a toolbox with compartments. You only take out the tools you need for a specific task, keeping everything else organized.
Example: Instead of writing all your code in one big file, you can break it into smaller files (modules) for different parts of your application.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/f550335f-6eb1-4e7f-80b0-e65efd8454d9" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e2cdf516-79cf-41d8-8ba5-433429dcbb4f" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/ce28259a-e84a-4364-b946-ca928863c2c8" width="444">

#### To use strict mode, you just write "use strict"; at the top of your JavaScript code. It's like saying, "Hey, let's be extra careful and make sure our code is clean and reliable."
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/cab093a2-4f1d-4a42-8b6f-186a8a493cee">

#### In JavaScript, when you have a function inside another function, the inner function creates a nested scope. Variables declared inside the outer function are accessible in both the outer and inner functions. But variables declared inside the inner function are only accessible within that inner function.


### "undefined" and "undeclared" refer to different concepts related to variables. 

#### 1. Undefined:
What it means: "Undefined" refers to a variable that has been declared but hasn't been assigned a value yet.
Example: If you declare a variable x but don't assign any value to it, x is considered "undefined."


#### 2. Undeclared:
What it means: "Undeclared" refers to a variable that has been used in code without being formally declared using var, let, or const.
Example: If you use a variable y without declaring it first with var, let, or const, y is considered "undeclared."

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/db61719f-8fb9-40df-8528-7d60ea373fb2" width="444">

##  Function Expressions:
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/211ea78f-80bf-42ae-bebf-3b22b419312d">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/05dae1aa-1d7d-4449-ad7a-35a87c574c1c">

##### Function expressions are handy because you can store functions as variables. This makes them easy to pass around, use as arguments in other functions, or even store in objects or arrays.


## Arrow function:
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/86b34068-3cc8-46f0-8702-8e3686689e29">

##### arrow functions are like writing cooking instructions using clear and direct sentences to make your code easy to understand and maintain!


# QUESTION #1

Create a function called arrowHOF that takes an arrow function as input and returns a new arrow function that enhances the behavior of the input function.

The enhanced function should accept additional arguments and execute the input function multiple times based on these arguments.

const exampleNormalFunc1 = (a, b, c) => {
  return a * (b + c);
}

const exampleNormalFunc2 = (x, y) => {
  return x * y;
}

const exampleNormalFunc3 = (string) => {
  return string + " " + string + " " + string + "!";
}


const arrowHOF = (normalFunc) => {
  // write your code here;
}

const hofNormalFunc1 = arrowHOF(exampleNormalFunc1);
const hofNormalFunc2 = arrowHOF(exampleNormalFunc2);
const hofNormalFunc3 = arrowHOF(exampleNormalFunc3);

console.log(hofNormalFunc1(3, 4, 5)(2)); // logs 60 twice
console.log(hofNormalFunc2(20, 35))(4); // logs 700 four times
console.log(hofNormalFunc3("Meow")()); // logs "Meow Meow Meow!" once

# SOL:
```
const exampleNormalFunc1 = (a, b, c) => {
  return a * (b + c);
};

const exampleNormalFunc2 = (x, y) => {
  return x * y;
};

const exampleNormalFunc3 = (string) => {
  return string + " " + string + " " + string + "!";
};

const arrowHOF = (normalFunc) => {
  return (...args1) => {
    return (...args2) => {
      const result = normalFunc(...args1);
      return (...multiplier) => {
        const multi = multiplier[0];
        return Array.from({ length: multi }, () => result(...args2));
      };
    };
  };
};

const hofNormalFunc1 = arrowHOF(exampleNormalFunc1);
const hofNormalFunc2 = arrowHOF(exampleNormalFunc2);
const hofNormalFunc3 = arrowHOF(exampleNormalFunc3);

console.log(hofNormalFunc1(3, 4, 5)(2)); // logs 60 twice
console.log(hofNormalFunc2(20, 35)(4)); // logs 700 four times
console.log(hofNormalFunc3("Meow")());  // logs "Meow Meow Meow!" once

```








# QUESTION #2
Build a function called preserveThis that takes a function as input and returns a new arrow function that behaves the same way as the input function but preserves the original this context when used as a method of an object.

// Example object
const obj = {
  name: 'John',
  greet: function (greeting) {
    console.log(`${greeting}, ${this.name}!`);
  }
};

const preserveThis = (func) => {
  // write your code here;
  return func;
}

// Wrap the greet function using preserveThis
const preservedGreet = preserveThis(obj.greet);

// Call the wrapped function as a method of the object
preservedGreet('Hello'); // Output: "Hello, John!"

# SOL:
```
const obj = {
  name: 'John',
  greet: function (greeting) {
    console.log(`${greeting}, ${this.name}!`);
  }
};

const preserveThis = (func) => {
  return (...args) => {
    return func.apply(this, args);
  };
}

const preservedGreet = preserveThis(obj.greet);

preservedGreet('Hello'); // Output: "Hello, John!"

```







# QUESTION #3
Consider the 2 following examples and distinguish the different output in each one with them with a reasoning.

Example 1:

function outer1() {
  var x = 10;

  var inner1 = function() {
    console.log(x);
  };

  inner1();
}

outer1(); // Output: 10
Reasoning for example 1's output:
.................................................................................

Example 2:

function outer2() {
  var x = 10;

  var inner2 = function() {
    var x = 20;
    console.log(x);
  };

  inner2();
}

outer2(); // Output: 20
Reasoning for example 2's output:


# SOL:
In Example 1, the inner function inner1 accesses the x variable from its parent scope, which is the outer1 function, resulting in an output of 10.
In Example 2, the inner function inner2 defines its own x variable with a value of 20, so it logs 20 when executed within the outer2 function.



















