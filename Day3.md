

# Third Day ✏️

<br>


# Array
The Array object, as with arrays in other programming languages, enables storing a collection of multiple items under a single variable name, and has members for performing common array operations.

Arrays let us keep multiple values together in a single collection
` let synonyms = ["plethora", "array", "cornucopia"] `

- Arrays can be empty, or hold a single item
  ```
  javaScript
  let emptyArray = [];
  let oneItemArray = ["lonely"];
  
  ```
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/5e8a70f8-dfd0-48cd-b799-d43f83f4a5b6" width="455">



- Like strings, arrays have a length `synonyms.length`
  <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/fd7020d9-ee9a-42ca-a83d-8acf75eb428b" width="455">
  
- And each value has an index
   `synonyms[1]
synonyms.indexOf("cornucopia")`

- Also like strings, we can check if an array contains a certain value
  `synonyms.includes("plethora")
synonyms.includes("variety")`

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8215839c-7b34-4439-a58e-d3b1dd33977a" width="466"> T || F

- Unlike strings, we can modify arrays

- ### .push() adds elements to the end of an array and changes the original array, while .concat() combines arrays into a new array without modifying the original arrays.
- 
```javaScript
synonyms[1] = "variety";
let lastItem = synonyms.pop();
synonyms.push("multitude");
```
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/99d72db5-0451-47c1-a2aa-e687abbb459b" width="446">

- Arrays can hold any type of items, or mix and match! `let mixedArray = ["pop", 6, "squish", false, document];`
- Arrays can do lots of useful tricks!
-  <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/88088c52-38a5-4381-bc73-29256b244565" width="455">
  ```
  javaScript


  ["c", "a", "d", "b"].sort() // ['a', 'b', 'c']
  [100, 2,50].sort()   // [100, 2,50].sort()  //It converts the elements into strings and then sort them
 
  ["lions", "tigers", "bears oh!"].join(" & ") // 'lions & tigers & bears oh!' // convert it to a string
  [1 , 2].join("@")  // '1@2'

  [1, 2, 3].concat([4, 5, 6]) // [1, 2, 3, 4, 5, 6] 
  ```
  
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9287b387-ee3f-46db-a30c-b1a61d2be52b" width="666">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/9287b387-ee3f-46db-a30c-b1a61d2be52b" width="666">


 ###  Array.prototype.join()
 The join() method creates and returns a new string by concatenating all of the elements in this array, separated by commas or a 
 specified separator string. If the array has only one item, then that item will be returned without using the separator.
 
 <img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/a46bc130-13fa-4a3c-9d95-29baa43e6dcb" width="477">

 
 ```
javaScript
const elements = ['Fire', 'Air', 'Water'];

console.log(elements.join());
// Expected output: "Fire,Air,Water"

console.log(elements.join(''));
// Expected output: "FireAirWater"

console.log(elements.join('-'));
// Expected output: "Fire-Air-Water"
```

  ## Mutating data:
  In JS certian values behave differently than certian other values that we might think are similar
 ```javaScript
let abcArray = ["a", "b", "c"];
abcArray[1] = "d";
abcArray;  // ['a', 'd', 'c']

let abcString = "abc";
abcString[1] = "d";
abcString; // 'abc'
  ```

### mutable vs. immutable🍀:
*"Mutable"* data can be edited (e.g. Arrays)

*"Immutable"* data always stays the same (e.g. strings & other primitives)


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e071c5a0-effa-4fcb-835b-6fbac58e8cd0" width="555">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/6e42302d-8eb6-418b-afd5-87ffa8a04517">
<br>


> ###  **See this** 💥
> Some actions "**mutate**" an array (e.g. `oldArray.push(newValue)`)
> aka(called) change the array ***in-place***
> Other actions **do** ***not* mutate** the original array, but instead create a new copy (e.g. `oldArray.concat(otherArray)`)


   <br>

### Variables themselves can also be (im)mutable 🌟 

```javaScript
let letVariable = "original value";
letVariable = "new value";

const constVariable = "original value";
constVariable = "new Value";
```
<br>

### Immutable variable with mutable value 💡
What happens when we use const with a mutable value like an array?
```javaScript
const operands = [4, 6];
const sum = operands[0] + operands[1]; //  10

operands[0] = 5;
const newSum = operands[0] + operands[1]; // 11
```

<br>
<br>

> ###  Advises:📌
> 1.  If you have the choice keep thing immutable
> 2.  The default for array is const unlees you have a good reson to use let      

