**`git_commands_A-Z`** hosted at `https://github.com/tanvirsweb/git_commands_A-Z`. It covers all the essential Git commands you might need for your workflow from initialization, commits, branches, merges, amending commits, to undoing commits.

---

## [Click here to View Detailed git_commands_A-Z webpage](https://tanvirsweb.github.io/git_commands_A-Z/)

# git_commands_A-Z

This repository contains a complete set of Git commands and instructions to help you manage your workflow efficiently. It covers everything from repository creation, committing changes, branching, merging, and undoing commits.

---

## Repository URL

[`https://github.com/tanvirsweb/git_commands_A-Z.git`](https://github.com/tanvirsweb/git_commands_A-Z.git)

---

## 1. Initialize Local Git Repository

```bash
# Navigate to your project folder
cd /path/to/git_commands_A-Z

# Initialize a new Git repository locally
git init
```

---

## 2. Add Files and Make Your First Commit

```bash
# Stage all files for commit
git add .

# Commit files with a descriptive message
git commit -m "Initial commit"
```

---

## 3. Add Remote Repository and Push to GitHub

```bash
# Add remote repository URL
git remote add origin https://github.com/tanvirsweb/git_commands_A-Z.git

# Push your local main branch to remote and track upstream
git push --set-upstream origin main
```

---

## 4. Amend the Last Commit (Update Message or Content)

```bash
# If you want to change files, edit them, then stage changes
git add <file(s)>

# Amend the last commit (to change message or add files)
git commit --amend -m "Updated commit message"

# Force push amended commit to remote repository
git push --force
```

---

## 5. Create a New Branch, Switch to It, and Commit

```bash
# Create and switch to a new branch named 'feature-branch'
git checkout -b feature-branch

# Make changes and stage them
git add .

# Commit your changes
git commit -m "Add new feature in feature-branch"

# Push new branch to remote and set upstream tracking
git push --set-upstream origin feature-branch
```

---

## 6. Merge Branches

### Merge `feature-branch` into `main`

```bash
# Switch to the main branch
git checkout main

# Pull latest changes from remote main branch
git pull origin main

# Merge the feature branch into main
git merge feature-branch

# Push merged changes to remote main
git push origin main
```

---

## 7. Undo Commits

### Undo the Last Commit but Keep Changes Staged

```bash
git reset --soft HEAD~1
```

### Undo the Last Commit and Unstage Changes (keep file changes)

```bash
git reset --mixed HEAD~1
```

### Undo the Last Commit and Discard Changes (irreversible!)

```bash
git reset --hard HEAD~1
```

---

## Quick Reference Table

| Operation                      | Command                               |
| ------------------------------ | ------------------------------------- |
| Initialize repository          | `git init`                            |
| Stage all files                | `git add .`                           |
| Commit changes                 | `git commit -m "message"`             |
| Amend last commit              | `git commit --amend -m "new message"` |
| Force push after amend         | `git push --force`                    |
| Create and switch branch       | `git checkout -b branch-name`         |
| Switch branch                  | `git checkout branch-name`            |
| Merge branch into current      | `git merge branch-name`               |
| Undo last commit (soft reset)  | `git reset --soft HEAD~1`             |
| Undo last commit (mixed reset) | `git reset --mixed HEAD~1`            |
| Undo last commit (hard reset)  | `git reset --hard HEAD~1`             |

---

Feel free to clone this repository and use the commands above to manage your Git workflow efficiently.

---

**Clone the repo:**

```bash
git clone https://github.com/tanvirsweb/git_commands_A-Z.git
```

---
