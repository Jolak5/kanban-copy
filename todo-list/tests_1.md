# Testing To Do list: part 1

## Learning objectives
- Write unit tests for a JavaScript app.

### Estimated time: 3h

## Description
In this project you will write unit tests for the To Do list application. The testing project has been divided into two parts. In part 1 you will test functions responsible for adding and deleting list items. In part 2 you will test the status and content updates as well as the order re-position of items in the list.

*IMPORTANT NOTE: Read **all** requirements before you start building your project.*

### General requirements

- Make sure that there are [no linter errors](https://github.com/microverseinc/linters-config).
- Make sure that you documented your work [in a professional way](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/documentation/articles/professional_repo_rules.md).

### JavaScript requirements
  - Follow our list of [best practices for JavaScript](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/javascript_best_practices.md).

### Project requirements

- This is a pair-programming project. Please decide whose project will you use for testing.
- Use jest framework for testing.
- Create a test file (`[..].test.js`) for a file containing the **add item** and **delete item**  functions that you want to test.
- Take a look at each of these functions. Are they *pure functions*? If the answer is "yes" then writing tests for them should be straightforward. Some of those functions however will update *localStorage* and manipulate the *DOM*. For those, you will need to use mocks:
  - Mock a storage object to "imitate" localStorage operations (only if you are using `jest < 24.x`, in newer versions localStorage is mocked automatically).
  - Mock HTML to test if add/delete functions add or remove exactly one `<li>` element to/from the list in the DOM.
- Make sure you group your tests using the `describe()` method.


### Optional requirement

- Add a `--coverage` flag to your test script in *package.json*. That way you will see the percentage coverage of your application code every time you run a test:
```javascript
    ...
    "scripts": {
        "test": "jest --coverage",
        ...
    }
    
```
When writing tests the closer you get to 100% coverage the better.

### Need a big picture? 

Remind me about [the big picture of this project](./sneak_peek.md).


## Work and submission mode

- You should implement the above requirements only in **one repository** in your pair-programming group.
- You should ask for a review and submit this activity **on behalf of your pair-programming group.**

## Code review

Follow [these steps](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/code-review/articles/how_to_ask_for_a_code_review.md) to request a code review of your project.

## Submit your project

After the final approval from a code reviewer, you need to submit your project.
[Read this FAQ for a reminder on how to submit your project.](https://microverse.zendesk.com/hc/en-us/articles/360061344234)
Now go to your Student Dashboard and submit your project.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
