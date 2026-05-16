Question 1: Project Initialization & First Push

Step 1: Create Project Folder
mkdir Assignment-2
cd Assignment-2

Step 2: Initialize Git Repository
git init

Step 3: Create Python File
touch app.py

Added sample Python code inside app.py:

print('This is main program')
print('CODE 01 added')
print('CODE 02 added')
print('CODE 03 added')

Step 4: Check Git Status: git status

Step 5: Stage the File: git add .

Step 6: Commit the Changes: git commit -m "First Commit to add Main Program"

Step 7: Create Remote Repository

Created a new GitHub repository: My_Assignment-2_repo

Step 8: Add Remote Repository:
git remote add origin https://github.com/Zeeshan6362/My_Assignment-2_repo.git

Step 9: Verify Remote Configuration: git remote -v

Step 10: Push Code to GitHub: git push -u --force origin main

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question 2: Working with Changes & History

Step 1: Modify app.py

Added new features:

print('Feature 01 added')
print('Feature 02 added')

Step 2: Check Current Changes: git status

Step 3: View Differences: git diff

Step 4: Stage Specific Changes: git add -p --> Selected: y

Step 5: Commit Changes: git commit -m "New features 1 and 2 added to main program"

Step 6: Make Another Change

Added 'program ending code' in app.py

Step 7: Stage All Changes: git add .

Step 8: Commit Again: git commit -m "Program ending code added"

Step 9: View Full Commit History: git log

Step 10: View Compact One-Line History: git log --oneline

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question 3: Branching & Feature Development

Step 1: Create New Branch: git checkout -b feature-update

Step 2: Verify Current Branch: git branch

Step 3: Modify app.py
Added 'Feature 03 code' in the new branch.

Step 4: Stage Changes: git add .

Step 5: Commit Changes: git commit -m "Added feature 03 for new branch"

Step 6: Switch Back to Main Branch: git checkout main

Step 7: Merge Feature Branch: git merge feature-update

Step 8: Verify Merge History: git log --oneline

Step 9: Delete Branch Safely: git branch -d feature-update

Step 10: Create Dummy Branch: git checkout -b dummy-branch

Step 11: Switch Back to Main: git checkout main

Step 12: Force Delete Dummy Branch: git branch -D dummy-branch

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Question 4: Handling Errors (Stash, Reset, Revert)

Step 1: Make Changes Without Commit
#Modified app.py but did not commit.

Step 2: Stash Changes: git stash

Step 3: View Stash List: git stash list

Step 4: Apply Stashed Changes: git stash pop

Step 5: Stage Changes: git add .

Step 6: Commit Stashed Work: git commit -m "Completed working on new feature for Question 02"

Step 7: Add Incorrect Code

Modified app.py with intentionally broken code.

Step 8: Commit Incorrect Code: 
git add .
git commit -m "intentionally adding broken code"

Step 9: Undo Last Commit Using Reset: git reset --hard HEAD~1

Step 10: Add Safe Changes:

Modified app.py with safe feature updates.

Step 11: Commit Safe Changes: 
git add .
git commit -m "safe feature added for question 04"

Step 12: Undo Commit Using Revert: git revert HEAD

Step 13: Verify Commit History: git log --oneline

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Commands Summary
Git Initialization: git init
Check Status: git status
Stage Files: git add .
Commit Changes: git commit -m "message"
View History: git log // git log --oneline

Branch Operations
git checkout -b branch-name
git checkout main
git merge branch-name
git branch -d branch-name
git branch -D branch-name

Stash Operations
git stash
git stash list
git stash pop

Undo Changes
git reset --hard HEAD~1
git revert HEAD
