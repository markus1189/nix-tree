# nix-tree

![Build Status](https://github.com/utdemir/nix-tree/workflows/nix-build/badge.svg)
[![Packaging status](https://repology.org/badge/vertical-allrepos/haskell:nix-tree.svg)](https://repology.org/project/haskell:nix-tree/versions)

Interactively browse the dependency graph of your Nix derivations.

[![asciicast](https://asciinema.org/a/ahDveBL1gs5t36z1myePtrKpR.svg)](https://asciinema.org/a/ahDveBL1gs5t36z1myePtrKpR)

## Installation

Stable version:

```
nix-env -i nix-tree
```

Development version (requires Nix with flake support):

```
nix profile install github:utdemir/nix-tree
```

## Usage

```
$ nix-tree --help
nix-tree --help
Usage: nix-tree [paths] [-h|--help]
  Paths default to $HOME/.nix-profile and /var/run/current-system.
Keybindings:
  hjkl/Arrow Keys : Navigate
  q/Esc:          : Quit / close modal
  w               : Open why-depends mode
  /               : Open search mode
  i               : Toggle modeline
  ?               : Show help
```

[home-manager]: https://github.com/rycee/home-manager

## Hacking

All contributions, issues and feature requests are welcome.

To hack on it, simply run `nix-shell` (or `nix develop`) and use `cabal` as usual.

# Related tools

* [nix-du](https://github.com/symphorien/nix-du)
* [nix-query-tree-viewer](https://github.com/cdepillabout/nix-query-tree-viewer)
* [nix-visualize](https://github.com/craigmbooth/nix-visualize)
