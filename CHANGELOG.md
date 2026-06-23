# Changelog

## 2026.06.23 — README install commands

### What Changed

**Install docs:** the README install section now lists the meta packages (top-level `*-icons-meta`, plus the group meta where applicable) alongside the per-variant `*-icons-git` package — replacing the outdated single `pacman -S` line.

### Files Modified

- README.md

## 2026.06.21 — repo standardisation

### What Changed

Replaced the obsolete legacy git script with the standard `setup.sh`/`up.sh`, added the
standard project docs, and corrected the README's dependency note.

### Technical Details

- Removed the old `git-v1.sh`/`setup-git-v5.sh` and added the canonical `setup.sh` and
  `up.sh` (matching the other surfn theme repos).
- README dependency note corrected: ships only `Surfn-Plasma-Light`, which
  `Inherits=Surfn-Plasma-Dark,breeze,hicolor`. The theme needs `surfn-plasma-dark-icons-git`
  at runtime, but the recipe has `depends=()` — known gap.
- Added CLAUDE.md.

### Files Modified

- README.md, CHANGELOG.md, CLAUDE.md
