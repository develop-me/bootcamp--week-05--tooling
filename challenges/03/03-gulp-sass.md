# Use gulp to compile your SASS

## Install the needed npm packages

We're going to need:

- gulp-sass


## Edit your gulpfile.js

Require the additional sass dependency at the top of your gulpfile

Add the sass task:

```javascript
gulp.task('sass', function () {
	return gulp.src('./scss/styles.scss')
		.pipe(sass())
		.pipe(rename('styles.css'))
		.pipe(gulp.dest('./css/'));
});
```


## Run the SASS task

1) Make a change to `scss/customisations.scss`
1) Run `gulp sass`
1) Verify it updated `css/styles.css` with your change
1) Sense check that it is all working by making a change to `scss/customisations.scss`, like `body{background:red;}` then running **both** gulp tasks *in the right order* - this is key, think about what is happening to the files in our build process
1) Verify you can see the resulting CSS change in the browser

## **Add an emoji to slack to let the instructor know you have finished**


## Advanced

1) Add more SCSS files into your project
1) Verify their CSS is being included in `css/styles.css`
1) Make some more pages for your site
1) Link to them in the menu
1) Continue to develop your site
