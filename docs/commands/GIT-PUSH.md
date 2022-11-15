# 📋 `git push` - update remote refs along with associated objects

| COMMAND                                                                            | DESCRIPTION                                                                                                                                                                                                                                                                                                       |
| ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git push <repository> <branch>`<br />`git push`                                   | push committed changes on `<branch>` into remote `<repository>`. The `-u` option is not needed when remote branch is already tracked. You also don't have to specify `<repository>` and `<branch>` parameters [🔗](#push-committed-changes-on-branch-into-remote-repository)                                       |
| `git push -u <repository> <branch>`                                                | push committed changes on `<branch>` into remote `<repository>`. Use `-u` option to add upstream ([**tracking**](../concepts/TRACK-REMOTE-BRANCHES.md)) reference, especially when you're creating a `<branch>` for the first time [🔗](#push-committed-changes-on-branch-into-remote-repository-and-add-upstream) |
| `git push <repository> <tag>`                                                      | push `<tag>` into remote `<repository>`                                                                                                                                                                                                                                                                           |
| `git push <repository> --tags`                                                     | push all tags into remote `<repository>`                                                                                                                                                                                                                                                                          |
| `git push -f`<br />`git push --force`                                              | force push, replace remote version with local version [🔗](#-force-push)                                                                                                                                                                                                                                           |
| `git push <repository> :<remote-branch>`                                           | delete remote branch (local branch is not deleted). Regular push is doing `<local-branch>:<remote-branch>` which is like "push `<local-branch>` to `<remote-branch>`" The `:<remote-branch>` is like "push nothing to `<remote-branch>`". It's old style way [🔗](#delete-remote-branch-old-style-way)             |
| `git push -d <repository> <branch>`<br />`git push --delete <repository> <branch>` | improved way of deleting remote branch [🔗](#delete-remote-branch)                                                                                                                                                                                                                                                 |
| `git push -d <repository> <tag>`                                                   | improved way of deleting remote tag                                                                                                                                                                                                                                                                               |

## 📌 Force Push

We use force push when:
- local version is **better** than the remote version
- remote version went wrong and needs **repair**
- versions have diverged and merging is **undesirable**

Use it with **extreme caution**. It is an easy way to anger your whole development team, because other commits can **disappear**. Any subsequent commits that they've made in their local repository that were dependent on those commits, are now **orphaned**.

## 📌 Example

### Push committed changes on branch into remote repository

![](images/git-push.png)

### Push committed changes on branch into remote repository and add upstream

![](images/git-push-upstream.png)

### Delete remote branch (old style way)

![](images/git-push-nothing.png)

### Delete remote branch

![](images/git-push-delete.png)