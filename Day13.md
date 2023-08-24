

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



















