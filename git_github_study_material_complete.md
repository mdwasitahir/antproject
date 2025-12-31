
# 📘 Git & GitHub Study Material (Beginner to Intermediate)

## 📁 Step 1: Project Initialization
```bash
mkdir git-demo-project
cd git-demo-project
git init
```
**Explanation:** Initializes a new Git repository to begin version control.

## ⚙️ Step 2: Git Configuration
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
**Explanation:** Sets global username and email for all repositories.

```bash
git config user.name "Project Name"
git config user.email "project.email@example.com"
```
**Explanation:** Sets username/email only for the current repository.

## 📄 Step 3: File Creation and Staging
```bash
echo "Hello Git!" > readme.txt
git status
```
**Explanation:** Creates a new file and checks status.

```bash
git add readme.txt
git add .
```
**Explanation:** Stages specific or all files for the next commit.

## ✅ Step 4: Commit Changes
```bash
git commit -m "Initial commit"
```
**Explanation:** Commits staged changes with a message.

## 🌐 Step 5: Connect to GitHub
```bash
git remote add origin https://github.com/yourusername/git-demo-project.git
git remote -v
```
**Explanation:** Links to GitHub repository and verifies remote URLs.

## 🚀 Step 6: Push to GitHub
```bash
git push -u origin main
```
**Explanation:** Pushes the local branch to GitHub and sets upstream.

## 🏷 Step 7: Default Branch Name
```bash
git branch -m master main
git push -u origin main
git push origin --delete master
```
**Explanation:** Renames branch locally and updates on GitHub.

## 🌿 Step 8: Branching
```bash
git branch feature-1
git checkout feature-1
git switch feature-1
git checkout -b bugfix-123
git switch -c bugfix-123
```
**Explanation:** Creates and switches between branches.

## 🔁 Step 9: Merging
```bash
git checkout main
git merge feature-1
```
**Explanation:** Merges changes from another branch.

## ⚔️ Step 10: Merge Conflict
```bash
# After resolving
git add conflicted_file.txt
git commit -m "Resolve merge conflict"
```
**Explanation:** Resolves conflicts and commits.

## 🔄 Step 11: Rebase
```bash
git checkout feature-1
git rebase main
```
**Explanation:** Reapplies commits onto updated branch base.

## 🧺 Step 12: Git Stash
```bash
git stash
git stash list
git stash apply
git stash pop
```
**Explanation:** Temporarily saves and retrieves uncommitted changes.

## 🧹 Step 13: Git Reset
```bash
git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1
```
**Explanation:** Reverts to previous state with different levels of change discard.

## 🍒 Step 14: Cherry Pick
```bash
git cherry-pick <commit-hash>
```
**Explanation:** Applies a specific commit to the current branch.

## 🔁 Step 15: Pull vs Fetch
```bash
git pull origin main
git fetch origin
git merge origin/main
```
**Explanation:** Pull = fetch + merge. Fetch downloads without merging.

## 🏷 Step 16: Remote Labels
```bash
git remote add origin <url>
git remote rename origin upstream
```
**Explanation:** Manage remote repositories using labels.

## ❌ Step 17: Delete Branches
```bash
git branch -d feature-1
git branch -D feature-1
git push origin --delete feature-1
```
**Explanation:** Deletes local and remote branches.

## 📋 Summary Table

| Task             | Command                              | Explanation                        |
|------------------|---------------------------------------|------------------------------------|
| Init repo        | `git init`                            | Start Git in folder                |
| Config           | `git config`                          | Set username/email                 |
| Stage            | `git add`                             | Track changes                      |
| Commit           | `git commit`                          | Save changes                       |
| Remote add       | `git remote add`                      | Link GitHub repo                   |
| Push             | `git push`                            | Upload to GitHub                   |
| Branch           | `git branch`                          | Create/view branches               |
| Switch           | `git checkout` / `switch`             | Change branch                      |
| Merge            | `git merge`                           | Combine branches                   |
| Conflict         | Manual + `git add`                    | Resolve merge issues               |
| Rebase           | `git rebase`                          | Linear history                     |
| Stash            | `git stash`                           | Save uncommitted work             |
| Reset            | `git reset`                           | Undo commits                       |
| Cherry-pick      | `git cherry-pick`                     | Copy a commit                      |
| Pull             | `git pull`                            | Fetch + merge                      |
| Fetch            | `git fetch`                           | Only fetch updates                 |
| Delete branch    | `git branch -d/-D`                    | Remove branches                    |
