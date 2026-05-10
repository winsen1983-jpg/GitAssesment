# Git Branching and Clone Assignment Documentation

## Objective
This assignment demonstrates how to:
- Check the Git repository status
- View and switch between branches
- Commit changes to a feature branch
- Clone a remote GitHub repository

---

## Repository Location

```powershell
D:\DevOps&MultiCloud\Assignment\Git

---

## 1. Check Git Status

```powershell
git status
```

### Output

```text
On branch Feature
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   app.py
```

### Explanation

* The current branch is `Feature`.
* The file `app.py` has been modified and staged for commit.

---

## 2. List All Branches

```powershell
git branch
```

### Output

```text
* Feature
  master
```

### Explanation

* `Feature` is the active branch.
* `master` is the main branch.

---

## 3. Switch to Master Branch

```powershell
git checkout master
```

### Output

```text
M       app.py
Switched to branch 'master'
```

### Explanation

* Git carries uncommitted changes while switching branches.

---

## 4. Attempt to Switch to Incorrect Branch Name

```powershell
git checkout featur
```

### Output

```text
error: pathspec 'featur' did not match any file(s) known to git
```

### Explanation

* The branch name was misspelled.
* The correct branch name is `Feature`.

---

## 5. Switch Back to Feature Branch

```powershell
git checkout Feature
```

### Output

```text
M       app.py
Switched to branch 'Feature'
```

---

## 6. Commit the Changes

```powershell
git commit -m "FeatureAdded"
```

### Output

```text
[Feature 625e6c2] FeatureAdded
 1 file changed, 2 insertions(+)
```

### Explanation

* The staged changes in `app.py` were committed successfully.

---

## 7. Verify Working Tree is Clean

```powershell
git status
```

### Output

```text
On branch Feature
nothing to commit, working tree clean
```

---

## 8. Switch to Master Branch

```powershell
git checkout master
```
- <img width="383" height="159" alt="image" src="https://github.com/user-attachments/assets/ed6b6ea3-62b1-465b-abf8-5cf4b1ebc9fb" />


### Output

```text
Switched to branch 'master'
```

---

# Clone Remote GitHub Repository

## Navigate to Assignment Folder

```powershell
cd D:\DevOps&MultiCloud\Assignment
```

## Verify Folder Contents

```powershell
dir
```

### Output

```text
Directory: D:\DevOps&MultiCloud\Assignment

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         5/10/2026   8:52 AM                Git
```

---

## Clone the Repository

```powershell
git clone https://github.com/winsen1983-jpg/GitAssesment.git
```

### Output

```text
Cloning into 'GitAssesment'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (6/6), done.
```

### Explanation

* The remote repository was cloned into a new folder named `GitAssesment`.

---

# Git Commands Used

| Command                   | Description                |
| ------------------------- | -------------------------- |
| `git status`              | Shows repository status    |
| `git branch`              | Lists branches             |
| `git checkout <branch>`   | Switches branches          |
| `git commit -m "message"` | Commits staged changes     |
| `git clone <url>`         | Clones a remote repository |
| `dir`                     | Lists directory contents   |

---

# Commit Information

| Branch  | Commit Message | Commit ID |
| ------- | -------------- | --------- |
| Feature | FeatureAdded   | 625e6c2   |

---

# Key Learnings

* Worked with multiple branches.
* Switched between branches.
* Handled branch name errors.
* Committed changes to a feature branch.
* Cloned a GitHub repository.

---

# Optional Next Steps

## Merge Feature into Master

```powershell
git checkout master
git merge Feature
```

## Push Changes to Remote Repository

```powershell
git push origin master
```

---

# Conclusion

This assignment successfully demonstrated the essential Git operations used in software development and DevOps workflows:

* Checking repository status
* Branch management
* Committing code changes
* Cloning remote repositories
* Preparing for merge and deployment

```
```

