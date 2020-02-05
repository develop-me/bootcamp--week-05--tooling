## Git
- git looks "up the path"
- best practices
- sense check with `git status` often
- atomic commits: use git commit -a sparingly
- read error messages
- post-PR merge: git remote prune origin & git branch -d
- quiz answers + explanation
- oh shit resource & exercises
- git autocomplete setup guide
- simplify git-simple site?
- Oh Shit, Git as an exercise? Talk? Demo? (see below)
- difference between git fetch and git pull

Notes:
- rm or mv files
- unstaging a file `git restore --stage {filename}`


## npm/Gulp

gulp built in functions

port 03/00-software-setup.md to pre-Git setup Game


Oh shit, I committed and immediately realized I need to make one small change!
# make your change
git add . # or add individual files
git commit --amend --no-edit
# now your last commit contains that change!
# WARNING: never amend public commits


Oh shit, I need to change the message on my last commit!
git commit --amend
# follow prompts to change the commit message


Oh shit, I accidentally committed something to master that should have been on a brand new branch!
# create a new branch from the current state of master
git branch some-new-branch-name
# remove the last commit from the master branch
git reset HEAD~ --hard
git checkout some-new-branch-name
# your commit lives in this branch now :)


Oh shit, I accidentally committed to the wrong branch!
# undo the last commit, but leave the changes available
git reset HEAD~ --soft
git stash
# move to the correct branch
git checkout name-of-the-correct-branch
git stash pop
git add . # or add individual files
git commit -m "your message here";
# now your changes are on the correct branch


git reset HEAD --hard