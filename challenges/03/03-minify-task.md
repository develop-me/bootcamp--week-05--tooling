# Setup a task to minify the CSS file

Add this to your `gulpfile.js` to define a new task `minify-css`:

```javascript
gulp.task('minify-css', () => {
  return gulp.src('css/styles.css')
	.pipe(cleanCSS({compatibility: 'ie8'}))
	.pipe(rename({suffix: '.min'}))
	.pipe(gulp.dest('./css/'));
});
```

## Run your second gulp task

1) run that task with `gulp minify-css`
1) verify it produced a `css/styles.min.css` file
1) switch your site (HTML) to use that CSS file instead
1) sense check that it is all working by making a change to `scss/customisations.scss`, like `body{background:red;}` then running **both** gulp tasks *in the right order* - this is key, think about what is happening to the files in our build process
1) verify you can see the resulting CSS change in the browser 
1) :+1: task in Slack

## Advanced

1) Make some more pages for your site
1) Link to them in the menu
1) Continue to develop your site
