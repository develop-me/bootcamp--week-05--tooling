# Automate your workflow with watching

1) create a task that will watch some files for changes then automatically run some other task(s) for you.
  You'll need a task with something like this:
  \
  `return gulp.watch('./scss/**/*.scss', gulp.series('{task to run}'));`

1) test it with `gulp {name of your watch task}`

1) :+1: task in Slack

## Advanced

1) Setup a watch task for JS files