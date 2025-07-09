# Git Commands A-Z

A complete reference of essential Git commands, designed to help you efficiently manage your version control workflow. This guide is ideal for beginners and experienced developers alike.

📍 **Repository URL:** [https://github.com/tanvirsweb/git_commands_A-Z](https://github.com/tanvirsweb/git_commands_A-Z)

👤 **Author:** [Tanvir Anjom Siddique, BSc in CSE from RUET](https://tanvirsweb.github.io)

---

## ✅ Git Commands in Sequential Workflow

This table outlines a typical Git workflow with commands listed in a logical order, ensuring clarity for beginners and advanced users. Each command includes a description and the reason for its use.

| Step | Command                                            | Description                                              | Reason                                                                                          |
| ---- | -------------------------------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| 1    | `git config --global user.name "Your Name"`        | Sets your name globally for all Git commits.             | Identifies you as the author of commits across all repositories.                                |
| 2    | `git config --global user.email "you@example.com"` | Sets your email globally for all Git commits.            | Links commits to your GitHub or other Git identity.                                             |
| 3    | `git config user.name "Local Name"`                | Sets username for the current repository only.           | Overrides global config for specific projects (e.g., work vs personal).                         |
| 4    | `git config user.email "local@example.com"`        | Sets email for the current repository only.              | Useful for projects requiring different credentials.                                            |
| 5    | `cd /path/to/project`                              | Navigates to your project folder.                        | Prepares your terminal for Git operations.                                                      |
| 6    | `git init`                                         | Initializes a Git repository in the current directory.   | Starts local version control for your project.                                                  |
| 7    | `git clone <repo-url>`                             | Copies a remote repository to your local machine.        | Starts collaboration on an existing project or sets up a local copy.                            |
| 8    | `git remote add origin <url>`                      | Links local repo with a remote named origin.             | Enables pushing to or pulling from GitHub or other platforms.                                   |
| 9    | `git remote -v`                                    | Shows added remotes with fetch/push info.                | Verifies that the remote is set correctly.                                                      |
| 10   | `git remote set-url origin <url>`                  | Updates the remote origin URL.                           | Corrects wrong remotes or switches between SSH/HTTPS.                                           |
| 11   | `git fetch`                                        | Downloads remote data without merging.                   | Syncs local repo with remote changes for review before pulling.                                 |
| 12   | `git fetch origin`                                 | Fetches data from a specific remote.                     | Ensures local repo is aware of the latest remote changes.                                       |
| 13   | `git branch`                                       | Lists all local branches.                                | Helps you view and manage branches in your repository.                                          |
| 14   | `git branch -r`                                    | Lists all remote-tracking branches.                      | Shows branches available on the remote (e.g., GitHub).                                          |
| 15   | `git branch -M main`                               | Renames the current branch to main.                      | Aligns with modern default branch naming conventions.                                           |
| 16   | `git checkout -b branch-name`                      | Creates and switches to a new branch.                    | Starts a new feature or bugfix branch for isolated development.                                 |
| 17   | `git checkout branch-name`                         | Switches to an existing branch.                          | Moves between branches (e.g., from feature to main).                                            |
| 18   | `git add .`                                        | Stages all modified and new files for commit.            | Prepares all changes in the working directory for committing.                                   |
| 19   | `git add filename.txt`                             | Stages a specific file.                                  | Allows selective staging of individual files.                                                   |
| 20   | `git add *.js`                                     | Stages all files matching a pattern (e.g., JavaScript).  | Efficiently stages specific file types.                                                         |
| 21   | `git status`                                       | Shows current file states (staged, unstaged, untracked). | Provides an overview before committing or pushing.                                              |
| 22   | `git diff`                                         | Shows changes in working directory vs. last commit.      | Helps review modifications before staging.                                                      |
| 23   | `git diff filename.txt`                            | Compares a file’s working copy with the last commit.     | Pinpoints changes in a specific file.                                                           |
| 24   | `git diff branch-name`                             | Compares current branch with another branch.             | Verifies differences before merging.                                                            |
| 25   | `git reset filename.txt`                           | Unstages a staged file.                                  | Undoes `git add` while keeping file changes.                                                    |
| 26   | `git restore filename.txt`                         | Discards local changes to a file.                        | Reverts file to its last committed state (use with caution).                                    |
| 27   | `git commit -m "Message"`                          | Records staged changes in the repository.                | Creates a snapshot of your project’s current state.                                             |
| 28   | `git commit --amend -m "New msg"`                  | Modifies the last commit’s message or content.           | Corrects typos or includes missed changes in the last commit.                                   |
| 29   | `git push -u origin main`                          | Pushes local main and sets upstream tracking.            | Syncs local main with remote and enables tracking.                                              |
| 30   | `git push --set-upstream origin branch-name`       | Pushes and sets upstream for a new branch.               | Required when pushing a new branch for the first time.                                          |
| 31   | `git push origin main`                             | Pushes updates to the remote main branch.                | Updates the shared repository with local changes.                                               |
| 32   | `git push --force`                                 | Overwrites remote history with local changes.            | Required after amending or rebasing (use cautiously).                                           |
| 33   | `git pull origin main`                             | Pulls latest changes from remote main.                   | Keeps local main branch updated with remote changes.                                            |
| 34   | `git pull origin main --allow-unrelated-histories` | Merges unrelated project histories.                      | Combines local and remote repos started independently.                                          |
| 35   | `git merge branch-name`                            | Merges another branch into the current branch.           | Integrates feature or bugfix changes into main.                                                 |
| 36   | `git merge --abort`                                | Cancels an in-progress merge.                            | Resolves issues when merge conflicts are unmanageable.                                          |
| 37   | `git log`                                          | Shows detailed commit history.                           | Reviews previous commits and their details.                                                     |
| 38   | `git log --oneline`                                | Shows commit history in a compact, single-line format.   | Simplifies scanning of commit history.                                                          |
| 39   | `git log --merge`                                  | Shows conflicting commits during a merge.                | Helps identify and resolve merge conflicts.                                                     |
| 40   | `git reset --soft HEAD~1`                          | Undoes last commit, keeps changes staged.                | Allows re-editing or re-committing changes.                                                     |
| 41   | `git reset --mixed HEAD~1`                         | Undoes last commit and unstages changes.                 | Resets staging area but keeps working directory changes.                                        |
| 42   | `git reset --hard HEAD~1`                          | Removes last commit and discards changes.                | Irreversibly discards changes (use with extreme caution).                                       |
| 43   | `git cherry-pick <commit-hash>`                    | Applies a specific commit from another branch.           | Selectively reuses commits from other branches.                                                 |
| 44   | `git revert <commit-hash>`                         | Creates a new commit to undo a previous one.             | Safely reverses changes without altering history. Commit has can be found by `git log` command. |
| 45   | `git branch -d branch-name`                        | Deletes a local branch (safe, only if merged).           | Cleans up branches after merging.                                                               |
| 46   | `git branch -D branch-name`                        | Force deletes a local branch (unmerged).                 | Removes branches even if not merged (use cautiously).                                           |
| 47   | `git push origin --delete branch-name`             | Deletes a branch from the remote repository.             | Cleans up merged or obsolete branches on GitHub.                                                |
| 48   | `git fetch -p`                                     | Prunes deleted remote branches from local metadata.      | Removes stale references to deleted remote branches.                                            |
| 49   | `git stash`                                        | Temporarily saves uncommitted changes.                   | Allows switching branches without committing incomplete work.                                   |
| 50   | `git stash pop`                                    | Restores and removes the most recent stashed changes.    | Reapplies saved changes and clears the stash.                                                   |
| 51   | `git stash list`                                   | Lists all stashed changes.                               | Reviews saved stashes before applying or dropping.                                              |
| 52   | `git stash drop`                                   | Deletes the most recent stash.                           | Removes unneeded stashed changes.                                                               |
| 53   | **GitHub Pull Request (GUI)**                      | Compare branches on GitHub → Create PR.                  | Facilitates collaboration and code review before merging.                                       |
| 54   | **GitHub Fork (GUI)**                              | Click Fork on a repo.                                    | Creates a personal copy of a repo for contributing changes.                                     |

---

## 🔧 Resolving Merge Conflicts

Merge conflicts occur when Git cannot automatically reconcile changes from two branches. Follow these steps to resolve them:

1. Attempt the merge and encounter a conflict:

   ```bash
   git merge feature-branch
   ```

2. Git will notify you about conflicts in specific files.

3. Open the conflicted files and look for conflict markers:

   ```
   <<<<<<< HEAD
   // Your current branch (e.g., main) changes
   =======
   // Changes from the feature-branch
   >>>>>>> feature-branch
   ```

4. Manually edit the file to keep the desired lines, removing the conflict markers.

   ```
   // Your current branch (e.g., main) changes
   // Changes from the feature-branch
   ```

5. Stage the resolved files:

   ```bash
   git add filename
   ```

6. Commit the resolution:

   ```bash
   git commit -m "resolve merge conflict"
   ```

7. Push the final version to the remote:

   ```bash
   git push origin main
   ```

---

## 🔍 Examples for Common Operations

### 1–4. Configure Git Identity

Set your global identity to associate commits with your name and email (used by platforms like GitHub):

```bash
git config --global user.name "Tanvir Anjom Siddique"        # Sets your name for all repositories
git config --global user.email "tanvir.anjom.siddique@gmail.com"  # Sets your email for all repositories

# Override locally if needed
git config user.name "Tanvir Work"                           # Overrides name for current repo
git config user.email "work@example.com"                     # Overrides email for current repo
```

---

### 5–7. Initialize or Clone a Repository

Start a new Git repository or clone an existing one:

```bash
cd ~/projects/practiceGit          # Navigate to your project directory
git init                         # Initialize an empty Git repository
```

Alternatively, clone an existing repository:

```bash
git clone https://github.com/tanvirsweb/gitPractice.git    # Copies remote repo locally
cd gitPractice                   # Move into the cloned directory
```

---

### 8–10. Connect to a Remote Repository

Link your local repository to a remote (e.g., GitHub):

1. Visit your GitHub profile: [https://github.com/tanvirsweb](https://github.com/tanvirsweb)
2. Click the **+** icon in the top-right corner and select **New repository**.
3. Create a new repository named: `gitPractice`
4. Click **Create repository** (no need to initialize with README, .gitignore, or license)

Then run the following commands in your terminal:

```bash
git remote add origin https://github.com/tanvirsweb/gitPractice.git  # Link remote repository
git remote -v                                                        # Verify the remote URL
git remote set-url origin git@github.com:tanvirsweb/gitPractice.git  # (Optional) Switch to SSH if preferred
```
---

### 11–15. Create and Commit Files

Create files, stage, and commit them:

```bash
echo "# My Project" > README.md    # Create a README file
git add README.md                  # Stage the README file
git commit -m "Initial commit"    # Commit with a descriptive message
git branch -M main                 # Rename default branch to 'main'
git push -u origin main            # Push to remote and set upstream tracking
```

If your local project has commits but the remote has initial commits (e.g., a README or license):

```bash
git pull origin main --allow-unrelated-histories  # Merge local and remote histories
```

---

### 16–17. Feature Branch Workflow

Create a new branch for isolated development:

```bash
git checkout -b feature-branch            # Create and switch to feature branch
echo "New feature" >> feature.txt         # Add content to a new file
git add .                                 # Stage all changes
git commit -m "Add feature"               # Commit changes
git push --set-upstream origin feature-branch  # Push branch and set tracking
```

---

### 18–22. Merge Feature Branch and Clean Up

Merge the feature branch into main and clean up:

```bash
git checkout main                         # Switch to main branch
git pull origin main                      # Ensure main is up-to-date
git merge feature-branch                  # Merge feature branch into main
git push origin main                      # Push merged changes to GitHub
git branch -d feature-branch              # Delete local feature branch
git push origin --delete feature-branch   # Delete remote feature branch
```

---

### 23–25. Amend a Commit

Fix or update the last commit:

```bash
git commit --amend -m "Updated message"  # Modify last commit
git push --force                         # Overwrite remote history (caution!)
```

---

### 26–28. Explore Commit History

Review the project’s commit history:

```bash
git fetch origin                        # Fetch latest remote metadata
git log --oneline                      # Compact commit history view
git log --merge                        # View commits causing merge conflicts (if any)
```

---

### 29–31. Work with Stashes

Temporarily save and restore uncommitted changes:

```bash
git stash                              # Save uncommitted changes
git checkout main                      # Switch branches without losing work
git stash pop                         # Reapply stashed changes
git stash list                        # List all stashed changes
git stash drop                        # Delete the most recent stash
```

---

### 32–34. Selective Staging and Discarding Changes

Stage specific files or revert changes:

```bash
git add file1.py                      # Stage a specific file
git add *.html                       # Stage all HTML files
git restore file1.py                 # Discard changes to a file (reverts to last commit)
```

---

### 35–36. Revert or Cherry-Pick Commits

Undo or reuse specific commits:

```bash
git log                               # get info of commits and hash
git revert <commit-hash>              # Create a new commit to undo a previous one
git cherry-pick <commit-hash>         # Apply a specific commit from another branch
```

---

### 37–39. Clean Up Remote and Local Branches

Remove obsolete branches:

```bash
git fetch -p                        # Prune stale remote-tracking branches
git branch -D feature-branch        # Force delete local branch
git push origin --delete feature-branch  # Delete remote branch
```

---

### 40–41. Compare Changes

Review differences before committing or merging:

```bash
git diff                          # View all changes in working directory
git diff main feature-branch      # Compare two branches
```

---

### 42–43. Resolve Merge Conflicts (Detailed)

If a merge results in conflicts:

```bash
git merge feature-branch            # Attempt merge, triggers conflicts

# Open conflicted files, edit to remove conflict markers (<<<<<<<, =======, >>>>>>>)

git add resolved-file.py            # Stage resolved files
git commit -m "Resolved merge conflict"  # Commit resolution
git push origin main                # Push changes
```

---

## 📦 Clone This Repository

Get this guide on your local machine:

```bash
git clone https://github.com/tanvirsweb/git_commands_A-Z.git
cd git_commands_A-Z
```

---

## 🙌 Contributing

Contributions are welcome! To contribute:

1. Fork the repository on GitHub.

2. Create a feature branch:

   ```bash
   git checkout -b my-contribution
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add my contribution"
   ```

4. Push to your branch:

   ```bash
   git push origin my-contribution
   ```

5. Create a Pull Request on GitHub.

Suggestions, additional commands, or improvements are greatly appreciated!

---

## 🔖 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🌐 Connect with Me

- 💼 [LinkedIn](https://bd.linkedin.com/in/tanvir-anjom-siddique)
- 💻 [GitHub](https://github.com/tanvirsweb)
- 🌍 [Portfolio](https://tanvirsweb.github.io/)

---
