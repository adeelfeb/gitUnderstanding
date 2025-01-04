# Understanding `git reset`

The `git reset` command is a powerful tool in Git that allows you to undo changes in your repository. It's versatile and can affect your working directory, staging area, and commit history depending on how it's used. This document explains the concept, usage, and types of resets in Git.

---

## Why Use `git reset`?

1. **Undoing Changes**: Roll back changes made to files, staging, or commits.
2. **Editing Commit History**: Rewrite commit history when needed (e.g., for squashing commits).
3. **Removing Changes from the Index**: Unstage files without altering their content.
4. **Cleaning Up Before a Commit**: Reset specific files or the entire working directory.

---

## Types of Resets in Git

The `git reset` command operates in three main modes, depending on the provided option: `--soft`, `--mixed`, and `--hard`. Each mode specifies how the reset impacts your working directory, staging area, and commit history.

### 1. **Soft Reset** (`git reset --soft <commit>`)

- **Effect**: Moves the `HEAD` pointer to the specified commit but keeps all changes staged.
- **Use Case**: When you want to modify the last commit or start fresh from a specific point without losing your staged changes.

#### Example:
```bash
git reset --soft HEAD~1
