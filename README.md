<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Complete Git Commands Cheat Sheet</title>
</head>
<body>
    <h1>Complete Git Commands Reference</h1>

    <!-- CONFIGURATION -->
    <b>Set your global username for commits:</b><br>
    git config --global user.name "Firstname Lastname"<br>
    <i>Set a name that is identifiable for credit when reviewing version history.</i><br><br>

    <b>Set your global email for commits:</b><br>
    git config --global user.email "valid-email@example.com"<br>
    <i>Set an email address associated with each commit in the history.</i><br><br>

    <b>Enable automatic color output for Git commands:</b><br>
    git config --global color.ui auto<br><br>

    <b>Verify current Git configuration:</b><br>
    git config --list<br><br>

    <!-- INITIAL SETUP -->
    <b>Create a new local repository:</b><br>
    mkdir directory_name<br>
    cd directory_name<br>
    git init<br><br>

    <b>Connect to a remote repository:</b><br>
    git remote add origin &lt;repository-url&gt;<br>
    git remote -v   <i>(Verify remote)</i><br><br>

    <b>Rename current branch to main:</b><br>
    git branch -M main<br><br>

    <!-- CLONE -->
    <b>Clone an existing remote repository locally:</b><br>
    git clone &lt;repository-url&gt;<br><br>

    <!-- STATUS -->
    <b>Show current status of working directory and staging area:</b><br>
    git status<br><br>

    <!-- ADD & COMMIT -->
    <b>Stage a specific file:</b><br>
    git add [file]<br><br>

    <b>Stage all changes:</b><br>
    git add .<br><br>

    <b>Unstage a staged file (keep changes):</b><br>
    git reset [file]<br><br>

    <b>Commit staged changes with a message:</b><br>
    git commit -m "Your descriptive commit message"<br><br>

    <b>Stage & commit tracked file changes in one step (skip for new files):</b><br>
    git commit -am "Your message"<br><br>

    <!-- DIFF -->
    <b>Show unstaged changes:</b><br>
    git diff<br><br>

    <b>Show staged changes:</b><br>
    git diff --staged<br><br>

    <!-- PULL -->
    <b>Pull latest changes from remote main branch:</b><br>
    git pull origin main<br><br>

    <b>Pull and allow unrelated histories:</b><br>
    git pull origin main --allow-unrelated-histories<br><br>

    <!-- PUSH -->
    <b>Push local commits to remote main branch:</b><br>
    git push origin main<br><br>

    <!-- BRANCHES -->
    <b>List all branches (* shows active branch):</b><br>
    git branch<br><br>

    <b>Create a new branch:</b><br>
    git branch [branch-name]<br><br>

    <b>Switch to another branch:</b><br>
    git checkout [branch-name]<br><br>

    <!-- MERGE -->
    <b>Merge another branch into current branch:</b><br>
    git merge [branch-name]<br><br>

    <!-- LOG -->
    <b>Show commit history:</b><br>
    git log<br><br>
</body>
</html>

