# 📋 `git add` - add file contents to the staging index

| COMMAND             | DESCRIPTION                                                                                      |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| `git add <file>...` | add files to the staging index [🔗](#add-a-file-to-the-staging-index)                             |
| `git add .`         | add all files in current directory to the staging index [🔗](#add-all-files-to-the-staging-index) |

| OPTION                    | DESCRIPTION                                                                                                 |
| ------------------------- | ----------------------------------------------------------------------------------------------------------- |
| `-i`<br />`--interactive` | enter staging in interactive mode [🔗](#run-staging-in-interactive-mode)                                     |
| `-p`<br />`--patch`       | enter staging in patch mode (shortcut to patch mode in interactive staging) [🔗](#run-staging-in-patch-mode) |

## 📌 Untracked file

**Untracked file** is a file that have been created within working directory but have not yet been added to the **staging index** using the `git add` command. It means that changes done in untracked file are **not tracked** by Git.

## 📌 Interactive staging

Interactive staging enters an **interface** that allows to **move files** or **portions of changed files** in and out of staging index.

## 📌 Examples

### Add a file to the staging index

![](images/git-add.png)

### Add all files to the staging index

![](images/git-add-all-files.png)

### Run staging in interactive mode

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

Interactive patch help:

![](images/git-add-interactive-staging-help.png)

## Run staging in patch mode

![](images/git-add-patch-mode.png)