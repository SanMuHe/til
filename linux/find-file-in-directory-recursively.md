# Find File in Directory Recursively

You can use `find /path/to/search -name '*.py' -type f` to recursively find all `.py` files in directory `/path/to/search` and its sub-directories. The option `-type f` will restrict the results to be files only (i.e., directories with substring `.py` in their name will be excluded).