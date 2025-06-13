# Git Branching and Merging
There are few steps

## Step 1: Create a new branch
```bash
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
git push origin feature-branch #push if the new branch added in the github
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