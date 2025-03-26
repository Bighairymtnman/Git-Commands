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
   git commit -m "Initial commit of BasicCalculator"
   ```

3. Configure remote:
   ```bash
   git branch --unset-upstream
   ```
   ```bash
   git remote -v
   ```
   ```bash
   git remote set-url origin https://github.com/Bighairymtnman/BasicCalculator.git
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
   git clone https://github.com/username/repository.git
   ```

4. Enter the project directory
   ```bash
   cd repository-name
   ```


