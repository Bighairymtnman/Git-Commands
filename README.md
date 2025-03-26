Commands to add a new repository on GitHub:

1. Navigate to your project folder:
   cd /path/to/your/project

2. Initialize a Git repository:
   git init

3. Add a remote repository (replace the URL with your GitHub repository URL):
   git remote add origin https://github.com/YourUsername/your-repository.git

4. Add your files to the staging area:
   git add .

5. Commit the changes:
   git commit -m "Initial commit message"

6. Push the changes to GitHub (if this is the first push, use master or main):
   git push -u origin master  # Or 'main' if your GitHub repo uses the main branch




Commands to force local files to replace the repo files:
cd C:\Users\amnic\OneDrive\Desktop\Coding\Git\ProjectName
git init
git add .
git commit -m "Initial commit of BasicCalculator"
git branch --unset-upstream
git remote -v
git remote set-url origin https://github.com/Bighairymtnman/BasicCalculator.git
git push -u origin master
git branch -m master main
git fetch origin
git push -f origin main
git push origin --delete master
