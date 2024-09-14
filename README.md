# tmx

## Installation

```bash
echo "source $HOME/path/to/tmx.sh" >> $HOME/.bashrc
```

## Usage

```bash
tmx attach # attach session
tmx new session-name # create new session
tmx newx config.json # create a more complex session
tmx rm # remove session
tmx help
```

### newx example

```json
{
  "sessions": [
    {
      "name": "solarized",
      "root": "~/github/solarized.nvim",
      "windows": [
        "nvim",
        "docker compose up",
        "styla -f ./stylua.toml ."
      ]
    },
    {
      "name": "docs",
      "root": "~/github/milianor-docs",
      "windows": [
        "nvim",
        "pnpm start"
      ]
    }
  ]
}
```

## Dependencies

- [jq](https://jqlang.github.io/jq/)

```bash
pacman -S jq
```

## Alternatives

- [tmuxinator](https://github.com/tmuxinator/tmuxinator)
- [tmuxp](https://github.com/tmux-python/tmuxp)
