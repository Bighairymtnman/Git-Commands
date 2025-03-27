# Git Commands Reference



## Adding a New Repository to GitHub

1. Navigate to project folder:
   ```bash
   cd /path/to/your/project
   ```

2. Initialize Git repository:
   ```bash
   git init
   ```

3. Add remote repository:
   ```bash
   git remote add origin https://github.com/YourUsername/your-repository.git
   ```

4. Add files to staging:
   ```bash
   git add .
   ```

5. Commit changes:
   ```bash
   git commit -m "Initial commit message"
   ```

6. Push to GitHub:
   ```bash
   git push -u origin master  # Or 'main' if your GitHub repo uses main branch
   ```




## Force Local Files to Replace Repository Files

1. Navigate to project:
   ```bash
   cd C:\Users\amnic\OneDrive\Desktop\Coding\Git\ProjectName
   ```

2. Initialize and stage:
   ```bash
   git init
   ```
   ```bash
   git add .
   ```
   ```bash
   git commit -m "Initial commit of ProjectName"
   ```

3. Configure remote:
   ```bash
   git branch --unset-upstream
   ```
   ```bash
   git remote -v
   ```
   ```bash
   git remote set-url origin https://github.com/YourUsername/your-repository.git
   ```

4. Push and update branches:
   ```bash
   git push -u origin master
   ```
   ```bash
   git branch -m master main
   ```
   ```bash
   git fetch origin
   ```
   ```bash
   git push -f origin main
   ```
   ```bash
   git push origin --delete master
   ```





## Cloning GitHub Repository

1. Get the HTTPS URL from GitHub repository
   - Go to repository on GitHub.com
   - Click green "Code" button
   - Copy the HTTPS URL

2. Navigate to desired directory
   ```bash
   cd your/desired/directory
   ```

3. Clone the repository
   ```bash
   git clone https://github.com/YourUsername/your-repository.git
   ```

4. Enter the project directory
   ```bash
   cd your-repository
   ```





## Cleaning Repository History

1. Navigate to repository:
   ```bash
   cd /path/to/your/project
   ```

2. Create backup branch:
   ```bash
   git checkout -b backup-main
   ```

3. Return to primary branch:
   ```bash
   git checkout master  # or 'main' depending on your branch name
   ```

4. Clean repository history:
   ```bash
   git filter-branch --force --index-filter "git rm --cached --ignore-unmatch PATH-TO-FILE" --prune-empty --tag-name-filter cat -- --all
   ```

5. Force push changes:
   ```bash
   git push origin --force --all
   ```

This process rewrites repository history to remove sensitive information from previous commits while preserving current code.




## Resolving Main/Master Branch Conflicts

1. Rename local branch to main:
   ```bash
   git branch -M main
   ```

2. Pull remote changes with unrelated histories:
   ```bash
   git pull origin main --allow-unrelated-histories
   ```

3. Push changes to main branch:
   ```bash
   git push -u origin main
   ```

This process synchronizes repositories when working across multiple machines and resolves branch naming conflicts.




## Removing Files from Repository

1. Remove file and stage deletion:
   ```bash
   git rm filename
   ```

2. Commit the removal:
   ```bash
   git commit -m "Remove file"
   ```

3. Push changes to remote:
   ```bash
   git push origin main  # or master depending on branch name
   ```





## Managing File Contents

1. Create backup of original files (optional):
   ```bash
   cp file1.md file1_backup.md
   cp file2.md file2_backup.md
   ```

2. Edit files with new content

3. Stage and commit changes:
   ```bash
   git add .
   git commit -m "Reorganized file contents"
   ```

4. Push to remote:
   ```bash
   git push origin master
   ```





[Previous content remains exactly the same until the end...]

## Managing File Contents

1. Create backup of original files (optional):
   ```bash
   cp file1.md file1_backup.md
   cp file2.md file2_backup.md
   ```

2. Edit files with new content

3. Stage and commit changes:
   ```bash
   git add .
   git commit -m "Reorganized file contents"
   ```

4. Push to remote:
   ```bash
   git push origin master
   ```

## Pulling Changes from Repository

1. Check remote repository status:
   ```bash
   git remote -v
   ```

2. Fetch latest changes:
   ```bash
   git fetch origin
   ```

3. Pull changes from remote:
   ```bash
   git pull origin main
   ```

4. Pull with specific options:
   ```bash
   git pull --rebase origin main
   ```
