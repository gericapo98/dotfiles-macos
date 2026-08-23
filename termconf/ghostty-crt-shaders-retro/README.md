# ghostty-config

My [Ghostty](https://ghostty.org) rice — Rosé Pine-ish palette with a CRT/bloom shader stack.

## Install

```sh
git clone https://github.com/gericapo98/ghostty-config ~/.config/ghostty
```

or copy `config` and `shaders/` into `~/.config/ghostty/`.

## Shaders

The active stack is `bloom.glsl` + `bettercrt.glsl`. Swap or stack any of the
files in `shaders/` by editing the `custom-shader` lines in `config`.

| Shader | Effect |
| --- | --- |
| `bloom.glsl` | Soft glow around bright text |
| `bettercrt.glsl` | Subtle CRT scanlines/curvature |
| `crt.glsl` | Timothy Lottes' CRT-styled scaler |
| `retro-terminal.glsl` | Green-tinted retro CRT |
| `glow-rgbsplit-twitchy.glsl` | Glow + twitchy chromatic aberration |
| `vhs.glsl` | Degraded VHS tape look |

Shaders are collected from public sources; credits and licenses are in each
file's header.
