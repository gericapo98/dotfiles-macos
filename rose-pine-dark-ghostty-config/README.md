# ghostty-config (rose-pine-dark)

My [Ghostty](https://ghostty.org) rice — Rosé Pine-ish palette lifted from
[vereis/blog_old](https://github.com/vereis/blog_old)'s theme, with the
background swapped to Rosé Pine's own dark base (`#191724`) instead of the
blog's near-black — same depth, but it stays in-family with the palette's
pinks/golds/purples instead of clashing like the earlier navy blue did.
Everything else (foreground, palette, selection, cursor, font) is unchanged
from the base rice.

## Install

```sh
cp config and shaders/ into ~/.config/ghostty/
```

## Shaders

The active stack is `vhs.glsl` — a self-contained pipeline (curve, scanline
tracking wobble, tape-wear grain, chroma bleed, vignette, static flecks),
swapped in for the grain/texture look on
[vereis.com](https://vereis.com)'s hand-painted theme. `bloom.glsl` composes
safely on top of it (purely additive, no curve/vignette of its own) if you
want extra glow — uncomment its `custom-shader` line in `config`. Don't stack
`vhs.glsl` with `bettercrt.glsl` or `crt.glsl`: both of those apply their own
barrel curve, and two curve passes compound into a warped mess.

Swap or stack any of the files in `shaders/` by editing the `custom-shader`
lines in `config`.

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
