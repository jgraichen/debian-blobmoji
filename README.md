# Blobmoji

Minimal debian package for [Blobmoji](https://github.com/C1710/blobmoji) font and a font-config that prefers blobmoji over other other emoji fonts.

## Usage

```bash
dpkg-buildpackage
sudo apt install ../fonts-blobmoji*.deb
```

## Doing a release with updated upstream

```bash
wget -O Blobmoji.ttf https://github.com/C1710/blobmoji/releases/download/v14.0.1/Blobmoji.ttf

# add info about new version to debian/changelog via $EDITOR
dch -i

# set new version to "released" in debian/changelog via $EDITOR (and save!)
dch -r
```
