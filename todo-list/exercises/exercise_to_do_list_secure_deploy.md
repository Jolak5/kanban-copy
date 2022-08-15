# To Do list: secure deploy

## Learning objectives
- Deploy a secure website using OpenSSL.

### Estimated time: 1h

## Exercise
Now that your To Do list application is ready, you can deploy it to the public. In this exercise, you will deploy your code via GitHub Pages. You will need to make sure that your web application uses HTTPS (not HTTP) protocol. SSL (Secure Sockets Layer) and HTTPS guarantee that all data sent between a browser and a server are encrypted, which adds a great layer of security for your users and their private and sensitive information.

*IMPORTANT NOTE: Read **all** instructions before you start this exercise.*

*SECOND IMPORTANT NOTE: Even though this lesson is solo, you should already be in contact through Slack with your partner. Each Monday should start with a message on Slack to your coding partner. Remember to start each week by setting working agreements with your partner to improve your collaboration and avoid conflict. [You can find the lesson here](https://github.com/microverseinc/curriculum-professional-skills/blob/main/orientation/establish-good-working-relationships.md). Bookmark it so you can use it at the start of each week. If you are experiencing difficulties with your partner, reach out to Student Success right away so we can help you. It's important that you have a good collaboration that results in learning. We always try to speak to all parties involved to resolve the conflict. In some cases, we will re-pair you with a new student (this is only possible in the beginning of the week).*



### Instructions 

- Commit and push all your work into the project's GitHub repository.
- If you worked with branches, make sure you merge all your work into the main branch.
- Make sure that in the `dist` directory on Github you have the latest version of your project.
    - Run `npm run build` to update the `dist` if necessary.
- Deploy your website using GitHub Pages (you are already familiar with this process), but this time pay attention to the extra step that will **ensure that your app uses HTTPS protocol**:
     - Scroll to the bottom of the **Pages** page and make sure the *"Enforce HTTPS"*  checkbox is selected.
- Confirm the deployment. Your application will be live in a few minutes. On the top of the **Pages** page, you will find your project's URL.
    - **NOTE: as GH pages are meant to deploy static pages you need to go to the `dist` directory to see your app: https://<GH_username>.github.io/<GH_repo_name>/dist/.**
    - As the point of this exercise is to learn about HTTPS with GitHub pages it is sufficient to stay with this setup. However, if you are interested in the deployment of the webpack-based app with GH pages in a more elegant way, check the information in the [Additional materials](#additional-materials) section.
- Make sure that your app URL uses SSL.
- Update the README of your repository to include a link to the online version.

### Submit your exercise
[Read this FAQ for a reminder on how to submit your exercise.](https://microverse.zendesk.com/hc/en-us/articles/360061344234)
Now go to your Student Dashboard and submit your exercise.


## Additional materials
*These are all optional, but if you're interested in exploring this topic further, here are some resources to help you. Any exploration here should be done outside program time.*
- Read about [why it's important to use SSL certificates](https://www.cloudflare.com/learning/ssl/why-use-https/).
- Read about potential [problems with mixed content](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https) and how to solve them.
- Curious about how to deploy webpack-based apps with GitHub pages in a more elegant way? Check the ["GitHub Pages Deploy & Domain" video](https://www.youtube.com/watch?v=SKXkC4SqtRk) (until 9:35 it explains how to deploy with the usage of [gh-pages package](https://github.com/tschaub/gh-pages), then it shows how to set up a custom domain).

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._
