# 📋 FORK REPOSITORY AND MAKE IT PRIVATE

1. Create a [new private repository on Github](https://github.com/new) and make it **Private**
2. `git clone https://github.com/user/original-repo.git dir`
3. `cd dir`
4. Create `.gitignore` file
5. `git init`
6. Check what will be committed with `git status`
7. `git commit -am "Initial commit"`
8. `git branch -m main`
9. `git remote add origin https://github.com/user/private-fork.git`
10. `git push -u origin main`
11. `git remote add upstream https://github.com/user/original-repo.git`
12. `git remote set-url --push upstream DISABLE`
13. You can list all your remotes with `git remote -v`
14. IntelliJ IDEA: `CTRL + SHIFT + ALT + S` -> `Modules` -> `+` icon -> `Import Module`
15. IntelliJ IDEA: `Git` tab -> `Log` tab -> `Open New Git Log Tab` (`+` icon) -> `Branch` -> `Select...` -> `origin/main | upstream/main` -> `CTRL + Enter` -> `Paths` -> `Choose module`