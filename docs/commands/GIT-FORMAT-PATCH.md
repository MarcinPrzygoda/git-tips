# 📋 `git format-patch` - prepare patches for e-mail submission

| COMMAND                                                                                | DESCRIPTION                                                                                                                                                            |
| -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git format-patch <commit>..<commit>`                                                  | export all commits in the range in Unix mailbox format into current directory, which is useful for e-mail distribution of changes. For each commit one file is created |
| `git format-patch <commit>..<commit> --stdout > <file.patch>`                          | export all commits in the range as a single file                                                                                                                       |
| `git format-patch main`                                                                | export all commits on current branch which are not in `main` branch into current directory                                                                             |
| `git format-patch main -o <dir>`<br />`git format-patch main --output-directory <dir>` | export all commits on current branch which are not in `main` branch into `<dir>` directory                                                                             |
| `git format-patch -1 <commit>`                                                         | export a single commit into current directory                                                                                                                          |

## 📌 Applying formatted patch

You can apply formatted patch with [`git am`](GIT-AM.md) command.