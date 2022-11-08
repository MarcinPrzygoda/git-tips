# 📋 `git config` - get and set configuration entries

Configuration values list: [Git Documentation](https://git-scm.com/docs/git-config#_variables)

| COMMAND                             | DESCRIPTION                            |
| ----------------------------------- | -------------------------------------- |
| `git config --system <key> <value>` | edit system level configuration entry  |
| `git config --global <key> <value>` | edit user level configuration entry    |
| `git config <key> <value>`          | edit project level configuration entry |
| `git config <key>`                  | show configuration entry               |
| `git config --list`                 | list configuration entries             |

## 📌 System level configuration

`/etc/gitconfig` - apply to every user

## 📌 User level configuration

`${HOME}/.gitconfig` - apply to single user

## 📌 Project level configuration

`project/.git/config` - apply to single project