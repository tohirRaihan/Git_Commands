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

### Comparison:

| Command | Description |
| ------- | ----------- |
| `git diff` | Show differences between the repository and working directory |
| `git diff --staged` | Show differences between the repository and the staging |
| `git diff --color-words` | Show only words that are different |
| `git diff <branch>..<branch>` | Compare branches |
| `git show` | Show `diff` between last two commits |
| `git show <SHA>..<SHA>` | Show `diff` between two specific commits |
| `git show <SHA>..<SHA> --color-words` | Show only words that are different |

### Branching & Merging:

| Command | Description |
| ------- | ----------- |
| `git branch` | Show list of the branches |
| `git branch <name>` | Create branch |
| `git checkout <branch>` | Switch branch |
| `git checkout -b <name>` | Create and switch branch |
| `git branch --merged` | Check what other branches have all of their commits merged into this branch already |
| `git branch --no-merged` | Does the opposite of `branch --merged` |
| `git branch -m <old name> <new name>` | Rename branch |
| `git branch -d <branch>` | Delete branch |
| `git merge <branch>` | Merge a branch into the active branch |
| `git merge <source branch> <target branch>` | Merge a branch into a target branch |

### Rewrite History:

| Command | Description |
| ------- | ----------- |
| `git reset --soft <tree-ish>` | Soft reset |
| `git reset <tree-ish>` | Mixed reset |
| `git reset --hard <tree-ish>` | Hard reset |
