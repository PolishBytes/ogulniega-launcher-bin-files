# Ogulniega Launcher for Arch Linux

> [!IMPORTANT]
> This repository is **not affiliated with Ogulniega or its author**.

This repository contains the files required to run the Ogulniega Minecraft Launcher natively on Arch Linux.

The included `PKGBUILD` is a temporary solution until the package can be published to the AUR. It can be used to build and install the launcher manually with `makepkg`.

## Installation

Create a directory and download only the `PKGBUILD`:

```bash
mkdir ogulniega
cd ogulniega
curl -O https://raw.githubusercontent.com/PolishBytes/ogulniega-launcher-bin-files/main/PKGBUILD
```

Then build and install the package:

```bash
makepkg -si
```

### Or do everything in one command

```bash
mkdir -p ogulniega && cd ogulniega && curl -O https://raw.githubusercontent.com/PolishBytes/ogulniega-launcher-bin-files/main/PKGBUILD && makepkg -si
```

That's it. The launcher should now be available as `ogulniega` and appear in your application menu.

## Updating

To update the package, download the latest `PKGBUILD` and rebuild it:

```bash
cd ogulniega
curl -O https://raw.githubusercontent.com/PolishBytes/ogulniega-launcher-bin-files/main/PKGBUILD
makepkg -si
```

## Disclaimer

Ogulniega Launcher is proprietary software. This repository is an unofficial community packaging effort and is not endorsed by or associated with the original developer.
