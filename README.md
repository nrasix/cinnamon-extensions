# Cinnamon Extensions for Cinnamon 5.6

**English** | [Русский](README_RU.md)

This repository contains adapted versions of two **Cinnamon** desktop
extensions, prepared to work on **Cinnamon 5.6.x** — the version shipped with
Linux Mint 21.1 and other distributions that use this Cinnamon release.

These are not the original extensions but patched builds: they keep the
functionality of the originals while being adapted to the APIs and behavior of
Cinnamon 5.6. The original projects and their authors are listed below.

## Who this repository is for

- Users of **Linux Mint 21.1** (and other systems with **Cinnamon 5.6**) who
  don't want to or can't upgrade their desktop to a newer release.
- People who want a **modern dock** and **rounded window corners** with custom
  borders and shadows, but whose Cinnamon version is not supported by the
  current releases of these extensions.
- Users who install extensions manually or distribute them through the spices
  repository.

> If you are running Cinnamon 5.8 or newer, the original versions maintained by
> their authors are probably a better choice.

## Extensions

### Mint-Dock

**What it is:** a native, customizable dock for Cinnamon.

**Why use it:** it replaces the default taskbar with a convenient macOS/Plank
style dock and offers extensive customization:

- customizable background color and appearance;
- reorder icons and drag and drop apps from the Cinnamon menu directly to the dock;
- choose the dock position (top, bottom, left, right, start, center or end);
- two hiding modes: smart hiding (Intellihide) and automatic hiding;
- tooltips, separators, trash and other configurable elements;
- notification badges and application progress bars;
- compatible with both X11 and Wayland.

**Who it's for:** users who find the default Cinnamon panel insufficient and
want a customizable dock.

**Original author:** [hilyxx](https://github.com/Hilyxx).

### Rounded Corners

**What it is:** an extension that rounds window corners and adds customizable
borders and shadows.

**Why use it:** it helps bring window appearance to a consistent style and tune
it to your liking:

- round the top and bottom corners of application windows;
- custom borders and shadows for windows with rounded corners;
- exclude specific applications from rounding;
- per-application border settings;
- different borders and shadow strength for the focused and unfocused windows;
- a mode where the rounded border matches the window's natural border;
- support for Gtk3, libhandy, Gtk4, Adwaita and Qt windows.

**Who it's for:** users who want to round the bottom corners of windows,
increase their theme's corner radius, customize borders and shadows, or make
the desktop look cleaner and more consistent.

**Original author:** [klangman](https://github.com/klangman/CinnamonRoundedCorners).

## Compatibility

| Extension       | Target Cinnamon version | License |
| --------------- | ----------------------- | ------- |
| Mint-Dock       | 5.6.x                   | GPL-3.0 |
| Rounded Corners | 5.6.x                   | GPL-3.0 |

## Installation

1. Copy the extension directory from `files/` into the Cinnamon extensions
   directory:

   ```bash
   mkdir -p ~/.local/share/cinnamon/extensions
   cp -r "mint-dock-5.6@hilyxx&nrasix/files/mint-dock@hilyxx" \
         ~/.local/share/cinnamon/extensions/
   cp -r "RoundedCorners-5.6@klangman&nrasix/files/RoundedCorners@klangman" \
         ~/.local/share/cinnamon/extensions/
   ```

2. Restart Cinnamon (for example, press `Alt+F2`, type `r` and hit `Enter`).
3. Open **System Settings → Extensions**, enable the extension you need and
   configure it using the gear icon.

## Authors

- **Mint-Dock**
  - original author: **hilyxx**;
  - Cinnamon 5.6 adaptation and maintenance: **nrasix**.
- **Rounded Corners**
  - original author: **klangman** (Kevin Langman);
  - Cinnamon 5.6 adaptation and maintenance: **nrasix**.

This project is distributed under the **GPL-3.0** license. All rights to the
original extensions belong to their respective authors.
