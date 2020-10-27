## Creating branches locally and pushing them to the remote

1) **Start on your main branch**

   `git checkout main`
   `git fetch` - get the latest version of main
   
	If you get an _There is no tracking information_ error run `git branch --set-upstream-to=origin/main main`

1) **Create your branch and do work**

   `git branch {branch name}`
   `git checkout {branch name}`
    [do work and commit]

1) **Send your branch to the remote repo**

   `git push origin {branch name}`

1) **Do some more work**

	`git push`

**Add an emoji to slack to let the instructor know you have finished**	
