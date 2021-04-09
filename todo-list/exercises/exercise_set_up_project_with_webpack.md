# Set up project with Webpack

## Learning objectives
- Use webpack

### Estimated time: 1.5h

## Description
In this exercise we want you to use the knowledge you have gained already by reading the webpack guides from the previous lesson. However, we don't want you to just follow all the steps from the guides. Instead, we want you to build a simple yet powerful webpack setup, which you can later use as a starting point boilerplate in many of your future projects.

### Why is it important?
You should know how webpack works, and how you can configure it to fit your project needs. This will greatly improve your developer experience and the quality of  your code.

## Exercise

### Init new project and install webpack

First, create a new folder **webpack-exercise**, `init` the project and install webpack:
```
mkdir webpack-exercise
cd webpack-exercise
npm init -y
npm install webpack webpack-cli --save-dev
```
Next, create two subfolders for our source and distribution code:
```
mkdir src
mkdir dist
```
We will do some custom setup in our project, so we need a **webpack.config.js** file. Create one in the root (main) directory and paste the following code:

```javascript
const path = require('path');

module.exports = {
  entry: './src/index.js',
  output: {
    filename: 'main.js',
    path: path.resolve(__dirname, 'dist'),
  },
};
```
Now we want to add webpack to our scripts in **package.json**, to  conveniently run it when we need it:
```json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    +"build": "webpack"
  },
```
### Add entry file 
With webpack installed and configured we are ready to add some code. In our **webpack.config.js** we have declared our main entry file to be *'./src/index.js'*, but we have not yet added it. Go ahead and create **index.js** file in */src* directory and add a console message to it - i.e. `console.log('hello webpack')`.
Now save it and run:
```
npm run build
```
If all went well, you should now see a new file created in */dist* folder. 

Your project folder and files structure should look like this:
```
webpack-exercise
    |- /dist
        |- main.js
    |- /src
        |- index.js
    |- package.json
    |- webpack.config.js

```
### Add HTML
To have our application working in the browser we need to add a HTML file. All the files viewable in a browser will be placed in */dist* directory. In general, we should not create files manually in the */dist* folder, as there's always a risk our changes will be overwritten. Therefore, we will add a webpack plugin to automatically create **index.html** for us. 

Follow the instructions from the [setting up HtmlWebpackPlugin](https://webpack.js.org/guides/output-management/#setting-up-htmlwebpackplugin) guide. Be extra careful when updating the `module.exports` object in your **webpack.config.js** file, to not to make any nesting mistakes.

Now run:
```
npm run build
```
and check your */dist* folder. If it contains a new **index.html** file, it means you were successful. Open it in a browser and check if your `console.log` message shows correctly. View it in a code editor and check, how webpack correctly inserted `<script>` tag with a path to *./main.js* and minified the HTML for better performance.

### Add CSS
Now let's add some style to our boilerplate.
Follow the steps in [loading CSS](https://webpack.js.org/guides/asset-management/#loading-css) guide.

In your **style.css** file add a generic rule, like:
```css
body {
    background-color: bisque;
}
```
Next, execute:
``` 
npm run build 
```
and check if the HTML body has changed.

### Setup local dev server
Finally, we want to improve our developer experience - we don't want to run the build command from the terminal every time we make a change in the code. 
Therefore we will install a webpack dev server, which will *watch* our source files, generate compiled distribution files, and even refresh the browser every time we save changes in the source code.

Follow the [using webpack-dev-server](https://webpack.js.org/guides/development/#using-webpack-dev-server) guide and set it up on your local machine.
Again, be cautious with the `module.exports` object in your **webpack.config.js**.

Once these steps are complete, you should see your application working at: `http://localhost:8080/`. Every change you make in **js** or **css** files now should be reflected in a browser a few seconds later.

### Submit your exercise
--TODO: write submission instructions

## Additional materials [optional header]
We strongly advise you to check the [official webpack documentation](https://webpack.js.org/concepts/) to have a thorough understanding of the tools you're using here.
