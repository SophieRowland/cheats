# How to use tmux
#### Source `https://hackernoon.com/a-gentle-introduction-to-tmux-8d784c404340`

## Cheat sheet
### Start new named session:
`$ tmux new -s [session name]`

### Detach from session:
`ctrl+b d`

### List sessions:
`$ tmux ls`

### Attach to named session:
`$ tmux a -t [name of session]`

### Kill named session:
`$ tmux kill-session -t [name of session]`

### Split panes horizontally:
`ctrl+b "`

### Split panes vertically:
`ctrl+b %`

### Kill current pane:
`ctrl+b x`

### Move to another pane:
`ctrl+b [arrow key]`

### Cycle through panes:
`ctrl+b o`

### Cycle just between previous and current pane:
`ctrl+b ;`

### Kill tmux server, along with all sessions:
`$ tmux kill-server`


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
