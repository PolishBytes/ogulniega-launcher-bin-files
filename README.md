# Ogulniega Launcher for Arch Linux

> [!IMPORTANT]
> This repository is **not affiliated with Ogulniega or its author**.

This repository contains the files required to run the Ogulniega Minecraft Launcher natively on Arch Linux.

The included `PKGBUILD` is a temporary solution until the package can be published to the AUR. It can be used to build and install the launcher manually with `makepkg`.

## Installation

Clone the repository:

```bash
git clone https://github.com/PolishBytes/ogulniega-launcher-bin-files
cd ogulniega-launcher-bin-files
```

Build and install the package:

```bash
makepkg -si
```

That's it. The launcher should now be available as `ogulniega` and appear in your application menu.

## Updating

To get the latest packaged launcher files:

```bash
git pull
makepkg -si
```

## Disclaimer

Ogulniega Launcher is proprietary software. This repository is an unofficial community packaging effort and is not endorsed by or associated with the original developer.
