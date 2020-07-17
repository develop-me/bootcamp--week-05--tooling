# Commit changes to already tracked files

1) **Make changes to one of your tracked files**

1) **Commit those changes**

	Again use `git status` to see what Git thinks is going on.
	
	Use `git add {filename}` to stage the change to that file.
	
	Use `git status` again to see what is the status now.
	
	Use `git commit -m "A useful comment"` to create your next commit, with the files you had previously added to tracking.

1) **Make some more changes**

	Edit 2 or more files at a time, use `git add` to add them and commit the changes.

1) **Use `git log` to see the recent changes in your project.**

	Study the information and try to relate to the changes you've made and commands you've run.	
	
	If your history is too long for your terminal window you'll end up with a `:` prompt at the bottom, as you can use your cursor to go up and down the log. Use `q` to quit.

1) Put an emoji in the slack channel so your instructor knows you're done.

## Advanced challenges

These are optional challenges you can do if you finish quickly.

1) See differences

Make a change to a file, save it and use git diff to see how you can use the diff tool to see what has changed.

Useful if a git status shows things have been modified but you're not sure what or can't remember what you changed.

2) `git add` shortcuts

Read the notes PDF box on "git commit arguments" in section 3.2.5 and experiment with the `-a` flag in `git commit -am`

