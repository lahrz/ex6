# ex6
Step 1: Create a repository on GitHub
1. Open https://github.com
2. Log in to GitHub.
3. Click the + icon → New repository.
4. Enter the repository name as Exp6.
5. Select Public.
6. Enable Add README.
7. Click Create repository.
Step 2: Clone the existing GitHub repository
Copy the HTTPS link from GitHub (Code → HTTPS).
git clone https://github.com/Precilla-mary/Exp6.git


Enter the cloned repository:
cd Exp6


Check the files:
ls


Expected file:
README.md


Step 3: Verify remote configuration
git remote -v


Expected output:
origin  https://github.com/Precilla-mary/Exp6.git (fetch)
origin  https://github.com/Precilla-mary/Exp6.git (push)


Step 4: Check Python version and repository contents
py --version
ls -la


Step 5: Create a Python file
Open the file using Vim:
vi sample.py


Press i to enter insert mode and type:
print("Welcome to Git Experiment 6")print("Working with a cloned repository")



To save and exit Vim:
1. Press Esc.
2. Type :wq
3. Press Enter.
Run the Python file:
py sample.py


Expected output:
Welcome to Git Experiment 6
Working with a cloned repository


Step 6: Check the status and commit the changes
git status


Add the Python file:
git add sample.py


Commit the changes:
git commit -m "Add Python source file"


Step 7: Verify the commit
git log --oneline


Check the files:
ls -la


Display the README file:
cat README.md


Display the Python file:
cat sample.py


Step 8: Create a feature branch
git checkout -b feature


Verify the branches:
git branch


Check the repository contents:
ls -la


Display the README:
cat README.md


Step 9: Switch back to the main branch
git checkout main


Check the repository status:
git status


Step 10: Pull the latest changes from the remote repository
git pull origin main


This command fetches and integrates the latest changes from the remote main branch into your local main branch.
Step 11: Verify the updated README
cat README.md


Expected updated content (as shown in the experiment):
Exp6
Latest changes added by another developer to remote repo.


Step 12: Switch to the feature branch and verify
git checkout feature


Display the README:
cat README.md
