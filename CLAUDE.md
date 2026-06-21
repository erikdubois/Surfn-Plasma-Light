# CLAUDE.md — surfn-plasma-light

## Project overview

Standalone repo for the **Surfn Plasma Light** icon theme, split out of the
`erikdubois/surfn` monolith. See [README.md](./README.md).

## Current state

Ships one theme: `usr/share/icons/Surfn-Plasma-Light/`. Packaged as
`surfn-plasma-light-icons-git` (recipe in `~/KIRO-PKG-BUILD-ICONS/surfn-plasma-light/`).

## Patterns & decisions

- Theme dir PascalCase; repo/package lowercase. `icon-theme.cache` rebuilt by the pacman
  hook on install. Theme `Inherits=Surfn-Plasma-Dark,breeze,hicolor`, so it needs
  `surfn-plasma-dark-icons-git` at runtime — but the recipe has `depends=()` (known gap).
  Bash scripts follow the canonical Kiro template.
