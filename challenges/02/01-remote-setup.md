# Setting up to work with a remote repository on GitHub

1) Set up a new project on [GitHub](https://github.com)
1) Define the name that your local repo uses for your new remote repository with `git remote add origin {"Clone with SSH" URL from GitHub}`
1) Fetch information about the project at GitHub with `git fetch`
1) Push your work on master to the remote repb with `git push -u origin master` (this also links the local and remote repos together with the -u flag)
1) Verify your work has appeared on GitHub by viewing in the browser
1) Make further changes to your project
1) Commit changes
1) Push changes (you can use just `git push`)
1) Rinse and repeat
