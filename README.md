# even-odd
git init 
git add .
git commit -m "Initial commit"
git checkout -b develop (create branch name develop)
git checkout -b feature/add-user-greeting
git checkout develop git merge feature/add-user-greeting
git checkout -b release/v1.0
git checkout main
git merge release/v1.0
git tag v1.0a

✅ EXPERIMENT 1 – USING VS CODE + GIT + GITHUB


---

🟢 STEP 1: Open Project in VS Code

1. Create a new folder on Desktop → SimpleApp


2. Open VS Code


3. Click File → Open Folder


4. Select SimpleApp




---

🟢 STEP 2: Create Simple Application

1. Click New File


2. Name it: app.py


3. Paste this code:



print("Welcome to My Simple Application!")

name = input("Enter your name: ")
print("Hello", name, "!")

4. Save the file (Ctrl + S)


5. Run it using:



Right click → Run Python File
OR

Open Terminal in VS Code →


python app.py


---

🟢 STEP 3: Initialize Git in VS Code

1. Open Terminal in VS Code
👉 Terminal → New Terminal


2. Type:



git init

3. Add files:



git add .

4. Commit with proper message:



git commit -m "Initial commit: Added simple console application"

✅ Local Git repository created successfully.


---

🟢 STEP 4: Create Remote Repository on GitHub

1. Go to GitHub


2. Click New Repository


3. Name it: SimpleApp


4. Do NOT select README


5. Click Create Repository




---

🟢 STEP 5: Connect Local Repo to GitHub

Copy the repository URL.

In VS Code terminal:

git remote add origin https://github.com/yourusername/SimpleApp.git
git branch -M main
git push -u origin main

Enter GitHub username & password (or token if asked).

✅ Now your project is live on GitHub.
Open browser → Check repository → Code is visible ✔


---

🟢 STEP 6: Create Feature Branch

In VS Code terminal:

git checkout -b feature-greeting

✅ New branch created.


---

🟢 STEP 7: Modify Application (Minor Enhancement)

Edit app.py:

print("Welcome to My Simple Application!")

name = input("Enter your name: ")
age = input("Enter your age: ")

print("Hello", name, "!")
print("You are", age, "years old.")

Save file.


---

🟢 STEP 8: Commit Changes in Feature Branch

git add .
git commit -m "Added age input feature"


---

🟢 STEP 9: Merge Feature Branch to Main

Switch to main:

git checkout main

Merge:

git merge feature-greeting

If no conflicts → It merges automatically ✅

If conflict occurs:

Open file

Fix conflict

Save

Then:


git add .
git commit -m "Resolved merge conflict"
git config --global user.name " "
git config --global user.email " "
A) Setup & Configuration

git --version

Checks the installed Git version.

git config --global user.name "Your Name"

Sets your Git username globally.

git config --global user.email you@example.com

Sets your Git email globally.


---

B) Create or Clone Repositories

git init

Initializes a new Git repository in the current directory.

git clone <repository-url>

Creates a copy of an existing remote repository.


---

C) Check Status

git status

Displays the state of working directory and staging area.


---

D) Add Files (Staging Area)

git add file.txt

Adds a specific file to the staging area.

git add .

Adds all files to the staging area.


---

E) Commit Changes

git commit -m "Message"

Commits staged changes with a message.

git commit --amend

Modifies the last commit.


---

F) View History

git log

Shows commit history.

git log --oneline

Shows compact commit history.

git log --oneline --graph --all

Shows graphical representation of all branches.


---

G) Branching

git branch

Lists all branches.

git branch <name>

Creates a new branch.

git checkout <name>

Switches branch.

git checkout -b <name>

Creates and switches to a new branch.


---

H) Merging

git merge <branch>

Merges the specified branch into current branch.


---

I) Remote Repository Commands

git remote add origin <url>

Adds a remote repository.

git remote -v

Displays remote repository URLs.

git push origin main

Pushes local commits to remote main branch.

git push -u origin main

Pushes and sets upstream branch.

git pull origin main

Fetches and merges changes from remote main branch.

git fetch

Downloads changes from remote without merging.


---

J) Undo / Reset / Restore

git restore file.txt

Restores file to last committed state.

git restore --staged file.txt

Removes file from staging area.

git reset --soft HEAD~1

Undo last commit, keep changes staged.

git reset --mixed HEAD~1

Undo last commit, unstage changes.

git reset --hard HEAD~1

Undo last commit and delete changes.

git revert <commit-id>

Creates a new commit that undoes specified commit.


---

K) Stash (Temporary Save)

git stash

Temporarily saves uncommitted changes.

git stash list

Lists all stashed changes.

git stash apply

Applies latest stash without deleting it.

git stash pop

Applies and removes latest stash.


---

L) Tagging

git tag v1.0

Creates a tag.

git push origin v1.0

Pushes tag to remote repository



---

🟢 STEP 10: Push Updated Main to GitHub

git push origin main
