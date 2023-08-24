


# Lexical Scope:
lexical scope means that the accessibility of a variable is determined by where the variable is declared within the source code. Variables declared in an outer scope are accessible in inner scopes, but variables declared in inner scopes are not accessible in outer scopes.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/af594924-0570-4f2f-a61e-41141d924c2b" width="355">


# dynamic scope:
Dynamic scope is a different approach to determining variable scope compared to lexical scope. Unlike lexical scope, where scope is determined by the physical structure of the code, dynamic scope focuses on the call hierarchy of functions when determining variable accessibility.


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3049fee0-e41a-4a1a-bd59-0be36bb33906" width="344">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b05c1560-d5d9-4c93-ae39-cc66a5df491b" width="344">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/02fcb39c-e676-4983-b85c-770b54bb9db9" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/a7e1f392-0973-497f-b08f-6ea97de5fd2f" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/ca9df418-4b5d-4188-87fd-37376dab25ad" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c37d198d-cb65-41e2-9ac5-dba6306a084b" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b9383dd1-2050-4a1b-9f2a-c14d3a0cb4d1" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4cd98e18-2354-48e8-a734-3ba8ff71cda5" width="355">

#### IIFE" stands for "Immediately Invoked Function Expression." It's a design pattern in JavaScript that involves creating a function and immediately invoking it. This pattern is often used to create a private scope for variables and avoid polluting the global scope with unnecessary variables.



#### Block scope is a concept in programming that defines the scope of variables based on blocks of code, typically enclosed within curly braces {}. Block scope is used in languages like JavaScript to limit the visibility of variables to specific blocks of code, such as loops or conditional statements.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/17213587-88f1-4222-a67d-3860dd280b15" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/35138234-227f-47dd-a299-1c6b117c15ef" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/5b2eb87a-7b82-4130-a553-293911b83215" width="355">


#### Choosing between let and var in JavaScript:
###### let and Block Scope:

1-Use let when you want to declare variables with block scope.
2-Variables declared with let are limited to the block (curly braces) in which they are defined.
3-They are not accessible outside of the block they're declared in.
4-This helps prevent variable leaks and conflicts in nested blocks, loops, and conditional statements.
5-Preferred choice for modern JavaScript code.
ex:

```
if (true) {
  let x = 10;  // x is only accessible within this block
}
console.log(x);  // This will result in an error because x is not accessible here

```
#### var and Function Scope:

1-Use var when you want to declare variables with function scope.
2-Variables declared with var are accessible within the function in which they are defined.
3-They can also be accessed outside the function if they are defined outside any block.
4-However, var variables are not limited to the block they're declared in, which can lead to unexpected behavior.
5-Considered somewhat outdated due to the issues it can introduce.
ex:
```
function example() {
  if (true) {
    var y = 20;  // y is accessible within the function
  }
  console.log(y);  // y can be used here, even though it's defined inside an if block
}
example();
console.log(y);  // This will result in an error if y is declared inside the function; otherwise, it will log the value

```




