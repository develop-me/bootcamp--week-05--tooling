# Quiz

## Rules

- Some questions you can setup your own test project directory to match the question setup.
- Draw from or add into your own notes.

---

## 1. Getting setup with Git

What does this command do?

`git remote add origin git@github.com:develop-me/drupal1.git`

Think about what each of these parts tells us:
a) `git remote add origin`
b) `git@github.com`
c) `develop-me`
d) `drupal1.git`


## 2. Committing files

Here is the state of our project directory after running `git status`:

```bash
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   hello.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	images/
	index.html
```

What commands would I run to first commit the `images` folder and `index.html` with message `"Apple"` and then, on the next commit, have `hello.html` with message `"Banana"`?

## 3. Reading Git messages: Oh noes #1

```bash
To github.com:develop-me/git-simple.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:develop-me/git-simple.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

a) What command have I just run?

b) What has gone wrong?

c) What should I do next?

## 4. Reading Git messages: Oh noes #2

```bash
remote: Enumerating objects: 38, done.
remote: Counting objects: 100% (38/38), done.
remote: Compressing objects: 100% (16/16), done.
remote: Total 53 (delta 26), reused 31 (delta 22), pack-reused 15
Unpacking objects: 100% (53/53), done.
From github.com:develop-me/git-simple
   6f630d7..7176d81  master            -> origin/master
 * [new branch]      addteampagetonews -> origin/addteampagetonews
   1760f80..bacdb99  projectname       -> origin/projectname
Updating 6f630d7..7176d81
error: Your local changes to the following files would be overwritten by merge:
	index.html
Please commit your changes or stash them before you merge.
Aborting
```

a) What command have I just run?

b) What has gone wrong?

c) What should I do next?

## 5. Reading Git messages: Oh noes #3

a) What command have I just run?

b) What has gone wrong?

c) What should I do next?

```bash
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 5 (delta 3), reused 5 (delta 3), pack-reused 0
Unpacking objects: 100% (5/5), done.
From github.com:develop-me/git-simple
   a657ab7..d6b1aa1  master     -> origin/master
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
```
## 6. Burn it all!

How do you 'throw away' all work since last commit, and revert to how the files were at that moment?

*Note: what humorous website was referenced to help you recover from Git mistakes?*

## 7. (Sort of) Burn it all!

How do you 'throw away' the last commit `bbb123`, going back to the commit before last `aaa123`, but keep the files as they are (i.e. the changes as they are respresentated in commit `bbb123`), to not lose that work.

## 8. Ignore it all!

Create a .gitignore file that will cause Git to only track hello.html in my folder:
