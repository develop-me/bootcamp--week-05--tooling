# Minify your site's CSS

Build on the project you set-up in exercise 1.


## Install gulp plugins we'll need

For this task to run we'll need to ensure we have the following packages installed:

- gulp (already installed from the previous challenge)
- gulp-clean-css
- gulp-rename

We can do this by running `npm install {package name}` for each.

Or, you can do them all at once with:

`npm install {package1} {package2} {package3}`


## Setup your gulpfile.js

Create a `gulpfile.js` in the project root (next to `package.json`)

Require gulp and your gulp dependencies at the top of the file:

```javascript
let gulp = require('gulp');
let cleanCSS = require('gulp-clean-css');
let rename = require('gulp-rename');
```

## Setup a task to minify the CSS file

Define a new task `minify-css`:

```javascript
gulp.task('minify-css', () => {
  return gulp.src('css/styles.css')
	.pipe(cleanCSS({compatibility: 'ie8'}))
	.pipe(rename({suffix: '.min'}))
	.pipe(gulp.dest('./css/'));
});
```

## Run the task and check it works

1) run the task with `gulp minify-css`
1) verify it produced a `css/styles.min.css` file
1) edit your site's HTML to use that CSS file instead
1) verify your site is using the new CSS file (it will be needed for later challenges)


## Commit your changes locally

Don't push your changes to the remote repo, just keep them as local changes


## **Add an emoji to slack to let the instructor know you have finished**