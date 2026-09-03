# Slate Signal Night

A dark Omarchy theme for people who read a lot of text on a small screen. Grey chassis lifted off black, one blue that means something, and a text selection you can actually see. This is the night half of a pair. The day half is [Slate Signal Day](https://github.com/vitalibondar/omarchy-slate-signal-day-theme).

## Why it looks like this

I work on a 14" 1920x1080 ThinkPad, I am short-sighted, and I read a lot of small text up close. Pure black on that panel makes the bottom of the ramp unreliable, and bright status colours glow in a dark room. So the ground is off-black (`#15171a`), body text is capped below pure white at 12.7:1, and the status colours are about 15% less saturated than in the day theme. The blue (`#82b4ea`) is the only colour that carries meaning: links, the accent, the border of the focused window.

Selection is a plain fill (`#455566`). But no terminal or editor that Omarchy themes exposes a selection edge, so the region is carried by the fill alone and the selected text is drawn in the brightest foreground. That lands at 6.9:1, a hair under the 7:1 I aimed for, and I think that is the right trade: a darker band would be less visible as a region, a lighter one would eat the text.

## Install

```sh
omarchy theme install https://github.com/vitalibondar/omarchy-slate-signal-night-theme.git
```

Two wallpapers ship with the theme. And they are part of it, not an afterthought: `01` is a damask tile for everyday use, so any gap between tiled windows lands on full detail. `02` is a bouquet with more empty space, better for the lock screen or as a change. `omarchy theme bg next` cycles between them.

## The pair

Day and Night use the same hues with the lightness order reversed. If you switch them by sunrise and sunset, keep the geometry (font size, window border, corner rounding) in a machine-level file rather than in the theme, so nothing jumps when the theme changes. Those files, the contrast checker and the design notes live in [slate-signal](https://github.com/vitalibondar/slate-signal).

## Numbers

Measured on the hex values with the checker from the slate-signal repo, WCAG 2.x.

| Pair | Ratio |
|---|---|
| body text / background | 12.7 |
| emphasis / background | 16.3 |
| muted text / background | 5.8 |
| accent / background | 8.3 |
| selected text / selection | 6.9 |
| selection / background | 2.35 (intentional, see above) |

## Status

New. It went onto my own machine on 3 September 2026, and previews will follow once I have lived with it for a bit. If something reads badly on your screen, open an issue and say which screen.

## Credits

The brief and every prompt came from ChatGPT (GPT-5.6). Claude Design executed them into the palette, checked against Omarchy 4.0.2 templates, and Claude Code did the install. The wallpapers were generated with ChatGPT as well. MIT, wallpapers included.
