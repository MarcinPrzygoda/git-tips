# Compare branches

`git diff <tree-ish>` - compare two files or any tree-ish

Typically, you put the older branch first during comparison. In the example below, `main` branch is older:

![git-diff.png](images/git-diff-branches.png)

![git-diff-branches-reverse.png](images/git-diff-branches-reverse.png)

---
`git diff --color-words <tree-ish>` - **highlight changed words** using only colors (there are no `+`/`-`)

---
`git branch --merged` - only list branches whose tips **are reachable** from the specified commit. All the commits are in checkout branch.

`git branch --no-merged` - only list branches whose tips **are not reachable** from the specified commit. Not all the commits are in checkout branch.

Knowing which branches are fully included in another branch is very useful. Especially, when we start deleting branches.

![git-branch-merged-vs-no-merged.png](images/git-branch-merged-vs-no-merged.png)