# JavaScript classes

## Learning objectives
- Use JavaScript classes

### Estimated time: 2h

## Description 

In this lesson, you will learn about JavaScript classes, how to use them, their syntax, relationship, and differences with objects and functions.

### Why are classes important?

Classes are one of the foundations of Object Oriented Programming. JavaScript doesn't have built-in classes, but it supports classes in a particular way, using objects, and a new class *syntax* was introduced with EcmaScript 6 (you'll learn more about ES6 later in this same module).

### Classes and objects

JavaScript classes are not objects, they are *templates* for objects, it means that behind the scenes they will create objects. To create them you can use:
- [JavaScript Object Constructors](https://www.w3schools.com/JS/js_object_constructors.asp) (a function!)
- Or, the new [class](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) keyword

### Class methods and the Constructor method

A class may have several *methods*, which are again just functions! And they can have a special method called `constructor` that will be executed automatically when creating an instance of that class, useful for initialization. For more information, take a look at this links:

- [W3Schools JavaScript classes](https://www.w3schools.com/js/js_classes.asp)
- [MDN Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes#constructor)


### Classes and the *this*

The `this` keyword in JavaScript is a complex concept to grasp since its value changes depending on several factors. The `this` is present in classes, objects, and functions. Take a look at the following links:

- [This in Class Context](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this#class_context)
- [The JavaScript this Keyword](https://www.w3schools.com/Js/js_this.asp)

## Additional materials

Classes are a controversial topic in JavaScript. Some people argue that they are just *syntactic sugar* for prototype-based inheritance, and therefore they should be avoided; while others love classes for their simplified, beautiful syntax, and also think they are not just syntactic sugar but a useful new feature of the language.

Take a look at this [StackOverflow discussion](https://stackoverflow.com/questions/36419713/are-es6-classes-just-syntactic-sugar-for-the-prototypal-pattern-in-javascript)