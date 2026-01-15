This file contains a list of commonly used Git commands with short explanations and examples.  
It’s useful for beginners learning how to manage version control and track project history.

---

## 🔹 1. Setting Up Git

| Command | Description | Example |
|----------|--------------|---------|
| `git config --global user.name "Your Name"` | Set your username | `git config --global user.name "Pratik Shelke"` |
| `git config --global user.email "your@email.com"` | Set your email address | `git config --global user.email "pratik@example.com"` |
| `git init` | Initialize a new Git repository | `git init` |
| `git clone <url>` | Clone an existing repository | `git clone https://github.com/user/repo.git` |

---

## 🔹 2. Tracking Changes

| Command | Description | Example |
|----------|--------------|---------|
| `git status` | Show current file states (modified, staged, untracked) | `git status` |
| `git add <file>` | Stage a specific file for commit | `git add index.html` |
| `git add .` | Stage all changed files | `git add .` |
| `git commit -m "message"` | Save staged changes with a message | `git commit -m "Add homepage"` |

---

## 🔹 3. Working with Branches

| Command | Description | Example |
|----------|--------------|---------|
| `git branch` | List all branches | `git branch` |
| `git branch <name>` | Create a new branch | `git branch feature-login` |
| `git checkout <name>` | Switch to another branch | `git checkout feature-login` |
| `git checkout -b <name>` | Create and switch to a new branch | `git checkout -b bugfix` |

---

## 🔹 4. Merging & Conflicts

| Command | Description | Example |
|----------|--------------|---------|
| `git merge <branch>` | Merge another branch into the current one | `git merge feature-login` |
| `git diff` | See file differences before committing | `git diff` |
| `git log` | View commit history | `git log --oneline` |

**Example Conflict Scenario:**
> If both `main` and `feature` edit the same line, Git will show conflict markers like:
> ```
> <<<<<<< HEAD
> Your change on main
> =======
> Change from feature
> >>>>>>> feature
> ```
> You must manually edit and commit the resolved version.

---

## 🔹 5. Undoing & Resetting

| Command | Description | Example |
|----------|--------------|---------|
| `git restore <file>` | Discard unstaged changes | `git restore app.py` |
| `git reset <file>` | Unstage a file | `git reset index.html` |
| `git revert <commit>` | Undo a specific commit safely | `git revert 2b6f123` |

---

## 🔹 6. Pushing & Pulling

| Command | Description | Example |
|----------|--------------|---------|
| `git remote add origin <url>` | Link local repo to remote | `git remote add origin https://github.com/user/repo.git` |
| `git push origin main` | Push local changes to GitHub | `git push origin main` |
| `git pull origin main` | Pull latest changes from remote | `git pull origin main` |

---

## 🔹 7. Stashing Work

| Command | Description | Example |
|----------|--------------|---------|
| `git stash` | Temporarily save uncommitted changes | `git stash` |
| `git stash pop` | Reapply stashed changes | `git stash pop` |

---

## 💡 Tips
- Make **frequent commits** with meaningful messages.  
- Always pull before pushing to avoid conflicts.  
- Use branches for new features or bug fixes.  

---

**Author:** *Your Name*  
**Date:** *January 2026*  
**Purpose:** *For learning and demonstrating Git basics.*
a
