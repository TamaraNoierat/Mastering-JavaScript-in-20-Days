# Classes & Prototypes
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/205743f1-3d73-47f5-9f7c-7ab354270cc3">



<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/1e8f2382-7828-4f70-a53f-191744ca837a">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/2505f995-3750-491c-be87-45d22c6faa44">


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/c601bba3-2c86-4315-917e-921c32ddd1b5">

 Using the prototype chain
Store the increment function in just one object and have the interpreter, if it
doesn't find the function on user1, look up to that object to check if it's there
Link user1 and functionStore so the interpreter, on not finding .increment, makes
sure to check up in functionStore where it would find it
Make the link with Object.create() technique

#### the code must be :
1. Easy to reason about
But also
2. Easy to add features to (new functionality)
3. Nevertheless efficient and performant
The Object-oriented paradigm aims is to let us achieve these three goals

============================
Using the prototype chain
Store the increment function in just one object and have the interpreter, if it
doesn't find the function on user1, look up to that object to check if it's there
Link user1 and functionStore so the interpreter, on not finding .increment, makes
sure to check up in functionStore where it would find it
Make the link with Object.create() technique


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/def4b392-261a-48a8-bcc6-7b2ec77fb192">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/a72c5691-1ef2-4fe2-b3b2-692aeb41546a">


##### What if we want to confirm our user1 has the property score?

We can use the hasOwnProperty method - but where is it? Is it on user1?
All objects have a __proto__ property by default which defaults to linking to a big
object - Object.prototype full of (somewhat) useful functions
We get access to it via userFunctionStore’s __proto__ property - the chain


<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/adbc88c6-4db4-4a54-9ed9-0b260692aad1">

<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/f5ae4c76-8e32-46a2-8a1d-56923f48f8fb">
=====================================
<img src="https://github.com/TamaraNoierat/Mastering-JavaScript-in-20-Days/assets/130704887/67740232-dd57-4339-ba25-b98e7f10ab27">
It creates a user named "Will" with a score of 3.
It creates another user named "Tim" with a score of 5.
It tells the first user (Will) to increase the score. This works because of the arrow function trick. So, Will's score becomes 4


===================================================
















