# Git Commands
---
---

## Commits
---
git status shows the current status of your repo. It will show you if you have any work that is unstaged, what branch you are on, how many commits you are ahead of the master remote on github, and other useful things
git log --oneline lists all commits with their Ids in short format for branch you are on


### Reset or Revert to Previous Commits
git reset <commit id> resets commits history, but doesnt change files. Commit history is lost
git reset <commit id> --hard resets commit history and changes files. Commit history is lost

git revert <commit id> reverts to state at commit id, but tracks the reversion in the commit history

## Branches
---
git checkout -b <new branch name> creates new branch and switches to that branch
git branch shows local branches
git branch -r shows remote branches

git branch -d <local branch>
git push origin  --delete <remote branch name>

## Remotes
---
git remote add <local remote name> <remote url> adds remote to local
git remote -v shows all remotes, v stands for verbose which includes urls

git fetch <remote> pulls data from all remote branches, but leaving local working directory intact
git fetch <remote> <branch> same as above but only specified branch

git merge <name-of-branch> will merge the specified branch into the branch you are currently on

git push -u <remote> <remote branch name> pushes all commits to the upstream remote
