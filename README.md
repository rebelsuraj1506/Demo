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

