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
const is a signal that the identifier won’t be reassigned. It needs initialisation upfront, so you can't write const something;

let, is a signal that the variable may be reassigned, such as a counter in a loop, or a value swap in an algorithm.

var is now the weakest signal available when you define a variable in JavaScript. The variable may or may not be reassigned, and the variable may or may not be used for an entire function, or just for the purpose of a block or loop.
It's declaration is hoisted, instead of let and const.

```
for ( var i=0; i<2; i++ ) {} console.log(i) // exists outside the blockscope
for ( let i=0; i<2; i++ ) {} console.log(i) // only exists inside the blockscope
for ( const i=0; i<2; i++ ) {} console.log(i) // error reassignment, but only on top-level
for ( const cnt={i:0}; cnt.i<2; cnt.i++ ) {} // only exists inside the blockscope
```

</details>

### 3. What is `===` operator?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

This is the strict comparision operator e.g. 5 == '5' = true vs 5 === '5' = false, this means that it checks the value and also the type, so that Int 5 isn't equal a Str 5.
</details>

### 4. List out the different ways an HTML element can be accessed in a Javascript code.
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

Access one element:
```
    let byID = document.getElementById('id');
    let qS = document.querySelector('#id');
```
They return the first matching node. querySelector is the new selector interface, should be faster, but depends on browser implementation. querySelector can take any css-selector and is more comfortable.

Access one and more:
```
    let byClass = document.getElementsByClassName(classname);
    let qSA = document.querySelectorAll('.classname');
```
They return a non-live NodeList, which is an array-like list of elements, array-like means that some functions are missing like push(), pop()).

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

Means that the declaration moved to the top of the current scope (current script or the current function). JavaScript only hoists declarations, not initializations.

let and const don't get hoisted.
</details>

### 16. What means "use strict"?
:star: _Junior_
<details>
    <summary>
        Answer
    </summary>

Switches to strict mode which helps to prevent common errors like using unsafe operators

</details>

### 17. What is bind() and when we use it?

:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

bind is a method to bind the current context for later execution e.g.
```
element.addEventListener('click', this.onClick.bind(this), false);
```
it creates a new function which prevents accidental loss of scope. An alternative approach is to use apply, call or ES6 fat-arrow function.

</details>

### 18. Explain higher order function?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

Function that will take a function as argument or return a new function. For example [].map/filter/reduce are higer order functions.

</details>

### 19. Explain map, filter, reduce and when to use it?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

map - to iterate over an array and return a new one
filter - to filter an array and return a new filtered one
reduce - takes and reducer function which evaluate against every element and can produce every desired output (filter, map or simple value like sum)
</details>

### 20. When to use event delegation?
:star: _Senior_
<details>
    <summary>
        Answer
    </summary>

If you have to watch a lot of elements and performance is key

</details>
