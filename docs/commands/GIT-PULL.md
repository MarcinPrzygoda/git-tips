# 📋 `git pull` - fetch from and integrate with another repository or a local branch

| COMMAND                                                      | DESCRIPTION                                          |
| ------------------------------------------------------------ | ---------------------------------------------------- |
| `git pull`                                                   | it is two-step operation: `git fetch` + `git merge`  |
| `git pull -r`<br />`git pull --rebase`                       | it is two-step operation: `git fetch` + `git rebase` |
| `git pull --rebase=merges`<br />`git rebase --rebase-merges` | local merge commits are included in the rebase       |
| `git pull --rebase=interactive`                              | enter rebase in interactive mode                     |

## 📌 Pull with Merge vs Rebase

Pull with Rebase keeps history **cleaner** by reducing merge commits. However, only use it on local commits which are **not shared to a remote**.

## 📌 Example

![](images/git-pull.png)