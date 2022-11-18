# 📋 `git blame` - show what revision and author last modified each line of a file

Useful for identifying which commit introduced a bug.

| COMMAND                                                          | DESCRIPTION                                                                           |
| ---------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `git blame <file>`                                               | annotate `<file>`, so you can determine who changed which lines in a `<file>` and why |
| `git blame -w <file>`                                            | ignores changes done to whitespace                                                    |
| `git blame -L 100,150 <file>`<br />`git blame -L 100,+50 <file>` | annotate only lines 100-150 of the `<file>`                                           |
| `git blame <commit> <file>`                                      | annotate `<file>` at `<commit>` revision                                              |