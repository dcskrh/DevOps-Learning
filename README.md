# Git Learning
This repository contains Git practice sessions.

Author: Chandrasekhar Dhanekul

## Beginner Git Commands
These are the most useful commands for a beginner working in this repository.

### 1. Check repository status
```bash
git status
```
Shows whether files are modified, untracked, or staged.

### 2. Initialize a repository
```bash
git init
```
Creates a new Git repository in the current folder.

### 3. View files in the repository
```bash
git ls-files
```
Lists tracked files.

### 4. Add files to staging area
```bash
git add <file-name>
```
Or add everything:
```bash
git add .
```

### 5. Commit changes
```bash
git commit -m "Your commit message"
```
Saves the staged changes with a message.

### 6. View commit history
```bash
git log --oneline
```
Shows recent commits in a short format.

### 7. Create a branch
```bash
git branch <branch-name>
```
Or create and switch in one command:
```bash
git checkout -b <branch-name>
```

### 8. Switch branches
```bash
git checkout <branch-name>
```
New Git versions also support:
```bash
git switch <branch-name>
```

### 9. Merge branches
```bash
git checkout main
git merge <branch-name>
```
Combines changes from another branch into the current branch.

### 10. View branches
```bash
git branch
```

### 11. See all changes
```bash
git diff
```
Shows the differences between working directory and staging area.

### 12. See staged changes
```bash
git diff --staged
```

### 13. Rename a file
```bash
git mv old-name.txt new-name.txt
```

### 14. Remove a file from tracking
```bash
git rm <file-name>
```

### 15. Undo unstaged changes
```bash
git restore <file-name>
```

### 16. Unstage a file
```bash
git restore --staged <file-name>
```

### 17. Check remote repository connection
```bash
git remote -v
```

### 18. Clone a repository
```bash
git clone <repository-url>
```

### 19. Pull latest changes
```bash
git pull origin main
```

### 20. Push changes to remote
```bash
git push origin main
```

## 10-Minute Git Practice Plan
Follow these steps in this repository to build confidence.

### Minute 1: Check repository status
```bash
git status
```
If the repo is already initialized, you will see the current state.

### Minute 2: View files and repo details
```bash
git ls-files
```
This helps you see what files are tracked.

### Minute 3: Create or edit a file
Create a simple file such as:
```bash
notepad practice.txt
```
Add a line like:
```text
Git practice session
```

### Minute 4: Stage the file
```bash
git add practice.txt
```
or
```bash
git add .
```

### Minute 5: Commit the file
```bash
git commit -m "Add Git practice file"
```

### Minute 6: Check history
```bash
git log --oneline
```
You should now see your commit.

### Minute 7: Create a new branch
```bash
git checkout -b feature/practice
```
or
```bash
git switch -c feature/practice
```

### Minute 8: Make a small change in the branch
Edit the file again and add a second line:
```text
Working on Git branch practice
```
Then stage and commit:
```bash
git add practice.txt
git commit -m "Update practice branch file"
```

### Minute 9: Merge the branch back to main
```bash
git checkout main
git merge feature/practice
```
If there are no conflicts, the merge is successful.

### Minute 10: Review final status
```bash
git status
git log --oneline --graph --all
```
This helps you confirm the branch and commit history.

## Suggested Beginner Exercise
Practice this sequence 2-3 times:
1. Create a file
2. `git add .`
3. `git commit -m "message"`
4. Create a branch
5. Edit file
6. Commit on the branch
7. Merge back to main
8. Check `git status`

## Quick Tips
- Always check `git status` before committing.
- Use clear commit messages.
- Commit small, meaningful changes.
- Do not commit generated or temporary files unless necessary.
- Keep branches short-lived for practice.

## Common Beginner Mistakes
- Forgetting to add files before commit
- Using vague commit messages like "test"
- Not checking status after every step
- Merging without reviewing the branch changes

## Practice Challenge
Try creating three files, committing each one separately, and then making a branch to update one of them. After that, merge the branch and review the log.

This will help you become comfortable with the basic Git workflow.