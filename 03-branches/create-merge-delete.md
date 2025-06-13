# Git Branching and Merging
There are few steps

## Step 1: Create a new branch
Run this command to create a new branch:
```bash
git branch branch-name
# Example:
git branch feature-branch
```

Use this command to switch branches:
```bash
git checkout branch-name
# Example:
git checkout feature-branch
```

Alternatively, create and switch in one step:
```bash
git checkout -b branch-name
# Example:
git checkout -b feature-branch
```

## Step 2: Make some changes
Create or edit a file
```bash
echo "This is a new feature" > feature.txt
```

## Step 3: Stage and commit the change
```bash
git add .
git commit -m "Add changes in feature branch"
```

## Step 4: Switch back to main branch
```bash
git checkout main
```

### Step 5: Merge the feature branch into main
```bash
git merge feature-branch
```

## Step 6: Push the changes to GitHub
```bash
git push
```

## Step 7: (Optional) Delete the feature branch
```bash
git branch -d feature-branch
```