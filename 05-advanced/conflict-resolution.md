# Conflict Resolution

## 
What is a Merge Conflict?
A **merge conflict** occurs when Git is unable to automatically 
reconcile differences between two branches. This typically happens 
when two branches have changes in the same part of a file, 
or when a file is deleted in one branch but modified in another.

## Common Causes of Merge Conflicts

- Multiple people editing the same line of a file.
- A file edited in one branch and deleted in another.
- Concurrent renaming or restructuring of files/directories.
- Long-lived branches diverging significantly from `main`.

---

## How to Detect Conflicts

During a `git merge` or `git pull`, Git will pause and output something like:

#Best Practices to Avoid Conflicts
Pull changes from main frequently and rebase.
Communicate with your team about who’s working on what.
Make small, frequent commits with focused changes.
Avoid large-scale file renaming or restructuring without coordination.
Resolve conflicts immediately rather than postponing.


For example,
You are working on a feature-branch. You change some files. So, you don't commit your work into the main branch directly — that’s not safe!

Here’s what you do instead:

Before starting your task, you run:

```bash
git pull origin main
This brings the latest changes from main into your local machine. So your feature branch stays up to date.
```
Then, you make changes to your files while staying in your feature-branch.

After finishing your task, you commit your changes:
```bash
git add .
git commit -m "Completed: Added new feature"
```
Then, for safety and backup, you push it to your remote feature-branch:

```bash
git push origin feature-branch
```
Once everything is safe and tested, and no conflict exists —
You switch to main:

```bash
git checkout main
```
Again, pull the latest from remote (if teammates made changes to main):
```bash
git pull origin main
```
Now, merge your feature branch into main:
```bash
git merge feature-branch
````
And finally, push the updated main to GitHub:
```bash
git push origin main
````