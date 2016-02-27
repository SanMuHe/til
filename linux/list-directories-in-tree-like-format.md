# List Directories in Tree-Like Format

The `tree` command is really neat and useful tool to view the structure of your file system in a tree-like format.
For example, 

- `tree` displays the contents of the current directory and subdirectories in a tree-like format.
- `tree -P 't*'` displays only directories beginning with `t` or directories containing files that begin with `t`.
- `tree -d` displays directories only.
- `tree -L 2` restricts the max depth of the subdirectories to be 2.

Note: if your get "command not found" error when run the tree command, you can install it with `sudo apt-get install tree`.