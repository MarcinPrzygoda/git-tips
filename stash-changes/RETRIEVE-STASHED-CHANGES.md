# ⭐ Retrieve stashed changes

| COMMAND                     | DESCRIPTION                                                                                                     |
| --------------------------- | --------------------------------------------------------------------------------------------------------------- |
| `git stash pop stash@{1}`   | **remove** a single stashed state from the stash list and **apply** it on top of the current working tree state |
| `git stash apply stash@{1}` | like `pop`, but **does not remove** the state from the stash list                                               |

When you `pop` or `apply` changes out of your stash back into your working directory, it's possible for it to **have conflicts**. And if you do have conflicts, it will work just like a `merge` does.