# DEEP JS FOUNDATIONS
Postfix Operators:
Postfix operators are applied after the operand. The most common example in JavaScript is the increment (++) and decrement (--) operators. When used postfix, they increase or decrease the value of the operand after the value is evaluated.
ex:
```
let x = 5;
let y = x++; // y will be 5, x will be 6
```
Prefix Operators:
Prefix operators are applied before the operand. In JavaScript, the increment (++) and decrement (--) operators can also be used as prefix operators. When used as prefix, they increase or decrease the value of the operand before the value is evaluated.
ex:
```
let a = 10;
let b = ++a; // a will be 11, b will be 11

```
<div>
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/abed7245-d0f0-4389-a538-c337909e70f1" width="355">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/a7d667f5-4c51-4969-bae2-d83fae6323b8" width="333">

</div>
#### In JavaScript, not everything is an object. JavaScript has both primitive data types and objects.

Primitive data types include:

1-Number: Represents both integer and floating-point numbers.

2-String: Represents sequences of characters.

3-Boolean: Represents true or false values.

4-Undefined: Represents a variable that has been declared but hasn't been assigned a value.

5-Null: Represents the intentional absence of any value.

6-Symbol: Represents a unique and immutable value that can be used as an object property.


Objects in JavaScript are more complex data structures that can have properties and methods. They include:

Plain Objects: Created using object literals or the Object constructor.
Arrays: Special type of objects used to store ordered collections of data.
Functions: Objects that can be executed and have their own properties and methods.
Custom Objects: Objects created using constructor functions or classes.
Built-in Objects: Objects provided by the JavaScript environment, like Date, RegExp, Math, etc.


## In JavaScript, variables don't have types, values do:
thats mean:the type of data is determined by the value that is stored in a variable, rather than by the variable itself.

```
let x;       // Here, x doesn't have a specific type yet.
x = 5;       // Now, x holds a number value, so its type is "number."
x = "Hello"; // Now, x holds a string value, so its type is "string."
x = true;    // Now, x holds a boolean value, so its type is "boolean."

```
<div>
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b539f652-7921-4aa0-99b9-c9ba3f39bfa4" width="344">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/ea52833b-ea5e-4a59-8c5a-b3f42043252c"width="344">
</div>

## Undefined: Declared, but no value assigned yet.
## Undeclared: Variable used without being declared first.
## Uninitialized: Declared, but not given an initial value.


