# Filter the Commit Log

`git log -3` - show last three commits:

![](images/git-log-number.png)

---
`git log --since=2022-10-06` - show commits after given date

![](images/git-log-since.png)

`git log --until=2022-10-06` - show commits before given date

![](images/git-log-until.png)

**Other formats:**
* `git log --until="3 days ago"`
* `git log --after=2.weeks --before=3.days`

---
`git log --author="Marcin"` - show commits done by Marcin

![](images/git-log-author.png)

---
`git log --grep="Initial"` - show commits that match the specified pattern

![](images/git-log-grep.png)

---
`git log 01e71d96..HEAD` - show commits in range

![](images/git-log-range.png)

---
`git log commit-tree/TREE-ISH.md` - show commits related to a file or directory

![](images/git-log-file.png)