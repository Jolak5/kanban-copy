# Async

## Learning objectives

- Use callbacks and promises.
- Describe the difference between async and sync calls.

### Estimated time: 2.5h

## Description

In this lesson, you will learn what are sync and async calls in JavaScript, when and how to use them.

### Sync vs async

**Synchronous** (sync) code is executed instruction by instruction, one by one, blocking the execution of the program until each step is completed before moving to the next one. Most operations in JavaScript are synchronous.

But sometimes, for several reasons, you don't want to wait until an instruction has finished, for example, because you are performing a request over the internet (like sending or receiving data from/to a server) and you don't know how much time this operation may take. In this case, you want to continue with the next operation and be notified in the future when the previous one has finished. **Asynchronous** (async) calls allow you to do that, start an operation, and do other things while you are *waiting* for the previous one to finish.

JavaScript has several ways to perform async operations:

- [Callback functions](https://www.w3schools.com/js/js_callback.asp)
- [Promises](https://www.w3schools.com/js/js_promise.asp)
- [Async functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function)

Callback functions are the traditional way of dealing with async code, while promises and async functions are newer additions to the language. You should be familiar with all of them since you will find them in different projects.


## Additional materials
**These are all optional, but if you're interested in exploring this topic further, here are some resources to help you. Any exploration here should be done outside program time.**

To get a deeper understanding of how JavaScript async code works, read this articles:

- [JavaScript Promise Tutorial: Resolve, Reject, and Chaining in JS and ES6](https://www.freecodecamp.org/news/javascript-es6-promises-for-beginners-resolve-reject-and-chaining-explained/).
- Be careful, avoid the [callback hell](https://www.freecodecamp.org/news/how-to-deal-with-nested-callbacks-and-avoid-callback-hell-1bc8dc4a2012/) and [promise hell](https://medium.com/@pyrolistical/how-to-get-out-of-promise-hell-8c20e0ab0513).
