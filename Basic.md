# Git Basics

---

**Author:** Shivam Bhardwaj  

**Connect with me:**  
- LinkedIn: [https://www.linkedin.com/in/cbum-bhardwaj](https://www.linkedin.com/in/cbum-bhardwaj)  
- GitHub: [https://github.com/CBUM-Bhardwaj](https://github.com/CBUM-Bhardwaj)

---

This repository is created to demonstrate basic Git and GitHub workflows. It contains sample scripts and files to help learn how to add, commit, push, and pull code effectively.

---

## Features

- Sample scripts and configuration files
- Basic Git workflow examples (add, commit, push, pull)
- Demonstrates branching and merging
- Easy to follow for beginners

---

## Getting Started

### Prerequisites
- Git installed on your local machine
- GitHub account

---

### Setup

 **Verify Git installation**
 ``` bash
git --version
```

**Intilize Git repo**
``` bash
git init
```


### Adding Files to Git

After making changes to your files or creating new ones, you need to **stage them** before committing. Staging means preparing the files so Git knows you want to include them in the next commit.

**Command:**
```bash
git add <file_name>
```
### Unstaging Files

If you accidentally staged a file and want to **remove it from the staging area** (but keep it in your local directory), use:

**Command:**
```bash
git rm --cached <file_name>
```
### Checking Repository Status

To see the current state of your Git repository, use:

**Command:**
```bash
git status
```
### Committing Changes

Once your files are staged, you can **commit them**. Committing saves a snapshot of your changes in Git.

**Command:**
```bash
git commit -m "<commit_message>"
```
### Discarding Changes

If you made changes to a file but want to **revert it back to the last committed version**, use:

**Command:**
```bash
git restore <file_name>
```
---

### Configuring Git User

Before making commits, Git needs to know **who you are**. Set your username and email using:

**Command:**
```bash
git config --global user.name "<Your Name>"
git config --global user.email "<your_email@example.com>"
```
### Viewing Commit History

To see all the commits made in your repository, use:

**Command:**
```bash
git log
```
---

### Managing Branches

Branches allow you to work on **different versions of your project** without affecting the main code.  

**View all branches:**
```bash
git branch
```
### Creating and Switching Branches in One Step

Instead of creating a branch and then switching to it separately, you can do both at once:

**Command:**
```bash
git checkout -b <branch_name>
```

### Switching Between Branches

To move between existing branches in your repository, use:

**Command:**
```bash
git checkout <branch_name>
```
```bash
git switch <branch_name>
```
### Viewing a Compact Commit History

To see a simplified, **one-line-per-commit** history, use:

**Command:**
```bash
git log --oneline
```

### Merging Branches

After working on a feature branch, you often want to **combine it with another branch** (usually `main` or `master`). This is called merging.

**Command:**
```bash
git merge <branch_name>
```
### Adding a Remote Repository

To link your local repository to a remote GitHub repository, use:

**Command:**
```bash
git remote add origin <url>
```
### Checking Remote Repositories

To see which remote repositories are linked to your local repository, use:

**Command:**
```bash
git remote -v
```

### Updating Remote URL with Personal Access Token (PAT)

If you want to use a PAT for HTTPS authentication, you can update the remote URL like this:

**Command:**
```bash
git remote set-url origin https://<USERNAME>:<PAT>@github.com/<USERNAME>/<REPO>.git
```

---

### Pushing Changes to GitHub

After committing your changes locally, you can **push them to the remote repository** on GitHub.

**Command:**
```bash
git push origin <branch_name>
```

### Pulling Changes from GitHub

To update your local repository with the latest changes from the remote repository, use:

**Command:**
```bash
git pull origin <branch_name>
```
