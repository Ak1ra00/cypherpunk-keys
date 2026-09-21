# cypherpunk-keys

A searchable Hyprland keybinding reference for [Omarchy](https://omarchy.org/), styled after the Cypherpunk theme.

Omarchy is keyboard-driven by design — nearly everything (launching apps, managing windows, switching workspaces) happens through key combinations rather than clicking through menus. This page collects every binding from a real, working Omarchy setup into one searchable, filterable list, so it's easy to find "what key does X" without digging through config files.

## Screenshots

![Overview — header, search, and the Essentials/Windows/Workspaces/Groups/Notifications sections](screenshots/overview.png)

![System & Hardware and Apps & Web sections](screenshots/system-and-apps.png)

### Desktop theme

The keybindings above come from an Omarchy setup running a custom theme called [Oracle](https://github.com/Ak1ra00/oracle) — a full Omarchy theme built around the maths behind [vaultless](https://github.com/Ak1ra00/vaultless): a cyan/violet/amber palette on charcoal, gradient window borders with a soft cyan glow, a themed shell (bar, menus, notifications, lock screen), btop, and six 4K backgrounds that are rendered from the actual elliptic-curve and OPRF constructions rather than downloaded.

![Oracle theme on the desktop — btop, Neovim and fastfetch in the theme's colours](screenshots/theme-desktop.png)

![Oracle wallpaper 01 — the group law on y² = x³ − 3x + 5, plotted on a blueprint grid](screenshots/theme-wallpaper.png)

![Oracle wallpaper 04 — a paper oracle sheet with a real VLT1 QR code](screenshots/theme-paper-oracle.png)

![Top bar showing the Oracle theme's accent colours](screenshots/theme-bar.png)

## What's in it

- **230+ keybindings**, pulled directly from `omarchy menu keybindings --print`
- Grouped into categories: Essentials, Windows & Layout, Workspaces, Window Groups, Notifications, System & Hardware, Apps & Web, Media Keys
- Live search box and category toggles to narrow the list down
- No build step, no dependencies — a single static `index.html`

## Viewing it

Live at: **https://ak1ra00.github.io/cypherpunk-keys/**

Or just open `index.html` directly in a browser.

## Updating

The bindings are stored as a plain JavaScript array inside `index.html`. To refresh them from a live Omarchy machine:

```bash
omarchy menu keybindings --print
```

Then edit the `DATA` array in `index.html` to match.
