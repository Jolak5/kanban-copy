# Testing To Do list: part 1

## Learning objectives
- Write units tests for a JavaScript app

### Estimated time: 3h

## Description
In this project, you will write unit tests for the To Do List application. Testing has been divided into to two parts. In part 1 you will test functions responsible for adding and deliting items to the list. In part 2 you will test the status and content updates as well as the order re-position of items in the list.

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
- This is a pair-programming project. Please decide whose project will you use for testing.
- Create a test file (`[..].test.js`) for a file containing your **add item** and **delete item**  functions you want to test.
- Take a look at each of these functions. Are they *pure functions*? If the answer is "yes" - writing tests for them should be straightforward. Some of those functions however will update *localStorage* and manipulate *DOM*. For those, you will need to use mocks.
  - mock a storage object to *imitate* localStorage operations
  - mock HTML to test if add/delete functions add or remove exactly one `<li>` element from the list in the DOM 
- Make sure you group your tests using the `description()` method.
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
