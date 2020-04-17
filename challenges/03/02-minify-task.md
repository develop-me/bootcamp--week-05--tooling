# Setup a task to minify the CSS file

Create your new `gulpfile.js` and define a new task `minify-css`:

```javascript
gulp.task('minify-css', () => {
  return gulp.src('css/styles.css')
	.pipe(cleanCSS({compatibility: 'ie8'}))
	.pipe(rename({suffix: '.min'}))
	.pipe(gulp.dest('./css/'));
});
```

## Run the task and check it works
