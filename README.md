# morvane-awesome-theme

The MorvaneOS theme for awesome: awesome's default theme with the MorvaneOS colours
(a Pastel Pink border on the focused window and on the current tag) and the
Twilight wallpaper. Everything else, icons and sizes, stays awesome's.

Installs `/usr/share/awesome/themes/morvane/theme.lua`. The MorvaneOS installer
points awesome's `rc.lua` at it. In your own `rc.lua`, use:

```lua
beautiful.init(gears.filesystem.get_themes_dir() .. "morvane/theme.lua")
```

Terminal colours (xterm, alacritty) come from
[morvane-wm-theme](https://github.com/MorvaneOS/morvane-wm-theme), apps from
[morvane-gtk-theme](https://github.com/MorvaneOS/morvane-gtk-theme).

## Changing it

Edit `tools/build.py`, then:

```
python tools/build.py
```

Needs only Python. Commit the output, bump `pkgver`, build and publish.

## License

LGPL-2.1-or-later.
