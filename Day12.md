#### You don't deal with these type conversion corner cases by avoiding coercions.

#### JavaScript's dynamic typing is not a weakness, it's one of its strong qualities:
means that the dynamic typing feature in JavaScript is not a drawback or weakness; instead, it is considered one of the language's strong and valuable features.

#### The statement "Implicit != Magic in js" is emphasizing that just because something happens implicitly in JavaScript doesn't mean it's a magical or mysterious process. Implicit behaviors, like type coercion, are well-defined and follow certain rules. While they might not be immediately obvious, they are not beyond comprehension.

#### "hiding unnecessary details, re-focusing the reader, and increasing clarity" can be applied to code and programming practices to make your code more readable, maintainable, and understandable. Here's how these principles can be applied in JavaScript.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/1f6a933a-c4fc-4949-a972-2f25f6a339f5" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3afa762e-1f3e-4f25-890e-4c9b5296fb96" width="355">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e405efae-2cbf-4dad-9aa4-b83c1268e97c" width="355">


#### Equality        == vs. ===
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e7ea4eea-6191-4d01-8579-2ce5b9dc6206">

#### 1-Loose Equality (==): When you use ==, JavaScript tries to make things equal by changing their types if needed. For example, it might treat a number and a string that look the same as equal, even if they're not exactly the same type.
####  2-Strict Equality (===): With ===, JavaScript only says things are equal if they have the same value and the same type. It doesn't try to change the types to make them match.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/29b2ad7d-7316-4030-a88b-9ce12f2be145">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/67434f2b-b739-4c33-a0fa-2433ea0cb067">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4845d076-e21e-4352-beba-1c09c8aa94eb">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4c489116-dc9e-4d99-9260-57863c681d98">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4e2e0130-8b43-4b49-bdd3-d7b0b9ac920a">




## 1. If the types are the same: Use ===

If you're comparing two things that are the same type, like two numbers or two strings, use ===. It's like asking if they're exactly the same, both in value and in what they are.

## 2. If null or undefined: They're equal

If you're comparing something to null or undefined, they're considered equal if you use ==. It's like saying, "Yeah, these are both nothing."

## 3. If non-primitives: Convert them to simpler form

For things that aren't simple numbers or strings, JavaScript tries to make them simpler before comparing. It's like trying to explain something complex in a simpler way.

## 4. Prefer: Convert to Number

When converting things to simpler forms, JavaScript often tries to turn them into numbers if it can. This is usually safer and easier to understand than other conversions.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/07cb1475-1a01-461b-92b7-4fc6134ee3c5">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/00a2a293-b595-432f-9381-38f6c16b77e2">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/59e6793c-9a29-4bae-adbb-691693446758">



### 1. Avoid == with 0 or "" (or even " "):

When you use == with 0 or an empty string "", JavaScript can sometimes confuse them with each other or with false. So, it's better to use === instead. This way, you make sure you're checking for both the value and the type.

### 2. Avoid == with non-primitives:

When you use == with things that are not simple numbers or strings (like objects), JavaScript can do unexpected things. It tries to make them simpler, but it's better to use === to avoid surprises.

### 3. Be careful with == true or == false:

Using == true or == false with == can work, but it's often clearer and safer to use === or convert to boolean (!!) to show your intention more explicitly.


### *TypeScript and Flow both introduce static typing to JavaScript, helping catch type-related errors before your code runs.
### *TypeScript is a separate language that compiles to JavaScript, while Flow is a type checker that works with regular JavaScript.
### *Type-Aware Linting combines linting tools with type information to provide enhanced analysis of your code, improving code quality and catching errors more comprehensively.


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/347f2ad7-e673-432d-b30d-2c4bc092b057">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e95358af-ee86-4417-98e5-c45227aee54d">


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/42518a31-43e4-436f-b04c-33a7d7646a99">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3b6d8e30-c35d-4352-a566-3c20630c1e77">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3dc2958c-5089-4736-9b4c-6d2be649d797">


# Q1:
Given the following promisesArray, convert the array into an object using the convertToObj function.

You should apply typescript types to every promise, the input of convertToObj, and the output of convertToObj.

Build interfaces and types as needed.
## solution:

```
interface HelloWorldResponse {
  message: string;
}

interface CheckBooleanResponse {
  result: boolean;
}

interface ReturnObjResponse {
  x: string;
  y: number;
}

const sayHelloWorld = new Promise<HelloWorldResponse>((resolve, reject) => {
  resolve({ message: "Hello world!" });
});

const checkBoolean = (boolean: boolean) => new Promise<CheckBooleanResponse>((resolve, reject) => {
  if (boolean) {
    resolve({ result: boolean });
  } else {
    reject(`Input is false :(`);
  }
});

const returnObj = new Promise<ReturnObjResponse>((resolve, reject) => {
  resolve({
    x: "meow",
    y: 45,
  });
});

const promisesArray = [sayHelloWorld, checkBoolean(true), returnObj];

const convertToObj = async (array: Promise<any>[]) => {
  const obj: Record<string, any> = {};

  await Promise.all(array.map(async (promise, index) => {
    try {
      const result = await promise;
      obj[`promise${index + 1}`] = result;
    } catch (error) {
      obj[`promise${index + 1}`] = { error: error.message };
    }
  }));

  return obj;
};

(async () => {
  const resultObj = await convertToObj(promisesArray);
  console.log(resultObj);
})();
```

# Q2
What will be the output of the following code snippet? Pick the right choice then justify your answer with an explanation.
```
function testScope1() {
  if (true) {
    var a = 1;
    let b = 2;
    const c = 3;
  }
  console.log(a);
  console.log(b);
  console.log(c);
}

testScope1();
```
Choices:

A) undefined, undefined, undefined
B) 1, undefined, ReferenceError
C) 1, ReferenceError, ReferenceError
D) 1, ReferenceError


# Solution:
C) 1, ReferenceError, ReferenceError

# Q3
QUESTION #3:
What will be the output of the following code snippet? Pick the right choice then justify your answer with an explanation.
```
function testScope2() {
  console.log(a);
  console.log(b);
  console.log(c);
  if (true) {
    var a = 1;
    let b = 2;
    const c = 3;
  }
}

testScope2();
```
Choices:

A) undefined, ReferenceError
B) 1, undefined, ReferenceError
C)undefined, undefined, ReferenceError
D) 1, ReferenceError

## The correct choice is:

A) undefined, ReferenceError

# Q4:
QUESTION #4:
What will be the output of the following code snippet? Pick the right choice then justify your answer with an explanation.
```
function testScope3() {
  var a = 36;
  let b = 100;
  const c = 45;

  console.log([a, b, c]);

  if (true) {
    var a = 1;
    let b = 2;
    const c = 3;

    console.log([a, b, c]);
  }

  console.log([a, b, c]);
}

testScope3();
```
choices:

A) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 36, 2, 3 ]
B) [ 36, 100, 45 ] | [1, 2, 3 ] | [ 36, 100, 45 ]
C) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 1,100, 45 ]
D) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 1, 2, 3 ]

## The correct choice is:

A) [ 36, 100, 45 ] | [ 1, 2, 3 ] | [ 36, 2, 3 ]









