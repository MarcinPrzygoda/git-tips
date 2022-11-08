# 📋 DISTRIBUTED VERSION CONTROL

Version control is a system that **records changes** to a file or set of files over time so that you can recall **specific versions** later.

**Centralized Version Control** is a system (such as [CVS](https://www.gnu.org/software/trans-coord/manual/cvs/cvs.html) or [SVN](https://subversion.apache.org/)) which have a **single server** that contains all the versioned files, and a number of **clients** that check out files from that central place.

Git is **Distributed Version Control System** created by **Linus Torvalds** (a person who created **Linux**) in **April 2005**.

## 📌 In Distributed Version Control different users maintain their own repositories

- there is **no single master repository**, just **many working copies** each with their own combination of **changesets** (patches)
- all repositories are considered **equal** by Git

## 📌 In Distributed Version Control changes are stored as changesets

- it tracks **changes**, not versions
- it is different from [CVS](https://www.gnu.org/software/trans-coord/manual/cvs/cvs.html) and [SVN](https://subversion.apache.org/), which track **versions**
- changesets can be exchanged **between repositories**

## 📌 Advantages compared with Centralized Version Control

- speeds up most operations (except pushing and pulling)
- improves the ability to work offline
- does not rely on a single location for backups