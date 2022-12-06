# 📋 `git clean` - remove untracked files from the working directory

| COMMAND            | DESCRIPTION                                                                                                                                           |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git clean`        | remove untracked files in current directory when `clean.requireForce` config defaults to `true`, otherwise git will refuse to execute clean operation |
| `git clean <path>` | remove untracked files under `<path>` when `clean.requireForce` config defaults to `true`, otherwise git will refuse to execute clean operation       |

| OPTION                | DESCRIPTION                                                                                                                                                                              |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `-f`<br />`--force`   | remove untracked files                                                                                                                                                                   |
| `-n`<br />`--dry-run` | don’t actually remove anything, just show what would be done                                                                                                                             |
| `-d`                  | normally, when no `<path>` is specified, git clean will not recurse into untracked directories to avoid removing too much. Specify `-d` to have it recurse into such directories as well |
| `-x`                  | normally, only files unknown to Git are removed, but if the `-x` option is specified, ignored files are also removed                                                                     |
| `-X`                  | remove only files ignored by Git. This may be useful to rebuild everything from scratch, but keep manually created files                                                                 |

## 📌 Example

![](images/git-clean.png)