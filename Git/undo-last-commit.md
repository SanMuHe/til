# Undo Last Commit

Sometimes I found I perform the commit so quickly without double checking the staged files (a typcial example is using the `Stage All Changes` feature of my IDE) and so the commit has unwanted changes.

To undo my last commit, I use

```bash
git reset --soft HEAD~1
```

This command will reset my git workspace to the revision before the current revision. Note the `--soft` flag is to make sure the changes in the undone revisisons are preserved.

If you don't want to keep the changes, simple use

```bash
git reset --hard HEAD~1
```
