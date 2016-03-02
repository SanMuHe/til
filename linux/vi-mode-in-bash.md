# Vi Mode in Bash

You can enable the Vi edit mode in bash command line by putting `set -o vi` in the `.bashrc` file (you need to resource the `.bashrc` file to make that setting takes effect.). By default, the bash command line will be in *insert* mode, you can press `Esc` to switch to *normal* mode. Then you can use the classic Vi key mapping to move the position of the cursor, delete, and yank. Also note that `k` and `j` in normal mode allow you to iterate through your command history.

There are alternative ways to enable Vi mode in bash. Please refer to [Use vi shortcuts in terminal](http://vim.wikia.com/wiki/Use_vi_shortcuts_in_terminal) and [Vi mode in Bash](http://blog.sanctum.geek.nz/vi-mode-in-bash/).