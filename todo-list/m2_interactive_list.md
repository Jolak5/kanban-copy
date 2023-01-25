# To Do list: interactive list

## Learning objectives
- Use webpack to bundle JavaScript.
- Learn how to use proper ES6 syntax.
- Use ES6 modules to write modular JavaScript.

### Estimated time: 4h

## Description
In this project, you will add some functionality to your application to make it interactive.  The user will also be able to **mark task completion** by selecting the corresponding checkbox (or undo it by unchecking the checkbox). The updated tasks list will be stored in *local storage*.

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

- Add a new JavaScript file and import it as a module:    
    - it will contain methods related to the status updates (`completed`: `true` / `false`).
- Add event listener to the checkbox (`change`).
- Update items object's value for `completed` key upon user actions.
- Implement a function for the "Clear all completed" button (use `filter()` method).
- Store the updated array of items in local storage, so the user gets the correct list of values after the page reloads (which means that any changes made to the list should be preserved).

### Need a big picture? 

Remind me about [the big picture of this project](./sneak_peek.md).

## Code review

Follow [these steps](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/code-review/articles/how_to_ask_for_a_code_review.md) to request a code review of your project.


## Work and submission mode

- You should submit this activity **individually.**

## Submit your project

After the final approval from a code reviewer, you need to submit your project.
[Read this FAQ for a reminder on how to submit your project.](https://microverse.zendesk.com/hc/en-us/articles/360061344234)
Now go to your Student Dashboard and submit your project.


## Additional requirements

_These are all optional, but if you're interested in exploring this topic further, feel free to implement them. Any exploration here should be done outside program time._

_If you decide to implement these requirements you should do it in a separate pull request. As always, remember to clearly document your decision in GitHub comments._



The user should be able to reorder the list by **dragging** each item and moving it into the desired position.

- Add a new JavaScript file and import it as a module:    
    - it will contain methods related to drag / drop and sorting functionality.
- Add event listeners to list items (`dragstart`, `dragover`, `drop`).
- Update items object's values for `index` key upon user actions.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._


