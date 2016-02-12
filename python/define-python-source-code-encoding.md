# Define Python Source Code Encoding

Defining Python source code encoding makes it is easier to use
non-Latin-1 literal strings in Python source code.
To do this, a magic comment must be placed into the source file
either as first or second line in the file. The magic comment 
must match the regular expression `coding[:=]\s*([-\w.]+)`.

For example, if you want to set UTF-8 as the encoding of your
source code, you can put
```
# -*- coding: utf-8 -*-
```
at the first or second line in your code.
You can even use a format that can be reconginzed by Vim
```
#vim:fileencoding=utf-8
```

For more details, please refer to [PEP 0623](https://www.python.org/dev/peps/pep-0263/).