# Git Commands Cheat Sheet

A quick reference for common Git commands.

## Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list
```

## Getting Started

```bash
git init                   # Initialize a new repository
git clone <url>            # Clone a repository
```

## Basic Snapshotting

```bash
git status                 # Show status of changes
git add <file>             # Stage file(s)
git add .                  # Stage all changes
git commit -m "message"    # Commit staged changes
git diff                   # Show unstaged changes
git diff --staged          # Show staged changes
```

## Branching & Merging

```bash
git branch                 # List branches
git branch <name>          # Create new branch
git checkout <branch>      # Switch branches
git checkout -b <name>     # Create and switch to new branch
git merge <branch>         # Merge branch into current
git branch -d <name>       # Delete branch
```

## Remote Repositories

```bash
git remote -v              # List remotes
git remote add origin <url> # Add remote repository
git fetch                  # Fetch changes from remote
git pull                   # Fetch and merge changes
git push                   # Push commits to remote
git push -u origin <branch> # Set upstream branch
```

## Undoing & Resetting

```bash
git checkout -- <file>     # Discard changes in file
git reset HEAD <file>      # Unstage file
git revert <commit>        # Create new commit to undo changes
git reset --hard <commit>  # Reset to a specific commit (DANGEROUS)
```

## Stashing

```bash
git stash                  # Stash changes
git stash pop              # Apply and remove latest stash
git stash list             # List stashes
git stash apply            # Apply stash
```

## Viewing History

```bash
git log                    # Show commit logs
git log --oneline          # Compact log
git log --graph --all      # Visualize branch history
```

## Tagging

```bash
git tag                    # List tags
git tag <name>             # Create tag
git tag -a <name> -m "msg" # Annotated tag
git push --tags            # Push tags to remote
```

## Other Useful Commands

```bash
git show <commit>          # Show details of a commit
git rm <file>              # Remove file and stage deletion
git mv <old> <new>         # Rename or move file
```

---

**Tip:** Use `git help <command>` for detailed info on any command.

