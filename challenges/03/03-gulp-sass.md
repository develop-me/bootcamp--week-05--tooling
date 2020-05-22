# Install the extra gulp plugins we'll need

We're going to need to install:

- gulp-sass


## Edit your gulpfile.js

Require the additional sass depenency

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
1) sense check that it is all working by making a change to `scss/customisations.scss`, like `body{background:red;}` then running **both** gulp tasks *in the right order* - this is key, think about what is happening to the files in our build process
1) verify you can see the resulting CSS change in the browser 
1) :+1: task in Slack


## Advanced

1) Add more SCSS files into the process
1) Verify their CSS is being included in `css/styles.css`
1) Make some more pages for your site
1) Link to them in the menu
1) Continue to develop your site
