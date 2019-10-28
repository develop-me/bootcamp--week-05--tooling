# Remove files from tracking or project

1) **Remove a file from tracking but keep the file**

	`git rm --cached {file path}`
	
1) **Add the file path to a `.gitignore` file**
	
	Make a file called `.gitignore` in your root project folder. You system might complain about `.dot` files being special or reserved, but you can just ignore this and click `Use "."`. You're an adult dammit!

	Then verify you can't accidentally add the file back in to tracking, e.g. with `git add {file path}` or `git add *` (**careful!**)

1) **Commit the change**

	Use `git status` to see what Git thinks is going on, then commit the change to the project.

1) **Remove a file from tracking and delete the file**

	Use `git rm {file path}`
	
	Use `git status` to see what Git thinks is going on, then commit the change to the project.
