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

### Inspection & Formation:

| Command | Description |
| ------- | ----------- |
| `git log` | Log all the commits |
| `git log -n 5` or `git log -5` | Last 5 commits |
| `git log --since=2020-07-03` | Log everything from that date |
| `git log --until=2021-07-03` | Log everything until that date |
| `git log --author="<Author Name>"` | Log all commits of this author |
| `git log --grep="<regex>"` | Search with regular expression from commit messages |
| `git log <SHA>..<SHA>` | Show all logs between those two commits |
| `git log <file>` | Log all commits focusing on a specific file or folder |
| `git log -p` | Show actual changes with each commit |
| `git log --stat` | Show statistics about what was changed in each commit |
| `git log --oneline` | Oneline view of all commits |
| `git log --graph` | Graph view of all commits |
| `git log --graph --all --oneline --decorate` | Nice & simple map view of all commits |
