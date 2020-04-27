# Feature branches

You are going to perform 3 tasks:

- add a new HTML page
- add an image to one of the pages
- add a footer copyright notice to all pages

To practice the branching technique, create a new feature branch *for each task*.

For each task follow the process:

1) Ensure you are on the master branch to start with. You can use `git checkout master` for this.
1) Create a new feature branch for your task, with a sensible name using `git branch {feature branch name}`.
1) Checkout that branch `git checkout {feature branch name}`
1) Use `git branch -a` to see available branches and which branch you are currently working on
1) Do work
1) Commit
1) Switch back to `master` with `git checkout master`
1) Where is your work?
1) Merge your feature branch into `master` with `git merge {feature branch name}`
1) Optionally delete the now merged feature branch
1) Do the remaining tasks, making sure you start on the master branch each time
