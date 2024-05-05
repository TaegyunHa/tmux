# TMUX

## Installation

```
brew install tmux
brew install tmuxinator
git clone https://github.com/tmux-plugins/tpm.git ~/.config/tmux/plugins/tpm
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

1. New Session
    ```
    tmux new -s <sessionName>
    ```
2. Attach Session
   ```
   tmux attach -t <sessionName>
   ```
3. Detach Session
   ```
   tmux detach
   ```
4. Close window
   ```
   exit
   ```

### Prefix operations

1. tmux Command
   ```
   <prefix> : <command>
   ```
2. List Sessions
   ```
   <prefix> s
   ```
3. Split Window Horizontally
   ```
   <prefix> %
   <prefix> |
   ```
4. Split Window Vertically
   ```
   <prefix> "
   <prefix> -
   ```
5. Resize Window
   ```
   <prefix> [h,j,k,l]
   ```

### vim-tmux-navigator

1. Move window
    ```
    <Cntr> [h,j,k,l]
    ```
