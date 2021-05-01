# Testing To Do list: part 1

## Learning objectives
- Write units tests for a JavaScript app

### Estimated time: 3h

## Description
In this project, you will write unit tests for the To Do List application you have already created. Your tests will cover all CRUD functions. 

*IMPORTANT NOTE: Read **all** requirements before you start building your project.*

### General requirements

- Make sure that there are [no linter errors](https://github.com/microverseinc/linters-config).
- Make sure that you documented your work [in a professional way](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/documentation/articles/professional_repo_rules.md).

### JavaScript requirements
  - Follow our list of [best practices for JavaScript](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/javascript_best_practices.md).

### Project requirements

#### Setup
Before you start writing tests we need to configure our project so that Jest can read ES6 modules. By default Jest uses CommonJS notation so we need to *transform* all modules into CommonJS notation. For that, we will use [**Babel** compiler](https://babeljs.io/).

Open a terminal in your project directory and execute:

```npm install --save-dev @babel/plugin-transform-modules-commonjs```

Then create a new file called: `.babelrc` and paste:
```javascript
{
  "env": {
    "test": {
      "plugins": ["@babel/plugin-transform-modules-commonjs"]
    }
  }
}
```
That's it! Now you can use `import` instead of `require` and write tests for all your ES6 modules.

#### Requirements

- Create a test file (`[..].test.js`) for a file containing your CRUD functions.
- Take a look at each of these functions. Are they *pure functions*? If the answer is "no" - try to refactor your code to make each CRUD function a pure one, by decoupling main data manipulation logic from DOM operations and `localStorage` operations.
For example - if your `addNewItem()` function pushes new item to array or updates the `localStorage`, change it - so it takes array and new item as arguments and returns a new array with concatenated value:
```javascript
const addNewItem = (tasksArray, newItem) => {
    return [...tasksArray, newItem]
}
```
Then you can use the returned value of `addNewItem()`, set it in local storage, and update the DOM in another function.
- Write a few tests for each of the pure functions for: 
    - add a task, 
    - remove a task, 
    - update task status, 
    - update task position
- Make sure you group your tests using `description()` method.
- Add a `--coverage` flag to your test script in *package.json*. That way you will see the percentage coverage of your application code every time you run a test:
```javascript
    ...
    "scripts": {
        "test": "jest --coverage",
        ...
    }
    
```


### Need a big picture? 

Remind me about [the big picture of this project](./sneak_peek.md).


## Code review

Follow [these steps](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/code-review/articles/how_to_ask_for_a_code_review.md) to request a code review of your project.

## Submit your project

After the final approval from a code reviewer, you need to submit your project.
[Read this FAQ for a reminder on how to submit your project.](https://microverse.zendesk.com/hc/en-us/articles/360061344234)
Now go to your Student Dashboard and submit your project.
