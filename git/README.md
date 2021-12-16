# Git

Just a repo that stores frequently used commands from Git

## ⛑ Status

#### Check status

This command will show the current status of the local repo.

```
git status
```

#### View logs

This command will show all commit logs.

```
git log
```

## 🪵 Branch

#### Fetch latest info from remote

This command will show latest info from remote Github repo (won't touch the files in local repo).

```
git fetch origin
```

#### Pull latest changes from remote

This command will pull latest changes from remote Github repo (will touch the files in local repo, sometimes will occur conflict if latest changes and local file have make change in same line).

```
git pull
```

#### Merge branch

This command will merge other branch into current branch.

###### Fast-forward (Does not generate merge commit)

```
git merge <<another_branch>>
```

###### No Fast-forward (Generate merge commit)

```
git merge --no-ff <<another_branch>>
```

#### Fetch latest branch from remote

This command will show all latest branches from remote Github repo.

```
git fetch -p
```

#### Create & switch to new branch

This command will create and switch to new branch

###### Method 1

```
git checkout -b <<branch_name>>
```

###### Method 2

```
git switch -c <<branch_name>>
```

#### Create new branch & copy content from a remote branch

This command will create a new branch and also copy all contents from a remote branch.

```
git checkout -b <<new_local_branch_name>> <<origin/remote_branch_name>>
```

#### View all local branches

This command will show all local branches of project repo.

```
git branch
```

#### View all local & remote branches

This command will show all local and remote branches of project repo.

```
git branch -a
```

#### Switch branch

This command will switch to another branch.

```
git [switch/checkout] <<branch_name>>
```

#### Delete branch locally

This command will delete a branch locally

```
git branch -d <<branch_name>>
```

#### Delete branch remotely

This command will delete a branch remotely

```
git push origin --delete <<branch_name>>
```

#### Go back to a specific commit

This command will create a commit and go back to specific commit. Yes, this method will leave the records instead of delete it completely from repo. However, this method is a lot **safer** than `git reset`, especially you're working with other people.

```
git revert <<commit_hash>>
```

#### Squash X commits into 1

This command will let you go back X commits by resetting git index to before the commits you want to squash. Use `--soft` so that git only resets the index and doesn't touch your working directory. Then create a commit as usual. [source from stackoverflow](https://stackoverflow.com/a/50302458/10868150)

```
git reset --soft HEAD~<<X>> // go back X commits
git add --all // Add the changes
git commit 
git push --force 
```
