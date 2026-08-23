# kitty-config

My [kitty](https://sw.kovidgoyal.net/kitty/) setup — Catppuccin Mocha theme,
JetBrains Mono Nerd Font, a beam cursor with trail, and a couple of custom
kittens for search and scroll marks.

## Install

```sh
git clone https://github.com/gericapo98/dotfiles-macos ~/repos/dotfiles-macos
ln -s ~/repos/dotfiles-macos/termconf/kitty-config/kitty.conf ~/.config/kitty/kitty.conf
ln -s ~/repos/dotfiles-macos/termconf/kitty-config/kitty-theme.conf ~/.config/kitty/kitty-theme.conf
ln -s ~/repos/dotfiles-macos/termconf/kitty-config/scroll_mark.py ~/.config/kitty/scroll_mark.py
ln -s ~/repos/dotfiles-macos/termconf/kitty-config/search.py ~/.config/kitty/search.py
```

or just copy the files into `~/.config/kitty/`.

## Contents

| File | Purpose |
| --- | --- |
| `kitty.conf` | Main config — font, cursor, padding, keybinds |
| `kitty-theme.conf` | Catppuccin Mocha color scheme |
| `search.py` | Kitten: in-terminal search (bound to `ctrl+f`) |
| `scroll_mark.py` | Kitten: scrollback marks |

`kitty-theme.conf` is Catppuccin's official Mocha theme for kitty (MIT,
[upstream](https://github.com/catppuccin/kitty/blob/main/themes/mocha.conf)).
