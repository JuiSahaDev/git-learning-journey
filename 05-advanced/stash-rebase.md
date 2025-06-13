# Git Stash and Rebase

## 1. What is `git stash`?

`git stash` temporarily shelves (or stashes) changes you've made to your working directory, so you can work on something else and come back to them later.

### Typical Use Case:

You’re working on a feature but suddenly need to switch branches without committing your changes.

```bash
git stash
git checkout main
# Do your task on main
git checkout feature-branch
git stash pop  # Bring your changes back
```

##  2. What is git rebase?
git rebase is used to integrate changes from one branch into another. Unlike merge, it rewrites the commit history to create a linear sequence.

### Typical Use Case:
You want to update your feature branch with the latest changes from main.
```bash
git checkout feature-branch
git fetch origin
git rebase origin/main
```
If conflicts occur, Git will stop and ask you to resolve them. After resolving:
```bash
git add .
git rebase --continue
```
To abort the rebase:
```bash
git rebase --abort
```