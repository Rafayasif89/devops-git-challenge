# PROOF OF WORK

## 1. Git Commit History

The following output is from `git log --oneline`:

98b2c92 Merge pull request #1 from Rafayasif89/development
f435c56 fix: resolved merge conflict
093701e fix: staging label
2f92392 feat: updated script with staging env
cd87a07 feat: initial commit with deploy script
```

## 2. Reflection Questions

### Q1. What is the difference between Git and GitHub?

Git is a distributed version control system that tracks changes in project files and records commit history. It allows developers to create branches, compare changes, and merge different versions of a project. GitHub is an online platform that hosts Git repositories and supports collaboration through pull requests, code reviews, and issue tracking. Git can work locally without GitHub, while GitHub makes sharing and collaboration easier.

### Q2. Explain the Working Directory, Staging Area, and Local Repository.

The Working Directory is where I create and edit project files. The Staging Area contains the changes selected for inclusion in the next commit using commands such as `git add`. The Local Repository stores committed snapshots and the project's version history. The typical workflow is to modify files, stage the desired changes, and commit them to the local repository.

### Q3. What is the difference between `git stash pop` and `git stash apply`?

Both commands restore previously stashed changes to the working directory. `git stash pop` restores the changes and normally removes the stash entry after successful application. `git stash apply` restores the changes but keeps the stash entry in the stash list. Therefore, `git stash apply` is useful when I want to preserve or reuse a stash, whereas `git stash pop` is useful when I want to restore and remove it.

### Q4. What is the difference between `git fetch` and `git pull`?

`git fetch` downloads updates from a remote repository without integrating them into the current local branch. `git pull` fetches those updates and then integrates them into the current branch, usually through merging or, depending on configuration, rebasing. Fetching allows me to inspect remote changes before integrating them. Pulling is convenient when I want to update my local branch with remote changes.
