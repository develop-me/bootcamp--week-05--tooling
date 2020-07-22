# Going back
1) **Use `git checkout {ref}` to rewind your project files**

	Use `git reflog` to see recent history and commit references
	
	Choose a commit to go back to (rewind) and check it out. 

	This can be done by referencing the commit reference `git checkout {ref}` or using the `git checkout HEAD~{n}` syntax to go back `n` commits.

	Check the files are in the state you expect, i.e. old versions.
	
1) **Go back to most recent commit**

	Use `git checkout master` or `git switch -` to get back to the most recent commit.

1) **Move to a different commit**

	Redo step 1 again, but this time move to a different commit than before.

1) **Use `git reset`**

	Experiment with `git reset --hard HEAD` and `git reset --soft HEAD` to return back to your last commits.

	Keep using `git reflog` to track how you are moving around between your commits.

1) **Add an emoji to slack to let the instructor know you have finished**

## Advanced

1) Roll back to a previous commit
1) Make some changes to your files
1) Try and commit those changes
1) You will find you can't - why is this?

Or for more fun read up about stashing in the notes and give it a whirl.