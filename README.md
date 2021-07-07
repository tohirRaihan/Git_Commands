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

### Temporary Commits:

| Command | Description |
| ------- | ----------- |
| `git stash save "<label>"` | Save changes in the stash |
| `git stash list` | List stack-order of stashed file changes |
| `git stash show <stash>` | Show a stash in `diff --stat` |
| `git stash show -p <stash>` | Show stash in patched version |
| `git stash pop` | Remove single stash and apply it to the working directory |
| `git stash pop <stash>` | Pop specific stash |
| `git stash apply` | Same as `stash pop` but doesn't delete the stash |
| `git stash clear` | Clear all stash |
| `git stash drop` | Delete from top of stash stack |
| `git stash drop <stash>` | Delete specific stash |

### Others:

| Command | Description |
| ------- | ----------- |
| `git checkout <SHA> -- <file>` | Retrieve old version of a file |
| `git revert <SHA>` | Revert a commit |
| `git clean -f` | Remove untracked files |

### Sharing & Updating:

| Command | Description |
| ------- | ----------- |
| `git remote` | Manage set of tracked repositories |
| `git remote add <alias> <url>` | Add a git URL as an alias |
| `git remote -v` | Be a little more verbose and show remote url after name |
| `git remote rm <alias>` | Remove the remote named "`<alias>`" |
| `git push -u <alias> <branch name>` | Push the branch to remote repository (and track the branch) |
| `git push <alias> <branch name>` | Push the branch to the remote repository |
| `git branch --unset-upstream <branch name>` | The branch will not tracking anymore |
| `git clone <url>` | Create a local copy of a remote repository |
| `git push` | Push changes to remote repository of active branch (if a tracking branch) |
| `git fetch` | Fetch all changes from a remote repository |
| `git merge` | Merge a remote branch into your current branch to bring it up to date |
| `git pull` | `git fetch` + `git merge` |
| `git branch <branch name> <alias>/<branch name>` | Create branch based on remote tracking branch |
| `git push <alias> --delete <branch name>` | Remove a branch from the remote repository |
