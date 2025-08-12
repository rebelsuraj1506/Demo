# Complete Git Commands Reference

### Configuration

**Set your global username for commits:**  
`git config --global user.name "Firstname Lastname"`  
_Set a name that is identifiable for credit when reviewing version history._

**Set your global email for commits:**  
`git config --global user.email "valid-email@example.com"`  
_Set an email address associated with each commit in the history._

**Enable automatic color output for Git commands:**  
`git config --global color.ui auto`  

**Verify current Git configuration:**  
`git config --list`  

---

### Initial Setup

**Create a new local repository:**
`mkdir directory_name`<br>
`cd directory_name`<br>
`git init`


**Connect to a remote repository:**  
`git remote add origin <repository-url>`  
_Verify remote:_ `git remote -v`

**Rename current branch to main:**  
`git branch -M main`  

---

### Clone

**Clone an existing remote repository locally:**  
`git clone <repository-url>`  

---

### Status

**Show current status of working directory and staging area:**  
`git status`  

---

### Add & Commit

**Stage a specific file:**  
`git add [file]`  

**Stage all changes:**  
`git add .`  

**Unstage a staged file (keep changes):**  
`git reset [file]`  

**Commit staged changes with a message:**  
`git commit -m "Your descriptive commit message"`  

**Stage & commit tracked file changes in one step (skip for new files):**  
`git commit -am "Your message"`  

---

### Diff

**Show unstaged changes:**  
`git diff`  

**Show staged changes:**  
`git diff --staged`  

---

### Pull

**Pull latest changes from remote main branch:**  
`git pull origin main`  

**Pull and allow unrelated histories:**  
`git pull origin main --allow-unrelated-histories`  

---

### Push

**Push local commits to remote main branch:**  
`git push origin main`  

---

### Branches

**List all branches (* shows active branch):**  
`git branch`  

**Create a new branch:**  
`git branch [branch-name]`  

**Switch to another branch:**  
`git checkout [branch-name]`  

---

### Merge

**Merge another branch into current branch:**  
`git merge [branch-name]`  

---

### Log

**Show commit history:**  
`git log`  

---

## Show Commit History
- `git log`  
  Show commit history for the currently active branch.

- `git log branchB..branchA`  
  Show the commits that are in branchA but not in branchB.

- `git log --follow [file]`  
  Show the commits that changed a specific file, even if the file was renamed.

## Remote Repositories
- `git remote add [alias] [url]`  
  Add a Git URL as an alias for a remote repository.

- `git fetch [alias]`  
  Fetch down all the branches from that Git remote without merging.

## Merging & Pulling
- `git merge [alias]/[branch]`  
  Merge a remote branch into your current branch to bring it up to date.

- `git pull`  
  Fetch and merge any commits from the tracking remote branch.

## Differences & Showing Commits
- `git diff branchB...branchA`  
  Show the diff of what is in branchA that is not in branchB.

- `git show [SHA]`  
  Show any Git object (commit, tag, tree) in human-readable format.

## Pushing Changes
- `git push [alias] [branch]`  
  Transmit local branch commits to the remote repository branch.
