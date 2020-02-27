# Forkify

Search over 100,000 recipes online. Please click [here](https://forkify-ram.netlify.com/) or [here](https://forkify.chsriram.repl.co/) to use the app.

*Note: This app was made by following an online course. Please check the course details [here](https://www.udemy.com/course/the-complete-javascript-course/).*

## Development Workflow -x- Learnings

There's a parent repository for this app, if the instructions in the parent repo are followed properly (the code is heavily commented), anyone can make this application. Please checkout the complete development workflow of this app [here (parent repo)](https://github.com/Ch-sriram/JavaScript#forkify-app-development-path-modern-js-es6-npm-babel-webpackforkify_project).

## Features -x- Instructions

1. Search for your favourite recipe by typing in the query in the search box. Please note that the number of search queries are limited to the list given [here](https://forkify-api.herokuapp.com/phrases.html).
2. Select a recipe from the recipe list generated from the query. The recipe with the details about the number of servings, time taken to make it along with all the ingredients, will be rendered onto the webapp. You can tweak the number of servings by pressing &#8853;/&#8854; buttons and the quantity of each ingredient for the recipe will change accordingly.
3. Add the recipe ingredients to the shopping list using the "ADD TO SHOPPING LIST" button. 
4. Increase/Decrease the quantity of each ingredient you want in the shopping list by using the &#x21f3; button respectively.
5. Remove the ingredient(s) from the shopping list by pressing the &#x24cd; button after hovering over the ingredient.
6. To remove all the ingredients from the shopping list, simply press the "DELETE ALL ITEMS" button below the "MY SHOPPING LIST" heading.
7. To get directions on how to make the dish by following the recipe given, just press the "DIRECTIONS" button below "HOW TO COOK IT" heading.
8. You can also like a recipe by pressing the &#x2661; symbol. Similarly, you can also unlike the recipes by pressing the &#x2661; symbol again on the recipe.
9. To find all your liked recipes, just hover on the &#x2764; symbol at the top right of the webapp, you can check out your liked recipes as a list. 

*Note that the webapp uses Cookies in the form of <code>localStorage()</code> API. If you see any warnings from the browser, kindly ignore them.*


## File Structure -x- Libraries Used

1. [axios](https://github.com/axios/axios) -- code dependency
2. [fractional](https://github.com/ekg/fraction.js/)    -- code dependency
3. [uniqid](https://github.com/adamhalasz/uniqid)   -- code dependency
4. [webpack](https://webpack.js.org/guides/getting-started/)  -- dev dependency
5. [babel](https://babeljs.io/docs/en/usage)    -- dev dependency

Please check <code>package.json</code>, <code>webpack.config.js</code> and <code>.babelrc</code> file present inside <code>./config/</code> for more information on the dependencies and configuration.

Check <code>./config/src/</code> for the code (Models - <code>./config/src/models/</code>, Views - <code>./config/src/views/</code>, Controller - <code>./config/src/index.js</code>) that makes the webapp work.

Original File Structure when developing the webapp can be found [here](https://github.com/Ch-sriram/JavaScript/tree/master/Modern-JS-ES6-NPM-Babel-Webpack/forkify_project). If you've the files in the original structure, then you can install the dependencies using <code>npm install</code> command using the shell/cmd/terminal in the cwd. After that, simply run <code>npm run start</code> command to run the app through the webpack-dev server @<code>localhost:8080</code>. To build it for production, run <code>npm run build</code> command in the shell. To build the app for development, run <code>npm run dev</code> command in the shell.