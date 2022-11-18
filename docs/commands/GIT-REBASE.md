# 📋 `git rebase` - reapply commits on top of another base tip

Rebasing means that we **take commits** from **branch** and **replay them** at the end of **another branch**. It is useful to integrate recent commits **without merging**. It maintains a **cleaner**, more **liner project history**.

| COMMAND                             | DESCRIPTION                                                                 |
| ----------------------------------- | --------------------------------------------------------------------------- |
| `git rebase <base-branch>`          | rebase current branch to tip of `<base-branch>` [🔗](#rebase-current-branch) |
| `git rebase <base-branch> <branch>` | rebase `<branch>` to tip of `<base-branch>`                                 |

## 📌 Conflicts when rebasing

When you `rebase` a branch, it's possible for it to **have conflicts**. And if you do have conflicts, it will work just like [merge conflicts](../concepts/MERGE-CONFLICTS.md) do. One difference is that after we resolve the conflicts, we go to the **next commit** and keep going down the chain of commits.

## 📌 Merge vs Rebase

See [Merge vs Rebase](../concepts/MERGE-VS-REBASE.md)

## 📌 Example

### Rebase current branch

![](images/git-rebase.png)