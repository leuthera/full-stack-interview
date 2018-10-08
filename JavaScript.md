1.  [Beginner] What is the difference between "var", "let", "const" and what happen if you omit the declaration
    The most difference is scoping.
    var - declaration which gets hoisted inside a function block
    let - declaration which is scoped to a enclosing block e.g. if () { scope }
    const - declaration which cant be altered afterwards

2.  [Beginner] Explain at least two ways to select an ID-DOMElement, what are the differences
    document.getElementById('id'), document.querySelector('#id') returns first matching node, old vs new selector interface, should be faster, but depends on browser implementation, querySelector can take any css-selector and is more comfortable

3.  [Intermediate] What means tripple equal ===
    This is the strict comparision operator e.g. 5 == '5' = true vs 5 === '5' = false

4.  [Intermediate] Which Test-Libraries do you use
    q-unit, mocha, chai, sinonJS, jasmine, ...

5.  [Intermediate] What is Hoisting
    Means that you can use functions and "var"-s before you declare them

6.  [Intermediate] What means "use strict"
    Switches to strict mode which helps to prevent common errors like using unsafe operators

7.  [Advanced] When to use .bind()
    To switch the context of an method e.g. fn.bind({context_member:1})(args)

8.  [Advanced] Explain higher order function
    Function that will take a function as rgument or return a new function

9.  [Advanced] Explain map, filter, reduce and when to use it
    map - to iterate over an array and return a new one
    filter - to filter an array and return a new filtered one
    reduce - to do what ever you want with an array and return whatever you want, e.g. filter some values and summarize them

10. [Advanced] When to use event delegation
    If you have to watch a lot of elements and performance is key
