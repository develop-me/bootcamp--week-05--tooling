# Project setup

1) **Create a new project folder with the command line**

	Use `cd  {directory name}` and `mkdir {my new folder}` to navigate to where you'd like to make your new directory and make it.

	_Protip: you can drag a file or folder from Finder (Mac) or Explorer (Windows) into terminal to get the full path rather than typing the whole path._

1) **Start to version manage that new folder**

	`cd` into your new directory first
	Use `git init` inside your new folder to start version managing the project.

1) **Check your Git repository is in place**

	Verify the `.git` directory has been created inside your project directory - this tells you that Git is ready to go.

	There are a few ways of doing this:
	
	- In Finder (Mac) or Explorer (Windows) if you have hidden files visible then you will see it.

	- On command line you can use `ls -a` to output *all* files including hidden files.

	- Run `git status` to see if Git is functioning. If the folder isn't version managed by Git you'll get:

		```bash
		fatal: not a git repository (or any of the parent directories): .git
		```

	*Note: Files starting with `.` are often hidden by default in visual/graphical file viewers and on command line*

## [Next challenge >](02-track-files.md)
