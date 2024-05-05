# TMUX

## Installation

```
brew install tmux
brew install tmuxinator
git clone --recursive https://github.com/TaegyunHa/tmux.git ~/.config/tmux
```

## Directory Tree

```
~/.config/
|- tmux
  |- tmux.conf
  |- plugins
    |- tpm
```

## Config

### Symlink Config File

```
ln -s ~/.config/tmux/tmux.conf ~/.tmux.conf
```

### Source Config (Optional)

```
tmux source-file ~/.config/tmux/tmux.conf
```

### Install plugins

```
<prefix> <Shift-I>
```

<br/>

# Basic Oprations

### Terminal Operations

Command                       | Description
------------------------------|------------
`tmux new -s <sessionName>`   | New Session
`tmux attach -t <sessionName>`| Attach Session
`tmux detach`                 | Detach Session
`exit`                        | Close window


### Prefix operations

Key bind              | Description
----------------------|------------
`<prefix> : <command>`| Inline command
`<prefix> s`          | List all Sessions
`<prefix> w`          | List all Windows
`<prefix> c`          | Create Window
`<prefix> [1,2,3..]`  | Select Window
`<prefix> n`          | Next Window
`<prefix> p`          | Previous Window
`<prefix> \|`         | Split Window Horizontally
`<prefix> -`          | Split Window Vertically
`<prefix> ,`          | Rename Window
`<prefix> [h,j,k,l]`  | Resize Pane
`<prefix> [`          | Copy mode (`ctrl-c` to finish)


### vim-tmux-navigator

Key bind              | Description
----------------------|------------
`<Cntr> [h,j,k,l]`    | Move Pane Focus

