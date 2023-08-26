# secound Day ✏️

# value & data type
<br>
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/138c49b1-7cb2-4028-bff1-240948b25213" width="455">

<br>
   👉 typeof => tells you the type of a value.
   here is the synatax:   typeof operand

   <br>
   
```
typeof "42" // string
typeof 42 //number
typeof false //boolean
typeof null //object
typeof "some string".length //number
typeof "" //string
```





### js has two kind of data: 
####  1-PRIMITIVE (eg : string , number,boolean, undefined,null,)    
#### 2- OBJECT(eg: document,  friend)

*** undefined is: when something hasn't been given a value yet, 

*** null is: when you're purposely saying there's no value there.

 ### .length:  returns the length of a string.
### String 🔻
are made of a sequence of characters`"super".length //4`are in a specific order, each gets a number, starting at 0 called "index".
index => a number given to a position

#### Examples:
```
"ALOHA"[0]      // “A”
"ALOHA".length  // 5

//What's the index of a specific character?if not exist will return -1
"ALOHA".indexOf("A")  //0
"ALOHA".indexOf("a")  //-1

//Does this string contain some other string?
"ALOHA".includes("LOL")//false
"ALOHA".includes("HA")  // true

//Does this string start with some other string?
"ALOHA".startsWith("AL") // true

// At what index does this substring begin?
"ALOHA".indexOf("HA") // 3

 // Connecting strings together
"ALOHA" + "!"

//we can make all character in string small or capital 
"ALOHA".toLowerCase() // "aloha"
"aloha".toUpperCase() //"ALOHA"


 
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/1b0bc134-ed06-47e4-89ab-ab23deaa2f31">
 indexof : find the first char in the string

 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e8561470-2ead-4986-9ec7-2ce3dcd8a109">

 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/6bfcd9dc-f271-43bc-869f-d7173b67a8f2" width="455">
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b9ef4408-57fe-40d6-bb1c-c26b2427a9bf">
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/0277d408-bcee-48c2-99b8-e5444e2776bc">

 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e18f8c2b-134d-49dc-b20b-aacaa2ccd1a2">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9c29a1ac-8869-4a80-b1bc-c5a30042ed19">

------------------------------------------------------------------------------------------------


 ## Operators ➗🤔 

### Arithmetic operators
-  '+' add
-  '-' subtract
-  '*' multiply
-  '/' divide

  
 ### ➕ operator:
   is an operator with several different uses:
  - when operating on strings => it concatenates the strings ` "abeer" + "belal" `.
  - it can operate on Numbers by adding them `1+1`.
  - it called an overloaded operator because it does different functions.

 
 
### typeof:
The typeof operator returns a string indicating the type of the operand's value.
```
console.log(typeof 42);
// Expected output: "number"

console.log(typeof 'blubber');
// Expected output: "string"
```

### Comparison operators  ⚡️
- '>' greater than
- '<' less than
- '>=' greater than or equal to
- '<=' less than or equal to




### Equality operators:


| strict     | loosey-    | meaning            |
|------------|------------|--------------------|
| ===        | ==         | equals             |
| !==        | !=         | does not equal     |




 ###


| strict        | loosey-goosey | meaning           | Do these differ? How?🤔            |
|---------------|---------------|-------------------|-----------------------------------|
| 1 === 1       | 1 == 1        | equals            | No difference. Both are true.     |
| "1" === "1"   | "1" == "1"    | equals            | No difference. Both are true.     |
| 1 === "1"     | 1 == "1"      | does not equal    | Yes, difference. Strict comparison checks both value and type, so 1 (number) is not equal to "1" (string). Loose comparison only checks the value, so it considers them equal. |


### Nullish coalescing operator (??):🚩
The nullish coalescing (??) operator is a logical operator that returns its right-hand side operand when its left-hand side operand is `null` or `undefined`, and otherwise returns its left-hand side operand.

## Expressions ☄️
an expression evaluates (aka resolves) to a value, more like content.
```
4 / 2 * 10
"Frontend" + "Masters"
5 > 4 !== 3 > 4
```

 ## Variables: 
 A variable is a named reference to a valu—thatt way an unpredictable value can be accessed through a predetermined name.
 - Variables let us remember values.
 - as pointer points to specific value.

  ### Declaring a variable
  - via var keyword ` var name;` 
  - via let keyword ` let name;`
  - via const keyword ` const name;` => const declares & assigns a "constant", aka a variable that can't be changed 

    ### Variable names
   -  camelCase 👉 'variables contain values? e.g: `let FirstName;`
   -  lso_valid_but_less_common
   -  ddbut_Technicallyfine2

### Assigning a variable:
" = "  operator here means assign value to variable 
```
let myDeclaredVariable;
myDeclaredVariable = "so value, much wow";

let myAssignedVariable = "such efficient, amaze"; //Declaring & assigning at once

let x = null;// i want this variable to be empty
let variable; //this will take undefined "nothing"
```
    

 
 ## **Statements vs. Expressions** 👩
 ### An expression "asks" JS for a value


```
myAssignedVariable  // what is the value of my variable
6 + 4               // what is the value of this summation
document.getElementById("board")
```

A **statement**  "tells" JS to do something, actions we want JS to do it

```
// e.g: declare/assign a variable
let ten = 6 + 4;
myDeclaredVariable = "new value";
let board = document.getElementById("board");

function add(x, y) {
    return x + y;
}

let biggest;
if (5 > 4) {
    biggest = 5;
} else {
    biggest = 4;
}
for (let character of "string") {
    console.log(character);
}
```
 








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















 
 

 








