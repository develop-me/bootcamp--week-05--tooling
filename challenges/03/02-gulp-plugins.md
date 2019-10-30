# Install gulp plugins we'll need

The gulp plugins we're going to need to install:

- gulp-sass
- gulp-clean-css
- gulp-rename

We can do this by running `npm install {package name}` for each.

Or, you can do them all at once with:

`npm install {package1} {package2} {package3}`

## Setup your gulpfile.js

Create a `gulpfile.js` in the project root (next to `package.json`)

Require your gulp dependencies:

```
let gulp = require('gulp');
let cleanCSS = require('gulp-clean-css');
let rename = require('gulp-rename');
let sass = require('gulp-sass');
```

Add your first task:

```
gulp.task('sass', function () {
	return gulp.src('./scss/styles.scss')
		.pipe(sass())
		.pipe(rename('styles.css'))
		.pipe(gulp.dest('./css/'));
});
```

## Run your first gulp task

1) Make a change to `scss/customisations.scss`

1) Run `gulp sass`

1) Verify it updated `css/styles.css` with your change

1) :+1: task in Slack

## Advanced

1) Add more SCSS files into the process

1) Verify their CSS is being included in `css/styles.css`