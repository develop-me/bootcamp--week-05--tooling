# Install gulp plugins we'll need

The gulp plugins we're going to need to install:

- gulp-sass
- gulp-clean-css
- gulp-rename

We can do this by running `npm install {package name}` for each.

Or, you can do them all at once with:

`npm install {package1} {package2} {package3}`

## Setup your gulpfile.js

```
let gulp = require('gulp');
let cleanCSS = require('gulp-clean-css');
let rename = require('gulp-rename');
let sass = require('gulp-sass');
```

Add your first task:

```
gulp.task('sass', function () {
    var stream = gulp.src('./scss/styles.scss')
        .pipe(sass())
        .pipe(rename('styles.css'))
        .pipe(gulp.dest('./css/'));
    return stream;
});
```
