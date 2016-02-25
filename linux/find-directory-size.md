# Find Size of Directory

The `du` command is used to estimate the file space usage. Since in Linux everything is a file, so this command can also be used to get the directory size. 

Below are several examples

- `du -a [FILE]` gives size of both the directories and all the files that are present in the current directory.
- `du -c [FILE]` gives the grand total size as the last line of the output.
- `du -s [FILE]` gives the summary of the directory size. It is the simplest way to know the total size of a directory.
- `du -S [FILE]` gives the size of the current directory excluding the size of the subdirectories that exist within that directory. So it basically shows you the total size of all the files that exist in the current directory.

Note: for all the above commands, you can combine with the `-h` option to output size in a *human readable format*.