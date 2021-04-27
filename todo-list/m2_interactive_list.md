# To Do list: interactive list

## Learning objectives
- Use webpack to bundle JavaScript.
- Learn how to use proper ES6 syntax.
- Use ES6 modules to write modular JavaScript.

### Estimated time: 3.5h

## Description
In this project, you will add some functionality to your application to make it interactive. The user will be able to reorder the list by **dragging** each item and moving it into the desired position. The user will also be able to **mark task completion** by selecting the corresponding checkbox. The updated tasks list will be stored in *local storage*.

*IMPORTANT NOTE: Read **all** requirements before you start building your project.*

### General requirements

- Make sure that there are [no linter errors](https://github.com/microverseinc/linters-config).
- Make sure that you used correct ([GitHub Flow](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/github_flow.md).
- Make sure that you documented your work [in a professional way](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/documentation/articles/professional_repo_rules.md).

### HTML/CSS requirements

- Follow our list of the [best practices for HTML & CSS](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/html_css_best_practices.md).

### JavaScript requirements

- Follow our list of [best practices for JavaScript](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/javascript_best_practices.md).

### Project requirements

- Add 2 new JavaScript files and import them as modules:    
    - one will contain methods related to drag / drop and sorting functionality.
    - the other will contain methods related to the status updates (`completed`: `true` / `false`).
- Add event listeners to list items (`dragstart`, `dragover`, `drop`) and to checkbox (`change`).
- Update items object's values for `index` and `completed` keys upon user actions.
- Store the updated array of items in local storage, so the user gets the correct list values after the page reloads.

### Need a big picture? 

Remind me about [the big picture of this project](./sneak_peek.md).

## Code review

Follow [these steps](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/code-review/articles/how_to_ask_for_a_code_review.md) to request a code review of your project.

## Submit your project

After the final approval from a code reviewer, you need to submit your project.
[Read this FAQ for a reminder on how to submit your project.](https://microverse.zendesk.com/hc/en-us/articles/360061344234)
Now go to your Student Dashboard and submit your project.

