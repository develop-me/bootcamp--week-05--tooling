# Create a series task

Add a new task to gulp to run other tasks in series like this:

`gulp.task('{task name}', gulp.series('{task1}', '{task2}'));`

## Verify combined task is working

1) make a change to `scss/customisations.scss` or similar

1) run `gulp {series task name}`

1) verify it produced the change in `css/styles.min.css` file or check browser

1) :+1: task in Slack

## Advanced

1) Continue to develop your site