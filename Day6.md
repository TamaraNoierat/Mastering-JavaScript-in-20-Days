# sixth Day :


# Data Fetching && Promises:

### APIs (Application Programming Interfaces)

 #### APIs provide special website addresses (URLs) that lead us to the specific data we want. These URLs are like doors to the information we're interested in. When we open these doors (by sending requests), the API gives us the data we asked for. It's like asking for a menu at a restaurant – you tell them what you want, and they bring it to you. APIs do something similar but with data on the internet.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/59dc63ec-8643-4212-bd40-5a5548003687">

#### fetch() lets us use JS to load data from APIs  fetch("https://dog.ceo/api/breed/hound/list")

#### JSON stands for "JavaScript Object Notation." It's a way to organize and share information that computers can easily understand. Imagine it as a simple language that both computers and humans can read. It's often used to exchange data between different programs or to store data in a format that's easy to work with. Think of JSON as a structured recipe that computers can follow to understand and use data.

###### is a standard text-based format for representing structured data based on JavaScript object syntax. It is commonly used for transmitting data in web applications

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3fc86f8b-67d7-406f-bddd-37f3ad98e584">

#### fetch() in JavaScript is like sending a request to a website to get some information.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/97fe27c5-e65f-4d8e-9f34-7b854c9e9426" width="433">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/47356782-d52d-4f55-bf82-7d48a77157c7" width="444">

## Promises:💣

It takes time to fetch data from the network, So JS writes us an "IOU" for the data value it doesn't have yet aka a **Promise** of a value
```javaScript
>> fetch("https://dog.ceo/api/breed/hound/list")
Promise { <state>: "pending" }
```

Promises can be in 3 possible **states**:
- **pending**: still waiting for the value, hang tight
- **fulfilled** (aka "resolved"): finally got the value, all done
- **rejected**: sorry couldn't get the value, all done, It takes time for Promises to resolve, so they are "asynchronous"
- 

### a promise in JavaScript is like a special container for something that will happen later. It's used when you're doing things that take time, like getting data from a website. The promise says, "I promise to give you the data when it's ready." Once the data is ready, you can use it in your code. It's a way to manage tasks that need some time to finish.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b3878943-387a-4c2e-995a-b9ef67366960">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/d87a5433-fe73-456f-abd1-a1e65dea6fae" width="555">
fetch("url"): This part of the code is making an HTTP request to the specified URL. It's asking the server at that URL to send some data back. The fetch function returns a promise that represents the response from the server.

await: The await keyword is used in front of the fetch function. It tells JavaScript to wait until the promise returned by the fetch function is resolved (the response is received) before moving on to the next line of code.

let response: This declares a variable named response to store the result of the fetch operation. Once the promise is resolved, the actual response from the server will be stored in this variable.

response have a method called JSON:
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/4bce8bb9-0d20-4fba-82b8-ef17340926d5">

let response = await fetch("url");
let data = await response.json();
##### In this code, after making a fetch request and receiving a response, the .json() method is used to convert the response body (which is in JSON format) into a JavaScript object. This makes it much easier to interact with the data and access its properties.



### await

**await** lets us tell JS to stop and wait for an asynchronous operation to finish

> In the case of a Promise, it waits for it to resolve before continuing with our code
> ```javaScript
> let response = await fetch("https://dog.ceo/api/breed/hound/list");
>   console.log(response);
> ```
 The Promise we get from fetch() resolves to a Response object
 It's body contains the data we care about

 Calling the **.json()** method on the response parses its body as a JSON object `response.json()`
  awaiting the JSON Promise too, because .json()returnspromises
  ```javaScript
let response = await fetch("https://dog.ceo/api/breed/hound/list");
let body = await response.json();
```
# Destructuring
###  destructuring : is like picking out the parts you need from a collection of data, making your code cleaner and more focused.

is a fancy way of declaring multiple variables at once
By "extracting" values from an object with their property names `let {name, nickname} = spices[0];`
- If we only care about some of the properties, we can omit the others`let {nickname} = spices[2];`
- We can also destructure Arrays, assigning variables for their items`const [baby, ginger, scary, sporty, posh] = spices;`
- We can ignore the values in the array we don't need use commas to "skip" values`const [,,melB] = spices;`
- use ... to collect remaining values`const [babySpice, ...adultSpices] = spices;`
### Exercise: 👩🏻‍💻
```javaScript
let a, b, rest;
[a, b] = [10, 20];
console.log(a);
// Expected output: 10
console.log(b);
// Expected output: 20
[a, b, ...rest] = [10, 20, 30, 40, 50];
console.log(rest);
// Expected output: Array [30, 40, 50]


#  ex:
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 30,
};
const { firstName, age } = person;


## async functions 🔥

If we try to await something in a regular function...
```javaScript
⭕⭕⭕⭕⭕⭕XX JS doesn't allow it
function fetchResponse(url) {
    const response = await fetch(url);
    return response;
}
```
We need to make it an async function. This tells JS to expect to await async operations inside the function
```javaScript
async function fetchResponse(url) {
    const response = await fetch(url);
    return response;
}
```


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/e09e4a76-e3bb-47d4-bb58-73723bef3449" width=""355>

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3cf41759-c92d-4b84-bea5-93f8efea0e91" width="455">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8ebf8a06-55ae-40c8-84a7-689f0f709d8a" width="455">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/6d2ee08c-c9a0-4f18-b6f9-0a7ba15bb11e" width="344">
شرح الصورة في الاعلى 
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/649e253f-801c-4de2-ab7a-7dc16b6455be" width="355">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/89586cd3-bdc9-4e62-b145-3fbc4193ff6f" width="355">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/798d7710-2c94-4e32-a8ac-fe8db1ebc4c8" width="455">
شرح الصورة::
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/8c8413b5-4a58-444f-a7a3-b0e63ebccd58" width="455">




### Modules🔥
 let us split big codebases across multiple files


 ```javaScript
<script type="module">
    //...
</script>
```
 JS modules work **differently** from JS scripts
1. One difference is that we can't use await outside of a function in a script
```javaScript
<script>
    await fetch("https://dog.ceo/api/breed/hound/list");
</script>
```
2. Module scope
modules create their own scope, Try loading the page and accessing the BREEDS variable we declare in the module
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/79b5475d-f2b2-4efc-a308-28712bcf3fe4">
<imd src="![image](https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/fdced6b3-3ad7-4800-862c-03c1c95b130f">


### import && export
- **export** lets us expose variables from our module's scope to the outside world
- **import** lets us use an exposed variable from another module

## Debugging: ✏️📋
We can console.log() (or .warn() or .error()) is one way to understand what's happening when your program runs

```javaScript
function whyIsntThisWorking(input) {
    console.log("Well at least we got this far");
    console.log(input);
    return thingThatDoesntWork(input);
}
```

You can also use the browser's debugger to pause JS and inspect what's happening

```javaScript
function whyIsntThisWorking(input) {
    debugger;
    return thingThatDoesntWork(input);
}
```
The debugger statement creates a breakpoint where JS will pause and let you look around

## Error handling 🔥🌠
Once we've discovered where in our program an error is likely, we can do something about it!
Usually errors will cause JS to stop running our code
  
**try** lets us "watch out" for potential errors
its friend **catch** lets us manage errors when they occur
```javaScript
try {
    thisMightThrowAnError();
} catch (error) {
    console.error("As if! Error:", error); 
    console.log("Whatever, let's press on anyway");
}
console.log("still rollin' with the homies");
```



































