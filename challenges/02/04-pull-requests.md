# Using pull requests

**Please read through all the instructions at least once before you start.**

You are going to perform 3 tasks:

- add a simple `<nav>` to all HTML pages, could just be 1 `<a>` link
- add a contact page with simple form
- add a new stylesheet and `<link>` to all HTML pages

For each task use a separate feature branch, pushing it to remote, create and resolve the merge request.

### Before you start

1) **Set up a new local and remote repo**

### The workflow for each task

1) **Start on your master branch**

   `git checkout master`

   `git pull` - get the latest version of master
   
	If you get an _There is no tracking information_ error run `git branch --set-upstream-to=origin/master master`

1) **Create your branch and do work**

   `git branch {branch name}`

   `git checkout {branch name}`

    [do work and commit]

1) **Send your branch to the remote repo**

   `git push origin {branch name}`

1) **Do the pull request**

   Go to your project repo on [GitHub.com](https://github.com/) and make a pull request with your new feature branch

   Review, approve and merge the pull request
   
   Delete the branch on remote (GitHub)

1) **Continue**

	Back to step one and continue to next task

**Add an emoji to slack to let the instructor know you have finished before moving on to stuff below**	


## Advanced, optional 

Once you have merged your branches onto master you could do a cleanup of the now redundant feature branches.

This needs to be done on remote (GitHub) and locally.

1) Delete branch from GitHub (there is a button in the branches area)
1) `git checkout master` and `git pull` to fetch freshest version of `master` branch
1) See what branches you're aware of with `git branch -a`
1) To delete local branches `git branch -d {branch name}`
1) To remove a branch from the list that is on remote (shows like `remotes/origin/{branch name}`) run: `git remote prune origin`

