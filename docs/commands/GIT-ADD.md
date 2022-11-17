# 📋 `git add` - add file contents to the staging index

| COMMAND                                   | DESCRIPTION                                                                                           |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `git add <file>..`                        | add files to the staging index [🔗](#add-files-to-the-staging-index)                                   |
| `git add .`                               | add all files contents in current directory to the staging index [🔗](#add-files-to-the-staging-index) |
| `git add -i`<br />`git add --interactive` | enter staging in interactive mode [🔗](#run-interactive-staging)                                       |
| `git add -p`<br />`git add --patch`       | enter staging in patch mode (shortcut to patch mode in interactive staging)                           |

## 📌 Untracked file

**Untracked file** is a file that have been created within working directory but have not yet been added to the **staging index** using the `git add` command. It means that changes done in untracked file are **not tracked** by Git.

## 📌 Interactive staging

Interactive staging enters an **interface** that allows to **move files** or **portions of changed files** in and out of staging area.

## 📌 Example

### Add files to the staging index

![](images/git-add.png)

### Run interactive staging

Interactive update (add to staging):

![](images/git-add-interactive-staging-update.png)

Interactive revert (remove from staging):

![](images/git-add-interactive-staging-revert.png)

Interactively add untracked files:

![](images/git-add-interactive-staging-add-untracked.png)

Interactive diff between HEAD and staging index:

![](images/git-add-interactive-staging-diff.png)

Interactive patch (stage portions (hunks) of a changed file):

![](images/git-add-interactive-staging-patch.png)

Interactive patch with splitting hunks:

![](images/git-add-interactive-staging-patch-split.png)

Interactive patch with editing hunks:

![](images/git-add-interactive-staging-patch-edit.png)