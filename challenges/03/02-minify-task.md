## Install gulp plugins we'll need

For this task we're going to need to install:

- gulp
- gulp-clean-css
- gulp-rename

We can do this by running `npm install {package name}` for each.

Or, you can do them all at once with:

`npm install {package1} {package2} {package3}`

## Setup your gulpfile.js

Create a `gulpfile.js` in the project root (next to `package.json`)

Require gulp and your gulp dependencies:

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

1) run that task with `gulp minify-css`
1) verify it produced a `css/styles.min.css` file
1) switch your site (HTML) to use that CSS file instead
1) :+1: task in Slack
