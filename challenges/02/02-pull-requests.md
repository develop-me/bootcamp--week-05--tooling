# Using pull requests

You are going to perform 3 tasks:

- add a simple `<nav>` to all HTML pages, could just be 1 `<a>` link
- add a contact page with simple form
- add a new stylesheet and `<link>` to all HTML pages

For these use separate feature branches with pushing to remote, and pull requests each time.

The workflow:

1) `git checkout master`
1) `git branch {branch name}`
1) `git checkout {branch name}`
1) [do work]
1) `git commit -am "commit message"`
1) `git push origin {branch name}`
1) go to [GitHub.com](https://github.com/) and make a pull request with your new feature branch
1) review, approve and merge the pull request
1) delete the branch on remote (GitHub)
1) on local switch back to master
1) `git pull` the recent changes to master
1) continue to next task