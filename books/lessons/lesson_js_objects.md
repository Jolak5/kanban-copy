# Working with objects

## Learning objectives
- Understand different ways to create objects in JavaScript.
- Create and access properties and methods of JavaScript objects.

### Estimated time: 1.5h

## Description

In this lesson, you will learn how to use JavaScript objects, how to create methods and properties, and how to access them.

### Why are JavaScript objects important?

In JavaScript, almost everything is an object! They are one of the data structures implemented natively by the language and they are fundamental to JavaScript programming. It is necessary to understand the different ways in which JavaScript objects work in order to write good JavaScript.

### Object creation

There are several ways to create objects in JavaScript, each one with small differences not only in syntax but also in the way you set the prototype and assign its properties. Take a look at the detailed documentation of each way (remember that your goal is to observe and understand the differences, not to read entire documentation):

- [Object *literal* notation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Object_initializer) (also known as *initializer* notation). This topic was already introduced in the [previous module](https://github.com/microverseinc/curriculum-html-css/blob/main/introduction_to_js_objects.md). 
- [Object() constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/Object).
- [Object.prototype.constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/constructor).
- [Object.create()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/create).
- [Object.assign()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign).

### Object prototypes

JavaScript is a multi-paradigm language and implements inheritance in its own way. Unlike other object-oriented programming (OOP) languages based on classes, like Java or C,  JavaScript uses **prototypal inheritance**.
 - Read [this article](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object_prototypes) to learn more about the object prototype.

### Object methods

Objects, as you already know, are collections of key/value pairs. The properties (keys), can have any value, including functions. When the properties contain function definitions they are called **methods**.
- Read about [defining methods in objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#defining_methods).

## Challenge yourself

You may have noticed that the `Object() constructor` and the `Object.prototype.constructor` ways of creating an object look similar. Take a deeper look and find the difference between the two of them. Hint: one of them seems like a function. As a matter of fact, you can use your own functions to create objects.

[Click here](lesson_js_objects_challenge.md) to check your answers to these questions.

## Additional materials
*These are all optional, but if you're interested in exploring this topic further, here are some resources to help you. Any exploration here should be done outside program time.*
- Read the article [How to create objects in JavaScript](https://www.freecodecamp.org/news/a-complete-guide-to-creating-objects-in-javascript-b0e2450655e8/) that summarizes the different ways of creating objects. Note that in this lesson we are not talking about *classes* - that's a topic that will be discussed in its own lesson.
- Learn more about [objects and object constructors](https://www.theodinproject.com/paths/full-stack-ruby-on-rails/courses/javascript/lessons/objects-and-object-constructors) in this article from The Odin Project.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
