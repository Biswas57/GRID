# GRiD - Git Reimplemented in Dash

GRiD is a simple yet powerful version control system implemented entirely in POSIX-compatible shell scripts. It aims to replicate a subset of Git's core functionality, providing a lightweight and educational tool for understanding version control concepts.

## Overview of Engineering Requirements
Version control systems are a cornerstone of modern software development, enabling teams to track changes, collaborate, and maintain codebases efficiently. While Git is the most widely used version control tool, building a simplified version, such as GRID, offers a deeper understanding of its core functionalities and the underlying concepts.

**GRiD** is a simple yet powerful version control system that mimics some of the fundamental features of Git. It is implemented entirely in POSIX-compatible shell scripts and provides a practical learning experience in shell programming, version control, and system design.

This project builds on the essential mechanics of Git but with a more streamlined approach, focusing on core functionalities. The blog post outlines the design, implementation, testing strategies, and reflections on building GRID.

## Key Achievements
Some of the major accomplishments throughout this project were:

- Constructed a simplified version control system (GRID) emulating core Git functionalities using POSIX-compliant shell scripts.
- Implemented key commands like grid-init, grid-add, grid-commit, grid-log, grid-show, grid-rm, grid-status, grid-branch, grid-checkout, and grid-merge to provide a comprehensive set of version control tools.
- Ensured correctness and robustness by developing an extensive suite of test scripts to validate command behaviors against expected outputs.
- Created a dynamic branching and merging strategy to handle multiple branches efficiently while preserving data integrity.
- Developed a detailed command-line interface (CLI) for managing and interacting with the GRID system, showcasing its functionality through clear and user-friendly commands.
- Designed and documented the entire system structure to provide a clear understanding of GRID’s architecture, with emphasis on modular and scalable code design.

## Project Overview
**NOTE:** A complete visual overview of the entire system exists, showcasing the architecture in the final design diagram. A more extensive overview of the capabilities, constraints, and functionality of the system can be found in the Engineering Requirements.

### General Structure of the System

**Repository Structure:**

- GRID Repository → .grid Directory
- Staging Area → .grid/index
- Commit History → .grid/commits
- Branches → .grid/branches

**GRID Commands**

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
