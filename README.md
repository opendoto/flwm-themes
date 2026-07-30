# flwm-themes

Color themes for FLWM, FLTK, and Aterm.

Tiny Core Linux has always focused on being small and fast. The desktop works well, but the default colors and widget styles feel old and sometimes hard to read.

This repository exists to improve that.

Each theme is a plain **.Xdefaults** file. No patches, no extra software, no background processes. Just copy a file and restart your session.

The goal is simple: better colors, better contrast, and a cleaner desktop while keeping the same lightweight system.

## Themes

### Dark

* 🌿 **Catppuccin Mocha** — Soft pastel colors.
* 🦇 **Dracula** — Dark purple with bright accents.
* 🪵 **Gruvbox Dark** — Warm retro colors.
* 💚 **Matrix** — Green-on-black colors inspired by the classic hacker terminal look.
* ❄️ **Nord Dark** — Cool blue and gray tones.
* 🌹 **Rosé Pine Moon** — Soft dark colors with warm accents.
* 🌃 **Tokyo Night** — Bright blues inspired by city lights.

### Light

* 🖥️ **CDE** — Classic UNIX look.
* 🌾 **Gruvbox Light** — Warm paper-like colors.
* 🍦 **Maycream** — Soft cream colors for reading.
* 🟠 **Old Ubuntu** — Inspired by the old Ubuntu Human theme.
* 🌅 **Rosé Pine Dawn** — Light pastel colors.

## Features

* Made for FLWM desktops.
* Better colors for FLTK applications.
* Full 16-color ANSI palette for Aterm.
* Good text contrast.
* No extra dependencies.
* No runtime overhead.
* Plain `.Xdefaults` files.

## Requirements

* These themes use **`~/.Xdefaults`**.
* They should work on any FLWM desktop that uses the same setup, but they have only been tested on **FLinux**.

## Installation

Clone the repository:

```bash
git clone https://github.com/opendoto/flwm-themes.git
cd flwm-themes
```

### Before You Start

It is recommended to backup your current **`.Xdefaults`** file before applying a new theme.

```bash
cp ~/.Xdefaults ~/.Xdefaults.bak
```

## Applying a Theme

Copy the theme you want to **`~/.Xdefaults`**.

Example:

```bash
cp dark/nord-dark ~/.Xdefaults
```

or

```bash
cp light/maycream ~/.Xdefaults
```

Restart FLWM, or simply log out and start a new X session.

The new theme will be used by:

* FLWM
* FLTK applications
* Aterm

## Repository Layout

```text
flwm-themes/
├── dark/
│   ├── catppuccin-mocha
│   ├── dracula
│   ├── gruvbox-dark
│   ├── matrix
│   ├── nord-dark
│   ├── rose-pine-moon
│   └── tokyo-night
└── light/
    ├── cde
    ├── gruvbox-light
    ├── maycream
    ├── oldubuntu
    └── rose-pine-dawn
```

## Keep in Mind

* **Compiled FLWM limits:** Some window borders, titlebars, or colors may look different depending on how your distribution compiled `flwm`. Some builds hardcode parts of the interface.
* **FLWM and FLTK limits:** FLWM and FLTK are very small projects. They were made to be fast and lightweight, not to support advanced desktop theming. Because of that, some themes needed small adjustments to keep good contrast, readable text, and visible buttons.
* **Live systems:** If you are running Tiny Core Linux or FLinux in a live session, remember to run:

```bash
filetool.sh -b
```

before shutting down, otherwise your changes may not be saved.

The goal is to stay as close as possible to the original themes while making them work well on this desktop.

## Why?

Because changing a desktop theme should not require another toolkit, another daemon, another compositor, or another configuration system.

One `.Xdefaults` file is enough.

## Notes

* These themes were made for FLWM desktops.
* They have only been tested on **FLinux**, but they should also work on Tiny Core Linux systems that use **`~/.Xdefaults`**.
* If an FLTK application ignores `.Xdefaults` and uses its own colors, there is nothing this repository can do about it.

## License

MIT License. See `LICENSE` for details.
