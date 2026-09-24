# Visudio AUR package

AUR package recipe for [Visudio](https://visudio.xyz), the audio-reactive ambient display visualizer.

Visudio is closed-source proprietary software. This repository contains only the AUR recipe and public package metadata—never the application source. The package downloads the official checksum-pinned Linux x64 binary from the project's release CDN rather than rebuilding source. No open-source licence is granted; see `LICENSE`.

## Install from the AUR

Once published to the official AUR:

```bash
yay -S visudio
```

## Build locally

```bash
git clone https://github.com/xonix97/visudio-aur.git
cd visudio-aur
makepkg -si
```

The pinned SHA-256 in `PKGBUILD` is the trust boundary. Update `pkgver`, `pkgrel`, the download URL, and the checksum together for each release.
