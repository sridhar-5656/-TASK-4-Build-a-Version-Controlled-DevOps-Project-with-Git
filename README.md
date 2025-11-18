# DevOps Git Practice Project – Task 4 🚀

## 📌 Objective

This project is part of **Task 4: Build a Version-Controlled DevOps Project with Git**.
The goal is to practice Git branching, pull requests (PRs), merging, tagging, and documentation in a real-world workflow.

---

## 🏗️ Step-by-Step Practice Plan

### 🔹 1. Create a Local Project

```bash
mkdir devops-task4
cd devops-task4
echo "# DevOps Git Practice Project" > README.md
git init
git add .
git commit -m "Initial commit"
```

### 🔹 2. Create a Remote GitHub Repo

1. Go to GitHub → **New repository** → name it `devops-task4`.
2. Copy the repo HTTPS link and run:

```bash
git remote add origin https://github.com/your-username/devops-task4.git
git branch -M main
git push -u origin main
```

### 🔹 3. Create Branches

```bash
git checkout -b dev
git push -u origin dev

git checkout -b feature-hello
```

### 🔹 4. Work on Feature Branch

Example script and workflow:

```bash
echo "print('Hello DevOps')" > hello.py
git add hello.py
git commit -m "Added hello.py script"
git push -u origin feature-hello
```

* Then open a PR on GitHub: **feature-hello → dev** and merge it once reviewed.

### 🔹 5. Merge Dev into Main

* Open a PR from **dev → main** on GitHub and merge after checks.

### 🔹 6. Add .gitignore

```bash
echo "*.log" > .gitignore
git add .gitignore
git commit -m "Add .gitignore to exclude log files"
git push origin dev
```

> Tip: If you get a push rejection, run `git pull origin dev --rebase` first, resolve conflicts if any, then push.

### 🔹 7. Tag a Version

```bash
git tag v1.0
git push origin v1.0
```

### 🔹 8. Document the Project

Create a `TASK4_NOTES.md` file to keep your notes and learning summary.

```markdown
# Task 4 - Git Practice

## Steps I followed
1. Initialized repo
2. Created branches (main, dev, feature)
3. Added hello.py script
4. Used Pull Requests to merge
5. Added .gitignore
6. Created tags

## What I Learned
- Git branching
- Pull requests
- Conflict resolution
- Git tags and .gitignore
```

Commit and push `TASK4_NOTES.md` to the repo. ✅

---

## 📂 Final Repository Structure

```
devops-task4/
│── README.md
│── TASK4_NOTES.md
│── hello.py
│── .gitignore
```

* **Branches:** `main`, `dev`, `feature-*`
* **Pull Requests:** history of merges and code reviews
* **Commits:** meaningful commit messages
* **Tags:** version tags like `v1.0`

---

## 🎯 What You’ll Learn

* Initializing and managing a Git project
* Creating and switching between branches
* Writing commits and pushing to remote
* Pull Request (PR) workflow for collaboration
* Using `.gitignore` effectively
* Tagging versions for release management

---

If you want, I can also generate the other files (`TASK4_NOTES.md`, `hello.py`, `.gitignore`) and provide a ZIP of the project. Want me to add those now?



📖 What I Learned

Difference between merge and rebase

How to resolve merge conflicts

How to use git stash for saving temporary changes

Importance of .gitignore

How to mark releases with git tags

How real-world teams use branching and pull requests

❓ Interview Questions Prepared

What is Git?

What is the difference between merge and rebase?

What is a pull request?

How do you resolve merge conflicts?

What are Git tags?

What is Git workflow?

Explain git stash.

What is the use of .gitignore?

🏁 Conclusion

This project helped me practice Git workflows in a real DevOps style.
Now I understand how version control is used in professional projects and how teams collaborate using Git and GitHub.
