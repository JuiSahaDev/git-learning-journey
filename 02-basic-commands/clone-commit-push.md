# Clone, Commit, and Push in Git

## 1. Clone a Repository
Use the following command to clone a remote repository to your local machine:
```bash
git clone https://github.com/your-username/your-repo.git
# Example:
git clone https://github.com/JuiSahaDev/git-learning-journey.git
```

## 2. Check Repository Status
To view changes (staged, unstaged, untracked):
```bash
git status
```

## 3. Stage Files
To stage a specific file:
```bash
git add filename.ext
# Example:
git add 02-basic-commands/clone-commit-push.md
```
To stage all changed files:
```bash
git add .
```

## 4. Commit Changes
To commit staged files with a message:
```bash
git commit -m "Your commit message"
# Example:
git commit -m "Add basic Git commands: clone, add, commit, push"
```

## 5. Push to Remote Repository
To push your committed changes to the remote repository:
``` bash
git push origin main
# Make sure your current branch is main. If it's something else (e.g., master, dev), replace main accordingly.
```

## 6. Summary of Workflow
```bash
git status           # Check current changes
git add .            # Stage all changes
git commit -m "..."  # Commit with a message
git push origin main # Push to remote
```





