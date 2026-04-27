🧪 Experiment: Git Operations and Version Tracking
🎯 Aim

To perform Git operations including repository initialization, branching, merging, commit tracking, reverting changes, and collaboration using GitHub.

🧰 System Requirements
OS: Windows / Linux / macOS
Internet connection


🪟 Windows
Download Git from official website
Run installer → Keep default settings → Finish


🔹 Verify Installation
git --version
🔹 Configure Git (First Time Setup)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

🔐 STEP 1: Generate Personal Access Token (IMPORTANT LOGIN STEP)
Open GitHub in browser
Click Profile → Settings

Go to:

Developer Settings → Personal Access Tokens → Tokens (classic)
Click Generate New Token (classic)
🔑 Select Permissions:

✔️ Tick:

repo
workflow (optional)
Click Generate Token
⚠️ Copy the token and save it somewhere

👉 Example:

ghp_xxxxxxxxxxxxxxxxxxxxx

✔️ This token will be used instead of password


📁 STEP 2: Create Project (Flask App Example) Named git-practical

cd git-practical

🔹 Create Sample File

app.py

Paste:
print("Hello Git Practical")

🔧 STEP 3: Initialize Git Repository
git init

👉 Creates .git folder (tracks project)

➕ STEP 4: Add & Commit Files

🔹 Add Files

git add .

🔹 Commit Changes

git commit -m "Initial commit"


☁️ STEP 5: Connect to GitHub

Go to GitHub

🔹 Create New Repository (on GitHub)

Name: git-practical
Click Create Repository

🔹 Link Local Repo to GitHub

git branch -M main
git remote add origin https://github.com/<username>/git-practical.git

🔹 Push Code
git push -u origin main

🔐 When Prompt Appears:
Username:

👉 Enter your GitHub username

Password:

👉 ⚠️ Paste your Personal Access Token (NOT password)

🌿 STEP 6: Branching Operations

🔹 Create New Branch
git branch feature
🔹 Switch to Branch
git checkout feature

👉 (or modern command)

git switch feature
🔹 Make Changes
app.py
Add Line:

print("Feature added")

🔹 Commit Changes
git add .
git commit -m "Feature update"

🔀 STEP 7: Merge Branch
🔹 Switch to Main
git checkout main

🔹 Merge Feature Branch

git merge feature

📜 STEP 8: View Commit History

git log --oneline

👉 Shows:

Commit ID
Message
History

↩️ STEP 9: Revert Changes

🔹 Revert Last Commit
git revert HEAD

🔹 Revert Specific Commit
git revert <commit-id>


👥 STEP 10: Collaboration Workflow
🔹 Push Changes
git push origin main

🔹 Clone Repository (Other User)

git clone https://github.com/<username>/git-practical.git

🔹 Pull Latest Changes
git pull origin main

🔍 STEP 11: Check Repository Status
git status

🔄 Complete Workflow
Initialize repository
Add and commit files
Push to GitHub
Create branch
Modify code
Commit changes
Merge branch
View history
Revert changes

Collaborate using clone/pull
⚠️ Common Errors + Fix
Problem	Solution
Git not recognized	Restart terminal
Push rejected	Pull first (git pull)
Merge conflict	Edit file → commit again
Wrong commit	Use git revert
🧾 Result

Git operations such as repository creation, branching, merging, commit tracking, reverting changes, and collaboration were successfully performed.

🎯 Viva Questions
What is Git?
Difference between Git and GitHub
What is commit?
What is branch?
Difference between merge and rebase
What is revert?

📊 IMPORTANT GIT COMMANDS (FOR VIVA)
Command	Purpose
git init	Create repo
git add	Add files
git commit	Save changes
git push	Upload code
git pull	Download updates
git clone	Copy repo
git branch	Manage branches
git merge	Merge branches