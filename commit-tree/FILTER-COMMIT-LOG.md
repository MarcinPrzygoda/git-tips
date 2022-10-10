# Filter the Commit Log

`git log -3` - show last three commits:

![git-log-number.png](images/git-log-number.png)

---
`git log --since=2022-10-06` - show commits after given date

![git-log-since.png](images/git-log-since.png)

`git log --until=2022-10-06` - show commits before given date

![git-log-until.png](images/git-log-until.png)

**Other formats:**
* `git log --until="3 days ago"`
* `git log --after=2.weeks --before=3.days`

---
`git log --author="Marcin"` - show commits done by Marcin

![git-log-author.png](images/git-log-author.png)

---
`git log --grep="Initial"` - show commits that match the specified pattern

![git-log-grep.png](images/git-log-grep.png)

---
`git log 01e71d96..HEAD` - show commits in range

![git-log-range.png](images/git-log-range.png)

---
`git log commit-tree/TREE-ISH.md` - show commits related to a file or directory

![git-log-file.png](images/git-log-file.png)