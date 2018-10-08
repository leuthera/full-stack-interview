<h1 align="center">
JavaScript Interview Questions & Answers
</h1>
<p align="center">
    <img src="https://github.com/monkey3310/full-stack-interview/blob/master/assets/js-logo.svg" alt="JavaScript Interview Questions & Answers" width="200"/>
</p>

_Note: Keep in mind that many of these questions are open-ended and could lead to interesting discussions that tell you more about the person's capabilities than a straight answer would._

### 1. Explain how `this` works in JavaScript
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

A function's `this` keyword behaves a little differently in JavaScript compared to other languages. It also has some differences between strict mode and non-strict mode.

In the **global execution context (outside of any function)**, `this` refers to the global object whether in `strict mode` or not.

**Inside a function**, the value of this depends on how the function is called.
    Explain _arrow functions_ this, `bind` method

As an `object method` its `this` is set to the object the method is called on.

###### References
* [MDN web docs / this](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)
</details>

### 2. What is the difference between `let` and `var` and `const`?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

The most difference is scoping.
var - declaration which gets hoisted inside a function block
let - declaration which is scoped to a enclosing block e.g. if () { scope }
const - declaration which cant be altered afterwards

</details>

### 3. What is `===` operator?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

This is the strict comparision operator e.g. 5 == '5' = true vs 5 === '5' = false

</details>

### 4. List out the different ways an HTML element can be accessed in a Javascript code.
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

Access one element: document.getElementById('id'), document.querySelector('#id') returns first matching node, old vs new selector interface, should be faster, but depends on browser implementation, querySelector can take any css-selector and is more comfortable

Access one and more: document.getElementsByClassName(classname), document.querySelectorAll('.classname') returns a non-live NodeList (array-like list of elements, some functions are missing like push(), pop()).

</details>

### 5. What does a `typeof` operator do?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 6. What is the difference between Local Storage and Session Storage?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 7. What is the difference between null and undefined?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 8. What are anonymous functions in Javascript?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 9. What is a function callback?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 10. What is the difference between innerHTML and innerText?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 11. What is the difference between HTMLCollection and NodeList?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 12. What is an Event Bubbling in Javascript?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 13. What is NaN in Javascript?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>
</details>

### 14. Which Test-Libraries do you use?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

q-unit, mocha, chai, sinonJS, jasmine, ...

</details>

### 15. What is Hoisting?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

Means that you can use functions and "var"-s before you declare them

</details>

### 16. What means "use strict"?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

Switches to strict mode which helps to prevent common errors like using unsafe operators

</details>

### 17. When to use .bind()?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

To switch the context of an method e.g. fn.bind({context_member:1})(args)

</details>

### 18. Explain higher order function?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

Function that will take a function as rgument or return a new function

</details>

### 19. Explain map, filter, reduce and when to use it?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

map - to iterate over an array and return a new one
filter - to filter an array and return a new filtered one
reduce - to do what ever you want with an array and return whatever you want, e.g. filter some values and summarize them

</details>

### 20. When to use event delegation?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

If you have to watch a lot of elements and performance is key

</details>
