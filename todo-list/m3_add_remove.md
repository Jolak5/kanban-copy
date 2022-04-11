# To Do list: add & remove

## Learning objectives
- Use webpack to bundle JavaScript.
- Learn how to use proper ES6 syntax.
- Use ES6 modules to write modular JavaScript.

### Estimated time: 4h

## Description
In this project, you will implement the CRUD (create, update, delete) methods. All the elements of the user interface will be fully functional and your application will be completed. 

*IMPORTANT NOTE: Read **all** requirements before you start building your project.*

### General requirements
- Make sure that there are [no linter errors](https://github.com/microverseinc/linters-config).
- Make sure that you used correct [GitHub Flow](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/github_flow.md).
- Make sure that you documented your work [in a professional way](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/documentation/articles/professional_repo_rules.md).

### HTML/CSS requirements
  - Follow our list of the [best practices for HTML & CSS](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/html_css_best_practices.md).
  
### JavaScript requirements
  - Follow our list of [best practices for JavaScript](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/javascript_best_practices.md).

### Project requirements
- Remove all hardcoded items from the tasks array.
- Create a new JavaScript file for the new functionality.
- Implement a function for adding a new task (add a new element to the array).
- Implement a function for deleting a task (remove an element from the array).
- Implement a function for editing task descriptions.
- By default new tasks should have the property `completed` set to `false` and the property `index` set to the value of the new array length (i.e. if you're adding a 5th task to the list, the index of that task should equal to 5).
- Deleting a task should update all remaining items' indexes, so they represent the current list order and are unique(i.e. if you're deleting the first task index 1 from the list, the index of the next task(2) should set to 1)..
- All changes to the To Do List should be saved in local storage.

### Need a big picture? 

Remind me about [the big picture of this project](./sneak_peek.md).

## Work and submission mode

- You should submit this activity **individually.**

## Code review

Follow [these steps](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/code-review/articles/how_to_ask_for_a_code_review.md) to request a code review of your project.

## Submit your project

After the final approval from a code reviewer, you need to submit your project.
[Read this FAQ for a reminder on how to submit your project.](https://microverse.zendesk.com/hc/en-us/articles/360061344234)
Now go to your Student Dashboard and submit your project.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
