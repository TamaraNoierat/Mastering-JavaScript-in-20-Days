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
### NaN stands for "not a number." It's a special value that represents the result of an operation that should produce a number, but for some reason, the result isn't a valid number.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/6e9904d6-f9b7-40bf-ba90-252c72cd1967" width="355">


// if you use the typeof operator on NaN, it will return "number"


console.log(typeof NaN);  // Outputs: "number"


```
Object.is(value1, value2);
```
Object.is:This method is used to determine if two values are the same. It's similar to the === (strict equality) operator, but with a few differences in how it handles certain special values like NaN and negative zero.
The method returns true if the values are the same, considering special cases like NaN and negative zero.
The method returns false if the values are not the same.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/49456368-5a68-4e5a-9990-51dca693e1eb" width="355">



*******************************
 the Math.sign() function is used to determine the sign of a number. It returns a value indicating whether the number is positive, negative, or zero. The function returns one of three possible values:

If the number is positive, Math.sign() returns 1.
If the number is negative, Math.sign() returns -1.
If the number is zero, Math.sign() returns 0.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4e82c66b-144d-4afb-8592-ec54000a0f96" width="444">


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/d4710ad1-cdfe-4fd1-ae67-fe10ffc56125" width="444">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/f421fab6-ffa1-4d6a-be0c-200bed3773c7">


******************************
 ## Use new:
 ```
const obj = new Object();
const arr = new Array();
const func = new Function('console.log("Hello, world!");');
const currentDate = new Date();
const regex = new RegExp('\\d{2}-\\d{2}-\\d{4}');
const customError = new Error('This is a custom error message.');


```
RegExp(): The RegExp constructor creates a new regular expression instance for matching patterns in strings.
Error(): The Error constructor creates a new error instance. Other more specific error constructors (like TypeError, SyntaxError, etc.) inherit from this one.
Date(): The Date constructor creates a new date instance representing a specific point in time.


### Don't use new:
• String()
• Number()
• Boolean()


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8839bf36-cd03-47a1-9848-5016ce18cf96">
**************************************************
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9e9f10ed-4b8e-4781-9ebb-ef6e71e7f277 "

## ToPrimitive:
ToPrimitive" refers to how a non-primitive data type (like an object) is converted to a primitive value (string, number, or boolean) when it's needed in a context where a primitive value is expected.
```
const obj = {
  valueOf: function() {
    return 42;
  },
  toString: function() {
    return "Hello";
  }
};

console.log(obj + 10); // The object is converted to a number: 42 + 10 = 52
console.log("Value: " + obj); // The object is converted to a string: "Value: Hello"

```


## tostring
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c3c28885-27c5-4c56-acf1-e26b91fce711" width="355">

## to string(object)
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4fc961a3-bab4-4fd7-8c68-d0db1bd707dc" width="355">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/db3cedbc-74c8-40c8-b856-51518205530e" width="355">

```
const number = 42;
const str = number.toString(); // Converts the number 42 to the string "42"
console.log(typeof str); // Outputs: "string"

```


```
const obj = { key: 'value' };
const objStr = obj.toString();
console.log(objStr); // Outputs: "[object Object]"
```

### ToNumber:
#### 1-Primitive Values:
Numbers: If the value is already a number, no conversion is needed.
Strings: If the string is a valid numeric representation, it's converted to a number. If not, it becomes NaN (Not-a-Number).
Booleans: true becomes 1 and false becomes 0.
```
const numStr = "42";
const num = Number(numStr); // Converts the string "42" to the number 42
console.log(num); // Outputs: 42

```

#### 2-Objects:
Objects undergo the ToPrimitive operation first, and then the resulting primitive value (if it's not already a number) is converted to a number following the rules above.
```
const obj = {
  valueOf: function() {
    return 42;
  }
};

const numFromObj = Number(obj); // Converts the object to the number 42
console.log(numFromObj); // Outputs: 42

```
#### Other Values:
null becconst nullValue = null;
const undefinedValue = undefined;


```
console.log(Number(nullValue)); // Outputs: 0
console.log(Number(undefinedValue)); // Outputs: NaN
omes 0.
undefined becomes NaN.
```
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/50b2a0ae-5da3-4ec1-99d2-c5203e03b776" widyh="333">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8313da4e-0d46-4957-a8c3-5cfd365faf3d" width="333">

















