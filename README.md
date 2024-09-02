# GRID - Git Reimplemented in Dash

GRID is a simple yet powerful version control system implemented entirely in POSIX-compatible shell scripts. It aims to replicate a subset of Git's core functionality, providing a lightweight and educational tool for understanding version control concepts.

## GRID Commands

1. **`grid-init`**: Initializes an empty GRID repository by creating a `.grid` directory to store repository data.
2. **`grid-add [filenames...]`**: Adds files to the staging area for the next commit.
3. **`grid-commit -m [message]`**: Commits staged changes to the repository with a descriptive message.
4. **`grid-log`**: Displays a list of all commits, including their commit numbers and messages.
5. **`grid-show [commit]:[filename]`**: Displays the contents of a specified file at a given commit.
6. **`grid-commit [-a] -m [message]`**: Commits changes with the `-a` option to automatically add all tracked files.
7. **`grid-rm [--force] [--cached] [filenames...]`**: Removes files from the staging area or the working directory.
8. **`grid-status`**: Displays the status of files in the working directory, staging area, and repository.
9. **`grid-branch [-d] [branch-name]`**: Manages branches by creating, deleting, or listing them.
10. **`grid-checkout [branch-name]`**: Switches between branches.
11. **`grid-merge (branch-name|commit-number) -m [message]`**: Merges changes from a specified branch or commit into the current branch.
