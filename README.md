## 🧠 Essential Git Commands


### 🧭 1. Setup and Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list


git init                              # Initialize a new Git repository
git clone <repo-url>                  # Clone a remote repository


git status                            # Show status of files (modified, staged, untracked)
git add <file>                        # Stage a specific file
git add .                             # Stage all new and modified files
git commit -m "Your commit message"   # Commit staged changes with a message


git log                               # View commit history
git log --oneline --graph --decorate  # Compact view with branch and merge info
git show <commit-hash>                # Display details about a specific commit


git branch                            # List all branches
git branch <branch-name>              # Create a new branch
git checkout <branch-name>            # Switch to a specific branch
git switch <branch-name>              # Alternative to 'checkout'
git merge <branch-name>               # Merge a branch into the current branch
git branch -d <branch-name>           # Delete a branch


git remote -v                         # List remote connections
git remote add origin <url>           # Connect local repo to a remote repo
git fetch                             # Get latest changes from remote (no merge)
git pull origin <branch>              # Fetch and merge changes from remote
git push origin <branch>              # Push local commits to remote


git restore <file>                    # Discard changes in working directory
git reset HEAD <file>                 # Unstage a file
git revert <commit-hash>              # Create a new commit that undoes a previous one
git reset --hard <commit-hash>        # Reset entire repo to a specific commit (⚠️ destructive)


git stash                             # Temporarily save uncommitted changes
git stash list                        # Show list of stashes
git stash apply                       # Apply most recent stash (keeps it)
git stash pop                         # Apply and remove most recent stash



git diff                              # Show unstaged changes
git diff --staged                     # Show staged changes
git diff <branch1>..<branch2>         # Compare two branches


git tag <tag-name>                    # Create a lightweight tag
git tag -a <tag-name> -m "message"    # Create an annotated tag
git push origin --tags                # Push all tags to remote


