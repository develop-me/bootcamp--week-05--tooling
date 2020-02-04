# Using pull requests

You are going to perform 3 tasks:

- add a simple `<nav>` to all HTML pages, could just be 1 `<a>` link
- add a contact page with simple form
- add a new stylesheet and `<link>` to all HTML pages

For these use separate feature branches with pushing to remote, and pull requests each time.

The workflow:

1) `git checkout master`
1) `git pull` in case master has changed (if you get an _There is no tracking information
_ error run `git branch --set-upstream-to=origin/master master
`)
1) `git branch {branch name}`
1) `git checkout {branch name}`
1) [do work]
1) `git commit -am "commit message"`
1) `git push origin {branch name}`
1) go to your project repo on [GitHub.com](https://github.com/) and make a pull request with your new feature branch
1) review, approve and merge the pull request
1) delete the branch on remote (GitHub)
1) on local switch back to master
1) `git pull` the recent changes to master
1) continue to next task

## Advanced, optional 

Once you have merged your branches onto master you could do a cleanup of the now redundant feature branches.

This needs to be done on remote (GitHub) and locally.

1) Delete branch from GitHub (there is a button in the branches area)
1) `git checkout master` and `git pull` to fetch freshest version of `master` branch
1) See what branches you're aware of with `git branch -a`
1) To delete local branches `git branch -d {branch name}`
1) To remove a branch from the list that is on remote (shows like `remotes/origin/{branch name}`) run: `git remote prune origin`

