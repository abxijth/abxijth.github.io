---
title: "Task 01 — Git Exercises"
date: 2025-11-08
description: "A concise summary of all Git exercises I solved, with key commands and takeaways."
tags: ["amfoss-anveshan", "git", "version-control"]
draft: false
---

# 🧩 Git Exercises — Summary

> Website: [gitexercises.fracz.com](https://gitexercises.fracz.com)

A practical task to learn **Git inside out** — commits, branching, rebasing, and recovery.  
Here’s a short walkthrough of what I did and what I learned.

---

## ⚙️Setup
```bash
git clone https://gitexercises.fracz.com/git/exercises.git
cd exercises
git config user.name "Your name here"
git config user.email "Your e-mail here"
./configure.sh
git start
```
---

## master  

> - **description**
>
> The first exercise was to push the commit created after running the git start command. After initializing the repository, I ran git verify and successfully passed the very first challenge.
>
> - **commands used**
> ```bash
> git start
> git verify
> ```
> - **completion screenshot**
> ![master.png](/images/master.png)

---

## commit-one-file

> - **description**
>
> In this exercise, two files — A.txt and B.txt — were created in the project’s root directory. The goal was to stage and commit only one of them while leaving the other untracked.
> Instead of pushing to a remote repository, the solution was verified locally using the git verify command.
>
> - **commands used**
> ```bash
> git add A.txt
> git commit -m "Commit A.txt file"
> ```
> - **completion screenshot**
> ![commit-one-file.png](/images/commit-one-file.png)

---

## commit-one-file-staged

> - **description**
> 
> In this exercise, two files — A.txt and B.txt — were created in the project’s root directory and both were initially added to the staging area.
> The challenge was to commit only one file while keeping the other staged but uncommitted.
> The solution was then verified locally using the git verify command.
>
> - **commands used**
> ```bash
> git reset A.txt
> git commit -m "Commit B.txt file"
> ```
> - **completion screenshot**
> ![commit-one-file-staged.png](/images/commit-one-file-staged.png)

---

## ignore them

> - **description**
>
> In this exercise, the goal was to configure Git to ignore unnecessary or generated files. This involved creating and committing a .gitignore file that excluded:
>
> - All files with the .exe extension
>
> - All files with the .o extension
>
> - All files with the .jar extension
>
> - The entire libraries/ directory
>
> These patterns ensured that build artifacts and external dependencies were not tracked in version control.
> Sample files were already provided to test the configuration, and the setup was verified using the git verify command.
>
> - **commands used**
> ```bash
> echo *.o > .gitignore
> echo *.exe >> .gitignore
> echo *.jar >> .gitignore
> echo libraries/ >> .gitignore
> git add .gitignore
> git commit -m "Ignore binary files"
> ```
> - **completion screenshot**
> ![ignore-them.png](/images/ignore-them.png)












