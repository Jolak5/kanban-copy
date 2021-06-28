# ES6 what is it about?

## Learning objectives

- Learn how to use proper ES6 syntax.
- Understand improvements that ES6 brings to JavaScript.

### Estimated time: 2h

## ECMAScript 6 (ES6)
The official name of JavaScript is ECMAScript (ES for short). Until 2015, subsequent versions of ES were numbered consecutively with integers, but starting with version 6 the creators decided to name new versions of ES using the year of publication instead of integers.For this reason you may come across the name ES2015 used interchangeably for ES6.

### Why is it important?
The sixth edition of ES has brought many excellent solutions and improvements to the language. Transpilers, *shim*, and *polyfill* libraries paired with the dynamic development of browsers mean that programmers can very quickly use all the possibilities that JavaScript now has to offer, making it one of the most popular programming languages in the world.

### `let`, `const` and *block scoping*
One of the most fundamental ideas of any programming language is **scope**. Each variable declared by the programmer lives in some scope. Before ES6, JavaScript used one keyword to declare variables - `var` - and two main scopes where variables lived:
- *global* scope.
- *function (local)* scope.

Among other new syntax changes, ES6 introduced two new keywords for variable declarations - `const` and `let`. It has also introduced *block level scoping* for variables declared with those new keywords. Correctly declaring variables is absolutely essential for any application. Understanding how scope and the new keywords work will make your code more resilient to unexpected errors and unwanted behavior.

To learn these concepts:
- [Read about *scope*](https://dev.to/sandy8111112004/javascript-introduction-to-scope-function-scope-block-scope-d11).

- [Read about  `const`, `let` and how it differs from `var`](https://dev.to/sandy8111112004/javascript-var-let-const-41he).

### Arrow functions
Another new feature introduced in the 6th version of EcmaScript is the **arrow function**. It has a new, shorter syntax, but most importantly, it has no `this` of its own. Problems with binding `this` in traditional JavaScript functions were the main reason for the introduction of the arrow function in ES6. We now have a new  powerful and predictable way to write and use functions in our applications.

- Read about the [*arrow functions*](https://www.w3schools.com/js/js_arrow_function.asp).
- [Watch this short video](https://youtu.be/NAN7U3MrX6o) to familiarise yourself with them.

### `Promise`s 
`Promise`s are a new, reliable intermediary between our calling function and our async code. We can think of them as *future value* containers. 
`Promise`s represent an important step in the development of asynchronous programming in JavaScript. They introduce order and guarantee the predictability of events.

- Read about [creating and using promises](https://javascript.info/promise-basics) in ES6.

### *Spread* and *destructuring*
ES6 introduces a new operator `...` (*spread*) and a new syntactic capability called *destructuring*. Both concepts quickly caught on in the JavaScript community and became an integral part of most modern applications.
Among the many other benefits of using the *spread* operator, it allows you to easily apply the concept of "immutability", which is crucial when building larger applications and has become the basis of libraries such as ReduxJS.
Destructuring, in turn, has become the primary syntax for writing *hooks* in the popular React library. Understanding both concepts is essential today for JavaSript developers.

To familiarise yourself with these concepts:
- [Read about *spread* operator](https://www.geeksforgeeks.org/javascript-spread-operator/).
- [Read about *destructuring*](https://javascript.info/destructuring-assignment).

## Challenge yourself
Check your understanding of this lesson. Try answering the questions below and then run the code snippets in the console to see if you got the answers right.

- Question 1 - What is the output of each of the console log?
```javascript
var color = "red";
let animal = "dog"
{
    var color = "blue";
    let animal = "cat"
    
    console.log(`log 1 - color: ${color}`);
    console.log(`log 2 - animal: ${animal}`);
}
console.log(`log 3 - color: ${color}`);
console.log(`log 4 - animal: ${animal}`);
```
- Question 2 - What is the output of the console log?
```javascript
const pr = new Promise(function(resolve,reject){
    setTimeout(() => resolve("foo"), 1000);
    setTimeout(() => resolve("bar"), 500);
})

pr.then(
    res => {
        console.log(res);
    },
    err => {
        console.log(err);
    }
)
```

## Additional materials
*These are all optional, but if you're interested in exploring this topic further, here are some resources to help you. Any exploration here should be done outside program time.*

In this lesson, we've covered only the most commonly used new ES6 features. For some, such as *class* or *modules*, we have created separate lessons because they are more complex and require more detailed study. Others, however, will not be discussed in detail because their use is too specific and you probably won't need them at this stage of learning.
But if you want to get familiar with all the new features of ES6 then [look through the ES6 documentation here](http://es6-features.org/).

You can also bookmark [this cheet sheet](https://devhints.io/es6) for future reference.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
