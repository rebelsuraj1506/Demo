# Demo
Understanding git commands
<br>

git config --global user.name “[firstname lastname]”<br>
set a name that is identifiable for credit when review version history<br>

git config --global user.email “[valid-email]”<br>
set an email address that will be associated with each history marker<br>

git clone [url]<br>
retrieve an entire repository from a hosted location via URL<br>

<p><strong>Show modified files in the working directory, staged files, and untracked files.</p>
git status<br>

Remove a file from the staging area but keep its changes in the working directory.<br>
git reset [file]<br>

Show the line-by-line differences for changes that haven’t been staged.<br>
git diff<br>

Show the differences between the staged files and the last commit.<br>
git diff --staged<br>

Fetch and merge changes from the remote `main` branch into your local branch, even if they have different histories.<br>
git pull origin main --allow-unrelated-histories<br>

If you want to add and commit a specific file:<br>
git add README.md
git commit -m "Add README.md with project description"

If you want to add and commit all changes at once:
git add .
git commit -m "Your descriptive commit message here"


Create a local repository on your own machine<br>
mkdir directory_name<br>
cd directory_name<br>
init :- Used to create a new git repo<br>
git init<br>
git remote add origin <link to new repo><br>
git remote -v(To verify remote)<br>
git branch(To check branch)<br>
git branch -M main(to rename branch)<br>
Upload your local commits to the remote repository’s `main` branch.<br>
git push origin main
