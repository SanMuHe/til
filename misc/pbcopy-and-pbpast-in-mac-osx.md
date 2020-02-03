# pbcopy and pbpast in Mac OSX command line

You can use command `pbcopy` and `pbpast` to interact with the system clipboard in Mac OSX.

```bash
echo 'Hello World' | pbcopy  # Copy from stdin to clipboard
echo `pbpast`  # Copy from clipboard to stdout
```
