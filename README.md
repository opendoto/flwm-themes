# flwm-themes

Color themes for FLWM, FLTK, and Aterm.

Tiny Core Linux has always focused on being small and fast. The desktop works well, but the default colors and widget styles feel old and sometimes hard to read.

This repository exists to improve that.

Each theme is a plain **.Xdefaults** file. No patches, no extra software, no background processes. Just copy a file and restart your session.

The goal is simple: better colors, better contrast, and a cleaner desktop while keeping the same lightweight system.

## Themes

### Dark

* 🟠 **Amber CRT** — Orange-on-black colors inspired by classic amber CRT monitors.
* 🌿 **Catppuccin Mocha** — Soft pastel colors.
* 🌸 **Cherry Blossom Dark** — Soft pink accents on a dark background.
* 🦇 **Dracula** — Dark purple with bright accents.
* 🌲 **Everforest Dark** — Soft green forest colors with a calm, natural look.
* 🪵 **Gruvbox Dark** — Warm retro colors.
* 💚 **Matrix** — Green-on-black colors inspired by the classic hacker terminal look.
* 🌌 **Midnight Blue** — Deep blue colors for a calm nighttime desktop.
* ⚫ **Monochrome** — Black, white, and gray for a clean minimalist desktop.
* ❄️ **Nord Dark** — Cool blue and gray tones.
* 🌹 **Red Rose Noir** — Deep black and crimson colors with a dark elegant look.
* 🌺 **Rosé Pine Moon** — Soft dark colors with warm accents.
* 🌈 **Synthwave** — Neon purple and pink colors inspired by the 80s retro aesthetic.
* 🌃 **Tokyo Night** — Bright blues inspired by city lights.

### Light

* 🖥️ **CDE** — Classic UNIX look.
* 🌸 **Cherry Blossom Light** — Soft pink and cream colors.
* 🌲 **Everforest Light** — Soft natural colors with warm green accents.
* 🌾 **Gruvbox Light** — Warm paper-like colors.
* 🌄 **Hachimi Landscape** — Warm countryside colors inspired by open fields and clear skies.
* 💜 **Kimi Light** — Soft lavender and light purple colors with a clean, bright look.
* 🍦 **Maycream** — Soft cream colors for reading.
* 🟠 **Old Ubuntu** — Inspired by the old Ubuntu Human theme.
* 🌅 **Rosé Pine Dawn** — Light pastel colors.
* 🌤️ **Skyline** — Bright blue sky colors with a clean light look.

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
│   ├── amber-crt
│   ├── catppuccin-mocha
│   ├── cherry-blossom-dark
│   ├── dracula
│   ├── everforest-dark
│   ├── gruvbox-dark
│   ├── matrix
│   ├── midnight-blue
│   ├── monochrome
│   ├── nord-dark
│   ├── red-rose-noir
│   ├── rose-pine-moon
│   ├── synthwave
│   └── tokyo-night
└── light/
    ├── cde
    ├── cherry-blossom-light
    ├── everforest-light
    ├── gruvbox-light
    ├── hachimi-landscape
    ├── kimi-light
    ├── maycream
    ├── oldubuntu
    ├── rose-pine-dawn
    └── skyline
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
