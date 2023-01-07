# Git Commands

### Commits
git log --oneline lists all commits with their Ids in short format for branch you are on

#### Reset or Revert to Previous Commits
git reset <commit id> resets commits history, but doesnt change files. Commit history is lost
git reset <commit id> --hard resets commit history and changes files. Commit history is lost

git revert <commit id> reverts to state at commit id, but tracks the reversion in the commit history

### Branches
git branch shows local
git branch -r shows remotes

git branch -d <local branch>
git push origin  --delete <remote branch name>

### Remotes
git remote add <local remote name> <remote url> adds remote to local
git remote -v

git fetch <remote> pulls data from all remote branches, but leaving local working directory intact
git fetch <remote> <branch> same as above but only specified branch
