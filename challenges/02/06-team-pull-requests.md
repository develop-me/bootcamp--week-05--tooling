# Team work with pull requests

The aim of this exercise is to simulate what it can be like working in teams.

*Note: we're using the same repo as the challenge before. It's available on GitHub here: [https://github.com/develop-me/git-simple](https://github.com/develop-me/git-simple)*

### Part 1

1) **Do some work in a feature branch**

   Create a local branch

   Make some changes to the site & preview changes in browser

   Commit them to your local branch

1) **Put your changes on the repo and merge into master**

   Push your branch up to GitHub `git push origin {branch-name}`

   Create a pull request in GitHub asking to merge your branch into master
   
   Assign the pull request to yourself and resolve any merge conflicts

   Once you have successfully merged, clean up after yourself and remove your branch from GitHub and your local repo. 
   
   Run `git branch -a` to see what branches your local repo knows about. Running `git fetch --prune` will update your local repo's output of what's branches exist in the remove. Run `git branch -a` again to check all your lists of branches are in sync with one another.

1) **Get the latest version of master** 

   Checkout your master branch
   
   Run `git pull` to an update to date copy of master from the remote repo.


1) **Add an emoji to slack indicate you are ready to receive pull requests in part 2**	


### Part 2

This where it could start getting interesting, and you are likely to encounter merge conflicts that you need to work through and resolve.

1) **Do some work in a feature branch**

   Create a local branch

   Make some smallish changes to the site & preview changes in browser

   Commit them to your local branch

1) **Put your changes on the repo and create a pull request**

   Push your branch up to GitHub

   Create a pull request in GitHub asking to merge your branch into master
   
   Assign the pull request to someone who has left an emoji against part 1 of this challenge in slack

1) **Resolve a pull request assigned to you**

   Hopefully you will already have, or will shortly receive a pull request from one else to resolve

   Have a go at resolving it. Use the commenting functionality within the pull request to communicate if you have questions etc.

   Once the merge is complete, clean up your branches.

   If you did not get chance to practice resolving a merge conflict, ask for another pull request. Remember a merge request happens when the same part of a file has been edited in two different commits.

**Add an emoji to slack to indicate you have finished part II**	



## Advanced challenges

These are optional challenges you can do if you want some more.

## [Optional challenge >](07-issues.md)
