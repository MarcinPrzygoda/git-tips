# 📋 `git commit` - record changes to the repository

| COMMAND                             | DESCRIPTION                                                                                                           |
| ----------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `git commit`                        | create a new commit containing the current contents of the staging index and multiline message describing the changes |
| `git commit -m "<message>"`         | create a new commit with one line `<message>` [🔗](#commit-changes)                                                    |
| `git commit -am "<message>"`        | automatically stage tracked files that have been modified/deleted and create a new commit                             |
| `git commit --amend -m "<message>"` | replace the tip of the current branch by creating a new commit [🔗](#amend-commit)                                     |

## 📌 No commit message

When Git is not provided a commit message, it will **abort the commit**. Using the "-m" option with empty quotes has the same result as exiting a text editor without providing a message.

## 📌 Atomic commit

- **small** commit
- only affect **a single aspect** (relate to one thing)
- **easier** to understand, to work with and to find bugs
- **improves** collaboration

## 📌 Example

### Commit changes

![](images/git-commit.png)

### Amend commit

![](images/git-commit-amend.png)

![](images/git-commit-amend-result.png)