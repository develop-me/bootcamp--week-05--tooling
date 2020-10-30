# Use gulp to compile your SASS

Heads up! This challenge is a little bit harder than the others you've done far. Read the instructions carefully and have a think about what each step is asking you to do because this challenge does not tell you the exact commands to run or exact steps to take. 

## Install the needed npm packages

1) Install the `gulp-sass` package into your project

2) How can you check this has worked?


## Edit your gulpfile.js

1) Require the additional sass dependency at the top of your gulpfile

2) Add the sass task into the body of your `gulpfile.js`:

```javascript
gulp.task('sass', function () {
	return gulp.src('./scss/styles.scss')
		.pipe(sass())
		.pipe(rename('styles.css'))
		.pipe(gulp.dest('./css/'));
});
```


## Run the SASS task

1) Make a change to `scss/customisations.scss` like `body{background: CornflowerBlue;}`
1) Run `gulp sass`
1) Verify it updated `css/styles.css` with your change
1) What gulp task do you need to run next to get the changes showing in your browser? This is key, think about what is happening to the files in our build process
1) Verify you can see the resulting CSS change in the browser

## **Add an emoji to slack to let the instructor know you have finished**


## Advanced

1) Add more SCSS files into your project and verify their CSS is being included in `css/styles.css`
1) Read more about {SASS}(https://sass-lang.com/documentation) and have a play with some of the cool features like nesting, variables or mixins. 
