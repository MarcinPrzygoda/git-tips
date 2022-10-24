# Reset types

**Reset** changes the files in the **staging index** and/or **working directory** to the state they had when a **specified commit was made**. It moves **HEAD** pointer to a **specific commit**.

> "Make my project look like it did back then"

There are 3 types of reset:
* **[soft](SOFT-RESET.md)** - `git reset --soft <tree-ish>`:
  * moves HEAD pointer
  * does not change staging index
  * does not change working directory
* **mixed** - `git reset --mixed <tree-ish>` (this is **default** option for `git reset`):
  * moves HEAD pointer
  * changes staging index to match repository
  * does not change working directory
* **hard** - `git reset --hard <tree-ish>`:
  * moves HEAD pointer
  * changes staging index to match repository
  * changes working directory to match repository