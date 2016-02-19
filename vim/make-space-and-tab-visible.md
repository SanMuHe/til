# Make Space and Tab Visible

Vim can display unprintable characters with `list` command and `listchars` option. 
It can be used to highlight unwanted tabs or trailing spaces.

For example, the below
setting will show all tabs as `>---` and all trailing spaces as `-`.

```
set list listchars=tab:>-,trail:-
```

See `:h listchars` for more information.
