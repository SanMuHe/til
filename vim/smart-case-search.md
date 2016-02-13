# Smart Case Search

You can enable the *smart* case search feature in Vim by putting the following
settings to your vimrc file.


```
set ignorecase
set smartcase
```

If a pattern contains an uppercase letter, it is case sensitive, otherwise, it is not. For example, `/The` would find only `The`, while `/the` would find `the` or `The` etc.