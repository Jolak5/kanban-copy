# JavaScript classes

## Learning objectives
- Use JavaScript classes

### Estimated time: 2h

## Description 

In this lesson, you will learn about JavaScript classes, how to use them, their syntax, relationship, and differences with objects and functions.

### Why are Javascript classes important?

Classes are one of the foundations of object oriented programming. JavaScript doesn't have built-in classes, but it supports classes in a particular way, using objects, and a new class *syntax* was introduced with EcmaScript 6 (you'll learn more about ES6 later in this same module).

### Classes and objects

JavaScript classes are not objects, they are *templates* for objects. That means that behind the scenes JavaScript classes will create objects. To create them you can use:
- [JavaScript object constructors](https://www.w3schools.com/JS/js_object_constructors.asp) (a function!).
- Or, the new [class](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) keyword.

### Class methods and the constructor method

A class may have several *methods*, which are again just functions! And a class can also have a special method called `constructor` that will be executed automatically when creating an instance of that class, which is useful for initialization. For more information, take a look at these links:

- [JavaScript classes](https://www.w3schools.com/js/js_classes.asp).
- [The constructor method](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes#constructor).

### Classes and the *this*

The `this` keyword in JavaScript is a complex concept to grasp since its value changes depending on several factors. The `this` is present in classes, objects, and functions. Take a look at the following links:

- [This in class context](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this#class_context).
- [The JavaScript this keyword](https://www.w3schools.com/Js/js_this.asp).

## Additional materials

*These are all optional, but if you're interested in exploring this topic further, here are some resources to help you. Any exploration here should be done outside program time.*

Classes are a controversial topic in JavaScript. Some people argue that they are just *syntactic sugar* for prototype-based inheritance, and therefore they should be avoided; while others love classes for their simplified, beautiful syntax, and also think they are not just syntactic sugar but are a useful new feature of the language.

Take a look at this [StackOverflow discussion](https://stackoverflow.com/questions/36419713/are-es6-classes-just-syntactic-sugar-for-the-prototypal-pattern-in-javascript) to learn more about both sides of this debate.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
