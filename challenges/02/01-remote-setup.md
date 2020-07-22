# Setting up to work with a remote repository on GitHub

1) **Set up a new project on [GitHub](https://github.com)**

1) **Define the name that your local repo uses for your new remote repository**
	`git remote add origin {"Clone with SSH" URL from GitHub}`

1) **Fetch information about the project from GitHub**
    `git fetch`

1) **Push your work to the remote repo**
   `git push -u origin master` 
   
   This pushes your local master branch to the remote master branch
   This also links the local and remote repos together with the -u flag

1) **Verify your work has appeared on GitHub**
	Open your repo in a browser

1) **Do work**
	Make further changes to your project
	Commit changes

1) **Push changes**
   Because you have linked the repos together you can use just `git push`

## [Next challenge >](02-pull-requests.md)
