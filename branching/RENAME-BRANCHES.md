# Rename branches

`git branch -m [<oldbranch>] <newbranch>` or `git branch --move [<oldbranch>] <newbranch>` - rename (move) branch. Optionally you can provide `<oldbranch>` if you're on **different branch**. When `<oldbranch>` is not provided, you rename **current checkout branch**.

![git-branch-move.png](images/git-branch-move.png)

You don't want to start renaming your branches **if other people are already using them by another name**.