# Move to First or Last Non-Blank Character of Line

In Vim normal mode, you can type `0` to move to the start of the line and `$` to the end of the line. The start or end of the line can be blank characters. But if you just want to move to the first or the last non-blank character of the line, you can type `^` and `g_` respectively.

`g_` is also very useful when you want to avoid selecting the line break character in visual mode. For example, `vg_` will select all the characters from the cursor position to the end of the line excluding the line break character.