## Going back
1) **Use `git checkout {ref}` to rewind your project files**

	Use `git reflog` to see recent history and commit references
	
	Choose a commit to go back to (rewind) and check it out. 

	This can be done by referencing the commit reference `git checkout {ref}` or using the `git checkout HEAD~{n}` syntax to go back `n` commits.

	Check the files are in the state you expect, i.e. old versions.
	
1) **Go back to most recent commit**

	Use `git checkout master` or `git switch -` to get back to the most recent commit.
	

## Removing experimental work

1) **Make sure you are on the last commit**

	Use `git checkout master` to be sure
	

1) **Make some changes, you can save your work but don't commit it**


1) **Use `git reset`**

	Experiment with `git reset --hard HEAD` to throw away your experimental work.

	Keep using `git reflog` to track how you are moving around between your commits and `git status` to check where you are

1) **Add an emoji to slack to let the instructor know you have finished**

## Advanced

1) Roll back to a previous commit
1) Make some changes to your files
1) Try and commit those changes
1) You will find you can't - why is this?

Other stuff you can do:
* Read up about stashing in the notes and give it a whirl.
* Read in depth about the different `git reset` flags: --hard, --mixed and --soft (Atlassian reset tutorial)[https://www.atlassian.com/git/tutorials/undoing-changes/git-reset]
