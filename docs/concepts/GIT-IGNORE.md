# 📋 `.gitignore`

| URL                                                                | DESCRIPTION                                         |
| ------------------------------------------------------------------ | --------------------------------------------------- |
| [github.com/github/gitignore](https://github.com/github/gitignore) | GitHub’s collection of `.gitignore` file templates. |
| [gitignore.io](https://gitignore.io)                               | `.gitignore` file generator                         |

The file `project/.gitignore` lists rules to determine which files Git should **ignore**. Changes made to ignored files will be ignored by Git.

## 📌 Pattern matching

Git understands [basic regular expressions](https://git-scm.com/docs/gitignore#_pattern_format) in `.gitignore` file.

| PATTERN                          | DESCRIPTION                                                                                                                |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| `access.log`                     | ignore `access.log` file                                                                                                   |
| `.settings`                      | ignore all files in `.settings` directory, the directory itself and files with the same name                               |
| `assets/videos/`                 | ignore all files in `assets/videos` directory and the directory itself (all paths are relative from the `.gitignore` file) |
| `**/assets/videos/`              | ignore all files in `assets/videos` directory and the directory itself anywhere in the project                             |
| `logs/*.log`                     | ignore all files in `logs` directory that end with `.log`                                                                  |
| `*.xml`</br>`!configuration.xml` | ignore all files that end with `.xml` except `configuration.xml`                                                           |

## 📌 Comments

You can put **comments** in `.gitignore` file after `#` character:
```md
# This is a comment
```

## 📌 Globally ignore files

| COMMAND                                                     | DESCRIPTION                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------- |
| `git config --global core.excludesfile ~/.gitignore_global` | set user specific `.gitignore` file (for all user projects) |

## 📌 Ignore tracked files

See [`git rm --cached`](../commands/GIT-RM.md)

## 📌 Example

![](images/gitignore.png)