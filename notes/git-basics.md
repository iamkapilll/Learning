# Git Basics
# Git Fundamentals & Branching

## 1. Git vs GitHub
- Git: Distributed version control system.
- GitHub: Platform for hosting Git repositories and collaboration.

## 2. Git Architecture
Working Directory → Staging Area → Local Repository → Remote Repository

- Working Directory: Files being edited.
- Staging Area: Changes prepared for the next commit.
- Local Repository: Commit history and Git metadata.
- Remote Repository: Another repository, often hosted on GitHub.

## 3. Important Concepts
- Repository: Project tracked by Git.
- Commit: Snapshot of staged changes.
- Branch: Movable pointer to a commit.
- HEAD: Current checkout reference, normally pointing to a branch.
- Tracked: File known to Git.
- Untracked: File not yet added to Git.
- Staged: Changes selected for the next commit.

## 4. Everyday Commands
```bash
git init -b main
git clone <url>
git status
git add <file>
git add .
git diff
git diff --staged
git commit -m "message"
git log --oneline
git log --oneline --graph --all
git show HEAD
```

## 5. Branching
```bash
git branch
git branch -a
git switch -c feature/login
git switch main
git switch -
git branch -m new-name
git branch -d feature/login
```

## 6. Merging
```bash
git switch main
git merge feature/login
```

- Fast-forward: Branch pointer moves forward; no merge commit needed.
- Three-way merge: Git combines diverged histories using a common ancestor.
- Merge conflict: Git cannot automatically reconcile some changes.

## 7. HEAD References
- HEAD: Current commit.
- HEAD~1: First parent.
- HEAD~2: Two first-parent steps back.
- HEAD^: First parent.

## 8. Commit Message Examples
- feat: add login
- fix: handle missing token
- docs: update README
- refactor: simplify API handler
- test: add authentication tests
- chore: update dependencies

## 9. Key Differences
- add vs commit: Stage changes vs save a commit.
- commit vs push: Save locally vs publish remotely.
- diff vs diff --staged: Unstaged vs staged changes.
- branch vs switch: Manage branches vs change checkout.
- fast-forward vs three-way merge: Move pointer vs combine diverged history.

## 10. Common Mistakes
- Committing secrets or .env files.
- Using git add . without inspecting changes.
- Committing on the wrong branch.
- Switching branches with unfinished changes.
- Deleting .git accidentally.

## 11. Interview Questions
1. What is Git?
2. Git vs GitHub?
3. What is the staging area?
4. What happens during a commit?
5. What is HEAD?
6. What is a branch?
7. What is a fast-forward merge?
8. What is a three-way merge?
9. What is a detached HEAD?
10. What is the difference between git diff and git diff --staged?

## 12. My Practice
- Initialized a repository.
- Created multiple commits.
- Inspected changes and history.
- Created and switched branches.
- Merged a feature branch.
- Deleted a merged branch.
