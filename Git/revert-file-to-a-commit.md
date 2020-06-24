# Revert File To A Particular Commit

I usually use the below flow of commands to revert the file to a particular commit.

```bash
git log -- path-to-file  # Show the history of a file
git diff commit-hash-1..commit-hash-2 path-to-file  # Show the difference of a file between two commits
git checkout commit-hash path-to-file . # Revert the file to a particular commit
```
