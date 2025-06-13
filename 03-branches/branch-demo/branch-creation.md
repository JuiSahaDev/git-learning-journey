# Branch Creation Demo – branch-creation.md
This document demonstrates how to work with Git branches. Follow the steps to create, list, switch, and delete branches.

## 1. Check Current Branch
This will list all local branches. The currently checked-out branch will be highlighted with an asterisk (*).
```bash
git branch
```
---
## 2. Create a New Branch
This creates a new branch named feature-branch from the current HEAD.
```bash
git branch feature-branch
```
---
## 3. Switch to the New Branch
This switches your working directory to the feature-branch branch.
```bash
git checkout feature-branch
```
### Shortcut (Git 2.23+):
```bash
git switch feature-branch
```
---
## 4. Create and Switch in One Command
This creates a new branch feature-2 and checks it out in one step.
```bash
git checkout -b feature-2
```
### Shortcut (Git 2.23+):
```bash
git switch -c feature-2
```
---
## 5. View All Branches (Including Remote)
This shows local and remote-tracking branches.
```bash
git branch -a
```
---

## 6. Delete a Branch
Deletes the feature-branch branch safely (only if it’s fully merged).
```bash
git branch -d feature-branch
```
### Force delete (if not merged):
```bash
git branch -D feature-branch
```