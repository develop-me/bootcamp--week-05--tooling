# Quiz Answers

## 1. Getting setup with Git

This sets up a relationship between an (existing) local repository and the remote repository at the given origin URL.

a) This is the part that sents the configuration to link to the remote repo.

b) The remote repo is hosted on github.com (could be bitbucket.org, gitlab.com or any other Git repository host)

c) The repo is owned by the user or organisation `develop-me`

d) The project repository name or address is `drupal1`

## 2. Committing files

First commit:
```bash
git add images/ index.html
git commit -m "Apple"
```

Second commit:
```bash
git add hello.html
git commit -m "Banana"
```

Or, as `hello.html` already tracked:

```bash
git commit -am "Banana"
```

## 3. Reading Git messages: Oh noes #1

a) `git push`

b) Some changes have been made at GitHub.

c) I first need to pull those changes down, with `git pull` then can try `git push` again, unless there is a conflict.

## 4. Reading Git messages: Oh noes #2

a) `git pull`

b) I have made some changes to `index.html` that I haven't committed yet.

If the pull had been allowed it might have overwritten that file.

c) I should commit my changes to that file before pulling again.

## 5. Reading Git messages: Oh noes #3

a) `git pull`

b) Some changes from the remote overlap have been made at GitHub.

c) I first need to pull those changes down, with `git pull` then can try `git push` again, unless there is a conflict.



## 6. Burn it all!

`git reset --hard HEAD`

The `--hard` means get rid of changes, allows it to lose work.

`HEAD` as reference to say we want to go back to how the project folder was at the last commit, before any edits were made.

## 7. (Sort of) Burn it all!
`git reset --soft HEAD~`

`--soft` means keep the changed files, `HEAD~` means go back one before the current commit.

## 8. Ignore it all!

Neatest `.gitignore` file:
```bash
* # ignore everything
!hello.html # but not this
```

This would work too:
```bash
.DS_Store
images
index.html
.Thumb_db
super-secret-config.php
```

## 9. Describe the process

```bash
git checkout development
git pull
git branch {feature branch}
git checkout {feature branch}
// [do work]
git commit -am "{commit message}"
git push origin {feature branch}
// Go to GitHub
// Find your branch in Code > Branches
// Create pull request for your branch (going into development branch)
// Continue with next task (starting with git checkout development)
```

## 10. npm & gulp

You would likely bring `package.json` and `gulpfile.js` over from a previous project to then use `npm install` to download all the dependencies into `node_modules` and allow you to use your gulp tasks.

## 11. Git, npm & gulp

`.gitignore` file:
This would work too:

```bash
.Thumbs.db
my\ secret\ passwords.txt
node_modules
```

## 12. Gulp and git

We'd look to fix conflicts in `/scss/_headings.scss` and `about.html`.

Then we can run our gulp task again to overwrite `/css/styles.min.css`, rebuilding it with any recent changes from `/scss/_headings.scss`.
