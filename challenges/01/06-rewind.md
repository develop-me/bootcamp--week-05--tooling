# Going back
1) **Use `git checkout {ref}` to rewind your project files**
	Use `git reflog` to see recent history and commit references
	\
	Choose a commit to go back to (rewind) and check it out with `git checkout {ref}`
	\
	This can be done by referencing the commit reference or use the `git checkout HEAD{n}` syntax to go back `n` commits.
	\
	Check the files are in the state you expect, i.e. old versions.
1) **Go back to most recent commit**
	If you used `git checkout {ref}` you can use `git checkout master` or `git switch -` to get back to the most recent commit.
	\
	If you used the `HEAD{n}` method you can do `git checkout HEAD` to get back to the most recent commit.
