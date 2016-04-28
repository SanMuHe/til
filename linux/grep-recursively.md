# Grep Recursively

If you want to find a string in all directories and subdirectories, you can use 

```
grep -r pattern /path/to/start
```

If you want to include or exclude particular file types during the search, you can use

```
grep -r --include "*.txt" pattern /path/to/start
grep -r --exclude "*.txt" pattern /path/to/start
```