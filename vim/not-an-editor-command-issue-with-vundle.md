# Not An Editor Command Issue With Vundle

After I re-image my Mac Pro, I have to setup my Vim again.
Thanks to the idea of [dotfiles](https://dotfiles.github.io/), I just need to clone my vim dotfiles from my github repository.
After doing that, I got the errors similar to below when I opened the Vim
```
line 10:
E492: Not an editor command: Plugin 'VundleVim/Vundle.vim'
...
...
line 29:
E117: Unknown function: vundle#end
```

If you also met the same issue, you can try the below method I found from Vundle's [Issue 486](https://github.com/VundleVim/Vundle.vim/issues/486).
* Configure git config by using `git config --global core.autocrlf input`.
* Delete the vundle folder (It will be `~/.vim/bundle/Vundle.vim` if you follow Vundle's install instructions).
* Re-install vndle by using `git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`.