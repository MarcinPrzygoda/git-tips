# Format the Commit Log

`git log -p` - show commits with a patch (changelist) information

![](images/git-log-patch.png)

---
`git log --stat` - show commits statistics

![](images/git-log-stat.png)

---
`git log --format=oneline` - show commits in different format

![](images/git-log-format.png)

**Format options:**
* oneline
* short
* medium **(default)** - equivalent to `git log` command
* full
* fuller
* email
* raw

---
`git log --oneline` - show commits in one line with shorter SHA-1 hash

![](images/git-log-oneline.png)

---
`git log --graph` - show commits graph

![](images/git-log-graph.png)

---
`git log --all --decorate --oneline --graph` - show commits graph of all branches in one line with decoration.

Think of the mnemonic `a dog` as a good way to remember this combo

![](images/git-log-graph-oneline.png)