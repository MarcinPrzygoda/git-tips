# 📋 `git branch` - list, create or delete branches

The default branch name in Git is **master** (in GitHub it is **main**).

| COMMAND                                   | DESCRIPTION                                                                                                                                            |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `git branch`                              | list local branches [🔗](#list-local-branches)                                                                                                          |
| `git branch --merged`                     | list only branches whose tips **are reachable** from the specified commit. All the commits are in checked out branch [🔗](#merged-vs-no-merged)         |
| `git branch --no-merged`                  | list only branches whose tips **are not reachable** from the specified commit. Not all the commits are in checked out branch [🔗](#merged-vs-no-merged) |
| `git branch -r`                           | list remote branches                                                                                                                                   |
| `git branch -a`                           | list both local and remote branches                                                                                                                    |
| `git branch <branch>`                     | create local `<branch>` [🔗](#create-local-branch)                                                                                                      |
| `git branch -m <new-branch>`              | rename (move) current branch to `<new-branch>` [🔗](#rename-current-branch)                                                                             |
| `git branch -m <old-branch> <new-branch>` | rename (move) `<old-branch>` to `<new-branch>`                                                                                                         |
| `git branch -d <branch>`                  | delete `<branch>` [🔗](#delete-branch)                                                                                                                  |
| `git branch -D <branch>`                  | force delete `<branch>` [🔗](#force-delete-branch)                                                                                                      |
| `git branch -u <upstream> <branch>`       | set `<upstream>` ([**tracking**](../concepts/TRACK-REMOTE-BRANCHES.md)) reference for `<branch>`                                                       |
| `git branch --unset-upstream <branch>`    | unset upstream ([**tracking**](../concepts/TRACK-REMOTE-BRANCHES.md)) reference for `<branch>`                                                         |

## 📌 Branch naming convention

Remember, **every commit** on `main` branch is a **new release** by definition.

| BRANCH NAME           | DESCRIPTION                                                                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| `develop`             | branch with an infinite lifetime (similarly to `main`) where development process is done                                                      |
| `release/version`     | branch preparing a release (branch off from `develop`, merge back into `develop` and `main`)                                                  |
| `feature/branch-name` | branch adding a new functionality during development process (branch off from `develop`, merge back into `develop`)                           |
| `bugfix/branch-name`  | branch fixing a bug during development process (branch off from `develop`/`release`/`feature`, merge back into `develop`/`release`/`feature`) |
| `hotfix/branch-name`  | branch patching a bug on already released version (branch off from `main`, merge back into `develop`/`release` and `main`)                    |

See "[A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)" for more information.

## 📌 Renaming branches

You don't want to start renaming your branches **if other people are already using them by another name**.

## 📌 Deleting branches

You can't delete checked out branch and branches which are not fully merged [🔗](#delete-checked-out-branch)

## 📌 Examples

Branch colored **green** means that this is checked out branch.

### List local branches

![](images/git-branch.png)

### Merged vs no merged

Knowing which branches are fully included in another branch is very useful. Especially, when we start deleting branches:

![](images/git-branch-merged-vs-no-merged.png)

### Create local branch

![](images/git-branch-create.png)

### Rename current branch

![](images/git-branch-move.png)

### Delete branch

![](images/git-branch-delete.png)

### Delete checked out branch

![](images/git-branch-delete-warn.png)

### Force delete branch

![](images/git-branch-delete-force.png)