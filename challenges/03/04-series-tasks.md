# Create a series task

Add a new task to gulp:

`gulp.task('styles', gulp.series('sass', 'minify-css'));`

## Verify combined task is working

1) make a change to `scss/customisations.scss` or similar
1) run `gulp styles`
1) verify it produced the change in `css/styles.min.css` file or check browser