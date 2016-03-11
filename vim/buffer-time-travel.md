# Buffer Time Travel

Vim allows you to go to an *earlier* text state for a buffer with
`:earlier`. For instance, if you want to see the state of the buffer from 10
minutes ago:

```
:earlier 10m
```

Similarly, you can move back toward the present text state of the buffer
with `:later`. If 10 minutes earlier was too far, you can come back 5
minutes like so:

```
:later 5m
```

**Reference** - [Josh Branchaud's TIL](https://raw.githubusercontent.com/jbranchaud/til/master/vim/buffer-time-travel.md)