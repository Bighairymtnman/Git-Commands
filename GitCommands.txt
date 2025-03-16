1. Basic Commands

git init — Initialize a new Git repository.
git clone <repository-url> — Clone an existing repository.
git status — Show the status of files (untracked, modified, etc.).
git add <file> — Add a specific file to staging.
git add . — Add all files in the current directory to staging.
git commit -m "message" — Commit changes with a message.
git push — Push commits to the remote repository.
git pull — Pull updates from the remote repository.

2. Branching & Merging

git branch — List all branches.
git branch <branch-name> — Create a new branch.
git checkout <branch-name> — Switch to another branch.
git checkout -b <branch-name> — Create and switch to a new branch.
git merge <branch-name> — Merge a branch into the current branch.

3. File Management

git mv <old-filename> <new-filename> — Rename a file.
git rm <file> — Remove a file from the staging area (and repository).
git reset <file> — Unstage a file.
git log — View the commit history.

4. Advanced Operations

git reset --hard — Reset the repository to the last commit (be careful, as this deletes uncommitted changes).
git rebase <branch> — Rebase your current branch onto another.
git stash — Temporarily save changes that aren't ready to be committed.
git stash pop — Retrieve changes that were stashed.
git remote add origin <url> — Set the remote repository.

5. Tagging

git tag <tag-name> — Create a tag.
git tag -a <tag-name> -m "message" — Create an annotated tag.