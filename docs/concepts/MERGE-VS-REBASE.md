# 📋 MERGE VS REBASE

[**Merging**](../commands/GIT-MERGE.md) and [**rebasing**](../commands/GIT-REBASE.md) are two ways to **incorporate changes** from one branch into another branch. The result is similar, but the means of doing it are **very different**.

## 📌 Merge

- **adds** a merge commit
- is **nondestructive**
- we **have** complete record of what happened and when
- it is **easy** to undo via [`git reset`](../commands/GIT-RESET.md)
- logs can become **cluttered**, **non-linear**

## 📌 Rebase

- **no additional** merge commit
- is **destructive**: SHA-1 hash changes, commits are rewritten
- we **no longer have** a complete record of what happened and when
- it is **tricky** to undo
- logs are **cleaner**, **more linear**

## 📌 The Golden Rule of Rebasing

> Thou shalt not rebase a public branch

Rebase **abandons** existing, shared commits and **creates new**, similar commits instead. Collaborators would see the **project history vanish**. Getting all collaborators back in sync can be a **nightmare**.

Rebasing should be used on your **local**, **private** branches or on branches that you use **exclusively**.

## 📌 How to choose?

- **Merge** to allow commits to stand out or to be clearly grouped.
- **Merge** to bring large topic branches back into main branch
- **Merge** anytime the topic branch is already public and being used by others ([The Golden Rule of Rebasing](#-the-golden-rule-of-rebasing))
- **Rebase** to add minor commits in main to a topic branch
- **Rebase** to move commits from one branch to another