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





