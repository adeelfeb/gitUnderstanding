# Understanding `git stash`

## What is `git stash`?

`git stash` is a powerful Git command that allows you to temporarily save changes in your working directory and staging area without committing them. It is particularly useful when you need to switch branches or perform other operations but aren't ready to commit your current changes.

---

## Why Use `git stash`?

1. **Switching Branches Safely**:  
   Suppose you're working on `branch-A` and need to quickly switch to `branch-B` to fix a bug or review changes. If you have uncommitted changes, Git will prevent you from switching branches. `git stash` allows you to save those changes temporarily, switch branches, and apply them later.

2. **Avoiding Dirty Commits**:  
   Sometimes, you're not ready to commit because your changes are incomplete or experimental. Instead of committing unfinished work, you can stash it until you're ready to proceed.

3. **Experimenting Without Risk**:  
   You can stash your changes, experiment with something new, and then restore your original work.

4. **Maintaining Clean Working Directories**:  
   `git stash` helps keep your working directory clean without losing your progress.

---

## Common `git stash` Commands

### 1. Save Changes to the Stash
```bash
git stash
