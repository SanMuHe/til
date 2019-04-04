# Rename Local Branch

If you want to rename a branch while pointed to any branch, do:

```bash
git branch -m <oldname> <newname>
```

If you want to rename the current branch, you can do:

```bash
git branch -m <newname>
```

A way to remember this, is `-m` is for "move" (or `mv`), which is how you rename files.

**Reference:** https://stackoverflow.com/questions/6591213/how-do-i-rename-a-local-git-branch