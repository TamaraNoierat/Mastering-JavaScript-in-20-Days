# Asynchronicity
JavaScript is:
- Single threaded (one command runs at a time)
- Synchronously executed (each line is run in order the code appears)

  ## setTimeout is a built in function - its first argument is the function to delay followed by ms to delay by
<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/755e7c0f-0529-4198-8ff2-5d52f9897440">

### JavaScript is not enough - We need new pieces (some of which aren’t JavaScript at all)

Our core JavaScript engine has 3 main parts:
- Thread of execution
- Memory/variable environment
- Call stack
We need to add some new components:
- Web Browser APIs/Node background APIs
- Promises
- Event loop, Callback/Task queue and micro task queue
- 
  <img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/0321994c-553c-4f8f-b1f4-778bee6a4972">
# Web API rules
URLs: APIs have special web addresses (URLs) for different tasks or data.

Actions: They use different commands like GET (get data), POST (add data), PUT (update data), DELETE (remove data).

Security: APIs require proof of identity (authentication) and permission (authorization) to use.

Format: Requests and responses follow specific formats for data and messages.
Limits: To be fair, APIs control how many requests you can make in a certain time.

Versions: As they change, APIs may have different versions for compatibility.

Errors: APIs give clear messages when things go wrong.

Sharing: If you use an API on a different website, some rules decide if it's allowed (CORS).

Data Style: Data is usually sent and received in simple formats like JSON or XML.

Guidelines: Good APIs have clear guides on how to use them, what they offer, and how to deal with issues.

## Callback and Event Loop
### Callback Queue
is a waiting area for completed tasks (callbacks) to be processed when their turn comes.
### Event Loop 
is like a manager that keeps checking the queue, picking tasks, and handling them one by one, allowing the program to stay responsive and manage different tasks smoothly.
### Both callback queue and the event loop are crucial concepts in asynchronous programming, which helps programs handle tasks that take time without freezing everything up.

************
## ES5 Web Browser APIs with callback functions


Our response data is only available in the callback function - Callback hell
- Maybe it feels a little odd to think of passing a function into another function only for it
to run much later
Benefits
- Super explicit once you understand how it works under-the-hood

## ES6+ Solution (Promises)

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/18298585-486d-4773-936b-b1fc5797e7e4">

Special objects built into JavaScript that get returned immediately when we make
a call to a web browser API/feature (e.g. fetch) that’s set up to return promises
(not all are)
Promises act as a placeholder for the data we expect to get back from the web
browser feature’s background work

### Problems
- 99% of developers have no idea how they’re working under the hood
- Debugging becomes super-hard as a result
- Developers fail technical interviews
Benefits
- Cleaner readable style with pseudo-synchronous style code
- Nice error handling process

  ### Non-blocking applications:
 This means we don’t have to wait in the single thread
and don’t block further code from running

### However long it takes: 
We cannot predict when our Browser feature’s work will
finish so we let JS handle automatically running the function on its completion
### Web applications: 
Asynchronous JavaScript is the backbone of the modern web -
letting us build fast ‘non-blocking’ applications

************
# Classes, Prototypes - Object Oriented JavaScript
1 Classes and Prototypes:
- Classes are blueprints for creating objects.
- Prototypes allow objects to inherit properties and methods from other objects.
- 
2 proto and prototype:
- --proto-- helps access an object's prototype directly.
- prototype is used to set the prototype for objects created by a constructor.
- 
3 new and class Keywords:
- new creates instances of objects.
-class is a modern way to define and create objects with methods.

***************
## Objects - store functions with their associated data!

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/1ec1110b-cb7c-40ee-a70e-68ea475ce005">

### The prototype chain enables efficient memory usage and supports the concept of "inheritance," allowing objects to share common behavior and avoid redundancy in property and method definitions. Understanding the prototype chain is essential for effective object-oriented programming in JavaScript.

### example:

<img src=" https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/49f16c4b-1477-4b9a-9eb2-ab996e778560">

## Declaring & calling a new function inside our ‘method’ increment

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/f1f5725b-e05c-4835-bffd-e9b37952ae5b">

In summary, when declaring and calling a new function inside a method, it's important to understand how the value of this is determined and ensure it's pointing to the right context, especially when you're accessing properties of an object.

## Arrow functions override the normal this rules

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/88e7916a-9594-4abc-b4ae-430fd41cc555">

#### Arrow functions are a powerful feature in modern JavaScript that make writing functions more concise, especially for simple operations. However, it's important to be aware of the differences in how this is handled compared to traditional function expressions, especially when using arrow functions as methods or in certain contexts.

************************
# Q1
## solotion:

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/0b20a54d-5c8e-4e5c-974d-5941f4c9e03c">



# Q2
## solution:

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/d5ad1076-7cea-4c57-a6d9-02398fa9dfdc">

# Q3
## solution:

<img src="https://github.com/mahaalqerem/Mastering-JavaScript-in-20-Days/assets/138065974/f397d9ae-a2b9-4e01-b01a-e08bdb59b45d">


