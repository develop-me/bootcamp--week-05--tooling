# Feature branches

You are going to perform 3 tasks:

- add a new HTML page
- add an image to one of the pages
- add a footer copyright notice to all pages

To practice the branching technique, create a new feature branch *for each task*. That'll be three new branches in all.

## Step by step guide

1) **Create new feature branch**
- Ensure you are on the master branch to start with - `git checkout master`
- Create a new feature branch for your task, with a sensible name using `git branch {feature branch name}`

2) **Begin working on your new branch**
- Checkout your newly created branch `git checkout {feature branch name}`
- Use `git branch -a` to see available branches and verify which branch you are currently working on

3) **Make changes**
- Do work
- Commit with fab commit messages

4) **Merge new branch into master**
- Switch back to `master` with `git checkout master`
- You won't see your changes in master as they are in your other branch
- Merge your feature branch into `master` with `git merge {feature branch name}`
- Optionally delete the now merged feature branch `git branch -D {feature-branch-name}`

5) **Keep going**
- Do the remaining tasks, making sure you start on the master branch each time
- **Add an emoji to slack to let the instructor know you have finished**

### Stretch stuff
If you have completed all of the above you can read about resolving merge conflicts in the notes.