<br>

### Copying an array: ✏️

```javaScript
let array1 = [1,2,3,4]
let array2= array1
array1[0]=5

array1 // [5,2,3,4]
array2 // [5,2,3,4]

// Even if I used const >> the same result
```

   <br>
   <br>

## **Objects:** 🌞
### The Object type represents one of JavaScript's data types. It is used to store various keyed collections and more complex entities. Objects can be created using the Object() constructor or the object initializer / literal syntax.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/d1bbdf69-0e70-45fe-820d-8b7c6ace94a5" width="555">


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/651285f0-c4f9-448e-b723-55ba9572e979" width="444">

- Objects collect multiple values together to describe more complex data
- Similar to how we can point at different values using variables in our code,
- objects let us point at related values using properties in the object.
- We can access edit and add any property using "."
- everything in javascript not a primitive type it is an object e.g array is a special kind of object

```javaScript
const js = {
    name: "JavaScript",
    abbreviation: "JS",
    isAwesome: true,
    officialSpec: "ECMAScript",
    birthYear: 1995,
    learn:false
    creator: "Brendan Eich"
};
```
Getting property values:`js.name`

Edit  property `js.learn = true`

Using property values `js.name.startsWith("Java")  ,  let age = 2022 - js.birthYear;`

Setting property values
```javaScript
const indecisive = {
    lunch: "sandwich"
};
indecisive.lunch = "tacos";
indecisive.snack = "chips";
```

### Feezing an object: 🥶❄️:
trick in JS, to essentially freeze an object in place and make it **immutable**,
and never be able to change from how it was when it was declared.

```javaScript
const obj = {
  prop: 42,
};

Object.freeze(obj);

obj.prop = 33;
// Throws an error in strict mode

console.log(obj.prop);
// Expected output: 42
```

### Methods🌌✨:
Properties can point to functions too. We call function-properties "methods" on objectsCopy
```javaScript
const dog = {
    name: "Ein",
    breed: "Corgi",
    speak: function () {
        console.log("woof woof");
    }
}
dog.speak();
```
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/90ea592d-0f02-4a18-85af-3593114f64a2" width="555">



<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c6185ddb-5b04-458c-a32a-0f3970c37517">






> ###  This:⚠️⚠️⚠️
> Its behavior is complicated & can be tricky
> A function's this keyword behaves a little differently in JavaScript compared to other languages. It also has some differences between > strict mode and non-strict mode.
> In most cases, the value of this is determined by how a function is called (runtime binding). It can't be set by assignment during  
> execution, and it may be different each time the function is called. The bind() method can set the value of a function's this 
> regardless of how it's called, and arrow functions don't provide their own this binding (it retains the this value of the enclosing 
> lexical context).
```javaScript
const test = {
  prop: 42,
  func: function () {
    return this.prop;
  },
};

console.log(test.func());
// Expected output: 42
```

### Built in objects:🗝️
1. document
2. array
3. console : has methods : log, error 
4. Math
5. Function

   <br>
   <br>




### const for things that stay the same, and use let for things that can change.







<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/90ea592d-0f02-4a18-85af-3593114f64a2" width="555">



<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c6185ddb-5b04-458c-a32a-0f3970c37517">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4ccf3d62-bbe1-42e9-bb93-235dcb530c33">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/01071bd8-4db0-4f2f-8a74-27308707568f" width="555">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c1471bff-fe04-4516-84cf-8e3c00ec21fd">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/31deac27-84da-428e-9027-d045b823f18c">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/7e738fb0-f13e-41f6-8335-d3d11cc1f4d5" width="344">
حل السؤال التاني
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/20130ee9-1270-49a4-98ea-125077f034fe width="333"">

### The Math namespace object contains static properties and methods for mathematical constants and functions.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3c13e466-b453-44d6-af1f-71189cec06e7" width="444">

# Exercises::::
# 1
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4f351e3e-c47a-4312-92cf-e0ab185e0156">

# 2

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/cd5d097a-e10a-4a88-9f4f-091bea31c947">

# 3
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/bf886f23-5c69-41af-a2a9-cd3c6518bd05">

# 4
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/7b79e68a-efb4-418a-bead-75a61ff92290">

# 5
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/650de9c9-717c-41d3-b6ac-16980d152126">

# 6

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/5e4272f6-6dfb-4d91-8cbb-e2d2ffccbddf">




























