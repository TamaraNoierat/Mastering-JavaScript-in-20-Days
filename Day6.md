# Data Fetching && Promises:

### APIs (Application Programming Interfaces)

 #### APIs provide special website addresses (URLs) that lead us to the specific data we want. These URLs are like doors to the information we're interested in. When we open these doors (by sending requests), the API gives us the data we asked for. It's like asking for a menu at a restaurant – you tell them what you want, and they bring it to you. APIs do something similar but with data on the internet.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/59dc63ec-8643-4212-bd40-5a5548003687">

#### JSON stands for "JavaScript Object Notation." It's a way to organize and share information that computers can easily understand. Imagine it as a simple language that both computers and humans can read. It's often used to exchange data between different programs or to store data in a format that's easy to work with. Think of JSON as a structured recipe that computers can follow to understand and use data.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/3fc86f8b-67d7-406f-bddd-37f3ad98e584">

#### fetch() in JavaScript is like sending a request to a website to get some information.
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/97fe27c5-e65f-4d8e-9f34-7b854c9e9426" width="433">
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/47356782-d52d-4f55-bf82-7d48a77157c7" width="444">

### a promise in JavaScript is like a special container for something that will happen later. It's used when you're doing things that take time, like getting data from a website. The promise says, "I promise to give you the data when it's ready." Once the data is ready, you can use it in your code. It's a way to manage tasks that need some time to finish.

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/b3878943-387a-4c2e-995a-b9ef67366960">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/d87a5433-fe73-456f-abd1-a1e65dea6fae" width="555">
fetch("url"): This part of the code is making an HTTP request to the specified URL. It's asking the server at that URL to send some data back. The fetch function returns a promise that represents the response from the server.

await: The await keyword is used in front of the fetch function. It tells JavaScript to wait until the promise returned by the fetch function is resolved (the response is received) before moving on to the next line of code.

let response: This declares a variable named response to store the result of the fetch operation. Once the promise is resolved, the actual response from the server will be stored in this variable.






