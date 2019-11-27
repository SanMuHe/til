# Linux Screen

Many times, I `ssh` to my raspberry Pi and executed a long running program, but found the program was terminated before finish due to the `ssh` session timed out. With some research, I found the `screen` command tool provide a perfect solution to me.

`screen` is a terminal multiplexer. It means you can start a screen session and then open any number of virtual terminals inside that session. Processes running in `screen` will continue to run when their window is not visible even if you get disconnected.

## Install

```bash
sudo apt get install screen
```

## Usage

* Start a new session with session name: `screen -S <session_name>`
* List running sessions: `screen -ls`
* Attach to a running session: `screen -r <session_name>`

## Detach or Exit

* Detach a running session: `screen -d <session_name>`
* Detach: `Ctrl-a d`
* Detach and logout: `Ctrl-a D D`
* Exit screen: `Ctrl-a :`
* Force-exit screen: `Ctrl-a C-\`
