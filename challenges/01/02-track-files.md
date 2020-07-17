# Version manage some new files

1) **Add some files into your new project**

	Create a basic web project of this sort of structure:

	```bash
	index.html
	/css
	   style.css
	/js
	   scripts.js
	```

	You can use `touch {filename}` to create files from the command line and `mkdir {dirname}` to create directories. 

	When you run these commands take care that you are in the right directory in your terminal.

1) **Start version managing your files**

	Use `git status` to see what Git thinks is going on.

	Use `git add {filename}` to start tracking the files in your project.

	Note: you may need to use the full path, e.g. `git add css/style.css`

	Use `git status` again to see what is the status now.

	Use `git commit -m "Basic project files created"` to create your first commit, with the files you had previously added to tracking. You can change the commit message if you like.

## [Next challenge >](03-changes.md)
