# Git Commands Cheat Sheet: A to Z Guide
## Basic Setup
`git config`
Set Git configuration values (username, email, editor, etc.)
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --list        # View all configs
```

## Starting a Repo
`git init`
Create a new local Git repository
```bash
git init
```
`git clone`
Clone an existing remote repository
```bash
git clone <repo-url>
# Example:
git clone https://github.com/JuiSahaDev/git-learning-journey.git
```

## Staging & Snapshots
`git status`
Check the status of working directory and staging area
```bash
git status
```

`git add`
Stage changes
```bash
git add <file>
# Example:
git add 02-basic-commands\README-update-demo\README.md

git add .              # Stage all changes
```

`git reset`
Unstage files (move from staged to unstaged)
```bash
git reset <file>
# Example:
git reset 02-basic-commands\README-update-demo\README.md
git reset             # Unstage everything
```

## Committing
`git commit`
Commit staged changes
```bash
git commit -m "Your message"
```

`git commit --amend`
Modify the last commit
```bash
git commit --amend
```

## Pushing & Pulling
git push
Send commits to remote repo
```bash
git push origin main
```

`git pull`
Fetch and merge changes from remote
```bash
git pull origin main
```

`git fetch`
Download commits without merging
```bash
git fetch origin
```

## Branching
`git branch`
List, create, delete branches
```bash
`git branch`                # List branches
git branch <name>         # Create branch
git branch -d <name>      # Delete branch
```

`git checkout`
Switch branches or restore files
```bash
git checkout <branch>
git checkout -b <branch>  # Create and switch
```

`git switch`
A modern alternative to checkout
```bash
git switch <branch>
git switch -c <branch>    # Create and switch
```

## Merging & Rebasing
`git merge`
Merge one branch into another
```bash
git merge <branch>
```

`git rebase`
Reapply commits on top of another base
```bash
git rebase <branch>
```

## History & Logs
`git log`
View commit history
```bash
git log
git log --oneline --graph --all
```

`git diff`
Show changes between commits, branches, files
```bash
git diff
git diff --staged
```

## Cleaning Up
`git clean`
Remove untracked files
```bash
git clean -f
```

## Tags
`git tag`
Tag specific commits
```bash
git tag v1.0
git tag -a v1.0 -m "Version 1.0"
git push origin v1.0
```

## Search
`git grep`
Search text in tracked files
```bash
git grep "function"
```

## Remote Repos
`git remote`
Manage remote connections
```bash
git remote -v
git remote add origin <url>
git remote remove origin
```

## Undo & Fix Mistakes
`git revert`
Revert a specific commit
```bash
git revert <commit-hash>
```

`git restore`
Restore file contents
```bash
git restore <file>
git restore --staged <file>
```