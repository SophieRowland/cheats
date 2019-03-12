# How to use tmux
#### Source `https://hackernoon.com/a-gentle-introduction-to-tmux-8d784c404340`

## Install
```sh
$ brew install tmux
$ tmux -V
```

## Getting started

- `ctrl+b` prefix needed to run tmux command
  - `:` after prefix to get a tmux prompt at the bottom of the screen
- `ctrl+b d` "detach", better way to get out
    - keeps session running

```sh
# New window
$ tmux new

# Labeled new window
$ tmux new -s [name of session]

# End session (vs detach keeps session running)
$ exit

# Check what sessions are running
$ tmux ls

# Re-enter a session (ex: session # = 3)
$ tmux attach-session -t 3
# Last created session (a = attach-session)
$ tmux a #
# Labeled session
$ tmux a -t [name of session]
```

## Working with panes

### Managing panes

- `ctrl+b "` split horizontally
- `ctrl+b %` split vertically
- `ctrl+b [arrow key]` move around panes
- You can split panes multiple times

### Resizing panes

- Open prompt (`ctrl+b :`)
- `resize-pane -U #`
  - `-U` up
  - `-D` down
  - `-L` left
  - `-R` right
  - # of lines to expand

## Customizing themes
#### Some default themes `https://github.com/jimeh/tmux-themepack`
