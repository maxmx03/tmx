# tmx

## Installation

```bash
echo "source $HOME/path/to/tmx.sh" >> $HOME/.bashrc
```

## Usage

```bash
tmx save # save sessions
tmx restore # restore all sessions
tmx attach # attach session
tmx list # list saved sessions ~/.cache/tmux-session
tmx new # create new session
```

## Dependencies

- [gum](https://github.com/charmbracelet/gum)

```bash
# golang
# $HOME/go/bin
go install github.com/charmbracelet/gum@latest

# btw
pacman -S gum

# macos
brew install gum
```
