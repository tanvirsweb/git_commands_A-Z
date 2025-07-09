# git_commands_A-Z

A complete reference of essential Git commands, designed to help you efficiently manage your version control workflow. This guide is ideal for beginners and experienced developers alike.

📍 **Repository URL:** [`https://github.com/tanvirsweb/git_commands_A-Z`](https://github.com/tanvirsweb/git_commands_A-Z.git)

---

👤 **Author**: [Tanvir Anjom Siddique, BSc in CSE from RUET](https://tanvirsweb.github.io)

## ✅ Git Commands in Sequential Workflow

| Step | Command                                            | Description                                              | Reason                                                          |
| ---- | -------------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------------------- |
| 1    | `git config --global user.name "Your Name"`        | Sets your name globally for all Git commits.             | Used to identify you as the author of commits across all repos. |
| 2    | `git config --global user.email "you@example.com"` | Sets your email globally for all Git commits.            | Links commits to your GitHub/Git identity.                      |
| 3    | `git config user.name "Local Name"`                | Sets username for current repository only.               | Overrides global config locally.                                |
| 4    | `git config user.email "local@example.com"`        | Sets email for current repository only.                  | Useful when using different credentials per project.            |
| 5    | `cd /path/to/project`                              | Navigate to your project folder.                         | Prepares your terminal for Git operations.                      |
| 6    | `git init`                                         | Initializes a Git repository in the current directory.   | Starts local version control.                                   |
| 7    | `git add .`                                        | Stages all files for commit.                             | Prepares files to be committed.                                 |
| 8    | `git status`                                       | Shows current file states (staged, unstaged, untracked). | Useful before every commit or push.                             |
| 9    | `git commit -m "Initial commit"`                   | Records changes to the repository.                       | Creates a snapshot of your project.                             |
| 10   | `git branch`                                       | Lists all local branches.                                | Lets you view and manage branches.                              |
| 11   | `git branch -M main`                               | Renames the current branch to `main`.                    | Modern default branch name for compatibility.                   |
| 12   | `git remote add origin <url>`                      | Links local repo with a remote named `origin`.           | Enables pushing to GitHub or other platforms.                   |
| 13   | `git remote -v`                                    | Shows added remotes with fetch/push info.                | Confirms remote is set correctly.                               |
| 14   | `git push --set-upstream origin main`              | Pushes local `main` and sets upstream.                   | Enables tracking with remote branch.                            |
| 15   | `git commit --amend -m "New msg"`                  | Modifies last commit message or content.                 | Corrects typos or adds missed changes.                          |
| 16   | `git push --force`                                 | Pushes amended commits (overwrites history).             | Required after amend or rebase.                                 |
| 17   | `git checkout -b feature-branch`                   | Creates and switches to a new branch.                    | For new features or fixes.                                      |
| 18   | `git add .`                                        | Stages changes in new branch.                            | Required before committing.                                     |
| 19   | `git commit -m "Add feature"`                      | Commits the new changes.                                 | Saves a feature-specific snapshot.                              |
| 20   | `git push --set-upstream origin feature-branch`    | Pushes and tracks the new branch.                        | Shares feature branch to remote.                                |
| 21   | `git checkout main`                                | Switches back to the main branch.                        | Prepares for merging.                                           |
| 22   | `git pull origin main`                             | Updates local main with remote.                          | Avoids merge conflicts.                                         |
| 23   | `git merge feature-branch`                         | Merges another branch into current.                      | Combines changes into main.                                     |
| 24   | `git push origin main`                             | Pushes merged updates to remote main.                    | Updates shared repository.                                      |
| 25   | `git reset --soft HEAD~1`                          | Undo last commit, keep changes staged.                   | For re-editing and re-committing.                               |
| 26   | `git reset --mixed HEAD~1`                         | Undo commit and unstage changes.                         | Re-select files to commit.                                      |
| 27   | `git reset --hard HEAD~1`                          | Remove last commit and changes.                          | Irreversibly discards changes.                                  |
| 28   | `git log`                                          | Shows commit history.                                    | View previous commits.                                          |
| 29   | `git diff main`                                    | Compares current branch with `main`.                     | Helps verify changes before merge.                              |
| 30   | `git pull origin branch-name`                      | Pulls changes from a remote branch.                      | Syncs local with remote.                                        |
| 31   | `git checkout another-branch`                      | Switches to a different branch.                          | For multitasking with branches.                                 |
| 32   | `git branch -d branch-name`                        | Deletes a local branch (safe).                           | After merge and cleanup.                                        |
| 33   | `git branch -D branch-name`                        | Force deletes branch (unsafe).                           | Deletes without merge.                                          |
| 34   | `git cherry-pick <commit-hash>`                    | Applies one commit from another branch.                  | Selectively reuse commits.                                      |
| 35   | `git log --merge`                                  | Shows conflicting commits during a merge.                | Helps identify merge conflicts.                                 |
| 36   | **GitHub Pull Request (GUI)**                      | Compare branches on GitHub → Create PR.                  | Collaborate and review before merging.                          |
| 37   | `git revert <commit-hash>`                         | Undoes a commit by creating a new one.                   | Safe way to reverse changes.                                    |
| 38   | **GitHub Fork (GUI)**                              | Click **Fork** on a repo.                                | Copies repo to your account for changes.                        |

---

## 🔍 Examples for Common Operations

### 1–4. Set Git Username and Email

```bash
git config --global user.name "Tanvir Anjom Siddique"
git config --global user.email "tanvir@example.com"

git config user.name "Tanvir Local"
git config user.email "tanvir.local@example.com"
```

---

### 5–6. Navigate and Initialize Repo

```bash
cd ~/projects/git_commands_A-Z
git init
```

---

### 7–9. Stage and Commit Changes

```bash
git add .
git status
git commit -m "Initial commit"
```

---

### 10–14. Branch Rename and Remote Setup

```bash
git branch
git branch -M main
git remote add origin https://github.com/tanvirsweb/git_commands_A-Z.git
git remote -v
git push --set-upstream origin main
```

---

### 15–16. Amend Last Commit

```bash
git commit --amend -m "Fix typo in README"
git push --force
```

---

### 17–20. Create Feature Branch and Push

```bash
git checkout -b login-feature
git add .
git commit -m "Add login page UI"
git push --set-upstream origin login-feature
```

---

### 21–24. Merge Feature Branch to Main

```bash
git checkout main
git pull origin main
git merge login-feature
git push origin main
```

---

### 25–27. Undo Commits

```bash
# Soft
git reset --soft HEAD~1

# Mixed
git reset --mixed HEAD~1

# Hard
git reset --hard HEAD~1
```

---

### 28–29. Logs and Differences

```bash
git log
git diff main
```

---

### 30–31. Pull and Checkout Branch

```bash
git pull origin login-feature
git checkout login-feature
```

---

### 32–33. Delete Branches

```bash
git branch -d login-feature
git branch -D debug-branch
```

---

### 34. Cherry-pick a Commit

```bash
git cherry-pick 9fceb02
```

---

### 35. Check Merge Conflicts

```bash
git log --merge
```

---

### 36. GitHub Pull Request (GUI)

1. Push your branch.
2. Open the repo on GitHub.
3. Click **Compare & pull request**.
4. Write description and click **Create pull request**.

---

### 37. Revert a Commit

```bash
git revert 9fceb02
```

---

### 38. Fork a Repository

1. Go to the repo page on GitHub.
2. Click the **Fork** button (top-right).
3. Choose your GitHub account to create a forked copy.

---

## 📦 Clone This Repository

```bash
git clone https://github.com/tanvirsweb/git_commands_A-Z.git
```

---

## 🙌 Contributing

Feel free to fork, improve, and contribute! Suggestions and pull requests are welcome.

---

## 🔖 License

This project is open-source and available under the [MIT License](LICENSE).
