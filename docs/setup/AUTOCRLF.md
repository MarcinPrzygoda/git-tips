# 📋 AUTOCRLF

Line endings vary between **operation systems**.

| LINE ENDING                            | SYSTEM      |
| -------------------------------------- | ----------- |
| `\n` (line feed)                       | Unix, MacOS |
| `\r\n` (carriage return and line feed) | Windows     |

When you **mix platforms**, such as when you perform your development on a Windows machine, and then you run your system on a Unix machine, there can be **issues** if line endings are not handled properly.

| COMMAND                                      | DESCRIPTION                                                     |
| -------------------------------------------- | --------------------------------------------------------------- |
| `git config --global core.autocrlf <option>` | add configuration for autocrlf handling to `${HOME}/.gitconfig` |

| AUTOCRLF OPTION | RESULT                                            | WHEN TO USE                  |
| --------------- | ------------------------------------------------- | ---------------------------- |
| `input`         | Commit `\r\n` to `\n`<br/>Checkout `\n` to `\n`   | Cross-platform + Unix, MacOS |
| `true`          | Commit `\r\n` to `\n`<br/>Checkout `\n` to `\r\n` | Cross-platform + Windows     |
| `false`         | No conversions                                    | Single platform              |