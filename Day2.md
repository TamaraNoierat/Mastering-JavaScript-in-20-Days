# value & data type

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/138c49b1-7cb2-4028-bff1-240948b25213" width="455">

#### typeof tells you type of value



### js has two kind od data: 
####  1-PRIMITIVE (eg : string , number,boolean, undefined,null,)    
#### 2- OBJECT(eg: document,  friend)

*** undefined is: when something hasn't been given a value yet, 

*** null is: when you're purposely saying there's no value there.

 ### .length:  returns the length of a string.
 
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/1b0bc134-ed06-47e4-89ab-ab23deaa2f31">
 indexof : find the first char in the string

 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e8561470-2ead-4986-9ec7-2ce3dcd8a109">

 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/6bfcd9dc-f271-43bc-869f-d7173b67a8f2" width="455">
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b9ef4408-57fe-40d6-bb1c-c26b2427a9bf">
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/0277d408-bcee-48c2-99b8-e5444e2776bc">

 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e18f8c2b-134d-49dc-b20b-aacaa2ccd1a2">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9c29a1ac-8869-4a80-b1bc-c5a30042ed19">

# Operation
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/d3f2ba44-90b6-4a08-b903-45fd662fd6de" width="455">

# Expressions
# Declaring and Assining Variables
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/32084397-007b-4244-a245-c8348e8a1527" width="455">

#### The let declaration declares re-assignable, block-scoped local variables, optionally initializing each to a value.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/ef143e47-e316-4bb2-8885-d026893cbf46">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e5403d75-722b-406e-8a86-1312269ba0a2">


### The const declaration declares block-scoped local variables. The value of a constant can't be changed through reassignment using the assignment operator, but if a constant is an object, its properties can be added, updated, or removed.

# Exercises:::
# Q1:
let a = 0;
let b = "0";
let c = false;
let d = "false";

console.log(a == b);
console.log(b === c);
console.log(!!d);




## SOLUTION:

console.log(a == b);
Output: true
Explanation: JavaScript converts the string "0" to a number 0, so they're equal.

console.log(b === c);
Output: false
Explanation: The types are different, so strict equality (===) is false.

console.log(!!d);
Output: true
Explanation: Double negation turns the non-empty string "false" into the boolean true.


# Q2
console.log(4 + 5 * "7");
## SOLUTION:
JavaScript first converts the string "7" to the number 7, then performs the multiplication, and finally adds the result to 4 to get the output of 39.

# Q3:
let result = 5 + 2 * 3 - 1;
SOL:
JavaScript first performs the multiplication, then the addition, and finally the subtraction to calculate the value of the expression, which is 10.

# Q4:
let x = 10;
let y = '10';
console.log(x == y);
console.log(x === y);
## SOLUTION:
x == y is true because of type coercion (string '10' is converted to number 10).
x === y is false because the types are different (number vs. string).


# Q5::
let num = "15";
let isPositive = true;
let result = (num > 10 && isPositive) || num < 0;
console.log(result);



## SOLUTION::
The final result is true because the first part of the expression (num > 10 && isPositive) evaluates to true, and in a logical OR operation, if one part is true, the whole expression is true.















 
 

 








