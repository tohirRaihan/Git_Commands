# Git Commands
_A list of most important and commonly used Git commands for easy reference_:sparkles::sparkles:
___

### Basic Snapshotting:

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize git in a project |
| `git status` | Check status |
| `git add <file>` | Add a file to the staging area |
| `git add .` | Add all changes that are in the current directory to the staging area |
| `git restore <file>` | Discard changes in working directory |
| `git restore --staged <file>` | Unstage a file |
| `git restore --staged .` | Unstage all files of the current directory that are staged |
| `git rm <file>` | Delete a file |
| `git mv <file> <new_file>` | Move or rename a file |
| `git commit` | Commit changes (multiple line message) |
| `git commit -m "<commit message>"` | Commit changes (single line message) |
| `git commit -am "<commit message>"` | Stages and Commits together (does’t include untracked files) |
| `git commit --amend -m "<commit message>"` | Amend Commits |
