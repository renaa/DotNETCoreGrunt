
removed and reinstalled both nvm (used the installer, althought I don't think it matters), and node.
# Creating a DotNetCore app with Grunt and Sass
https://dzone.com/articles/how-to-use-sass-in-aspnet-core-20-mvc

### template for creation
* create project in VS
* Add Styles/*.scss
* npm init
* npm install grunt --save-dev
* npm install grunt-cli --save-dev
* npm install grunt-sass --save-dev
* add gruntfile.js to root with content provided
  * (these  can be installed globally by appending the command with '-g')
* add `const sass = require('node-sass'); && implementation: sass,`
* install Whack Whack Terminal (!)

this works when running grunt 
But in Task Runner Explorer gruntfile.js is showing (No tasks found) 

And Gulp seems cooler now so:

# PROCESSING SASS WITH GULP IN ASP.NET
https://www.craftedpod.com/tech/processing-sass-with-gulp-in-asp-net/

* ` npm install --save-dev gulp-sass gulp-rename gulp-postcss autoprefixer cssnano gulp`
* add gulpfile.js
* `gulp styles`
* still not working in task runner :smh
* gulp watch, ran into this problem 
* https://stackoverflow.com/questions/39665773/gulp-error-watch-task-has-to-be-a-function
* tried npm rebuild node-sass 
* still not working in task runner :smh
* had to go into `Tools > Options > Projects and Solutions > Web Package Management > External Web Tools` to put PATH at top (!) 
* 😃

