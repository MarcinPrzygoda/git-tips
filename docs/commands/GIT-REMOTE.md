# 📋 `git remote` - manage set of tracked repositories

| COMMAND                                                                           | DESCRIPTION                                                                        |
| --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `git remote`                                                                      | list existing remotes                                                              |
| `git remote -v`                                                                   | list existing remotes together with remote url                                     |
| `git remote add <repository> <url>`                                               | add a remote named `<repository>` (usually `origin`) for the repository at `<url>` |
| `git remote remove <repository>`                                                  | remove the remote named `<repository>`                                             |
| `git remote prune <repository>`                                                   | remove stale remote-tracking branches                                              |
| `git remote prune <repository> -n`<br />`git remote prune <repository> --dry-run` | perform dry run of removing stale remote-tracking branches                         |

## 📌 Example

![](images/git-remote.png)