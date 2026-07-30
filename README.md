# MatsyaOS Package Repository

This repository hosts compiled MatsyaOS packages used by the live ISO and installed systems.

## Usage

Add to `/etc/pacman.conf`:

```
[matsyaos]
SigLevel = Optional TrustAll
Server = https://raw.githubusercontent.com/MatsyaOs/matsyaos-repo/main/x86_64
```

Then:

```
sudo pacman -Syu
```

## Layout

```
x86_64/
  *.pkg.tar.zst
  matsyaos.db
  matsyaos.db.tar.gz
  matsyaos.files
  matsyaos.files.tar.gz
```

Packages are built from https://github.com/MatsyaOs/MatsyaOS and versioned from each component PKGBUILD (release line 1.1+).
