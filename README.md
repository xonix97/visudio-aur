# Visudio AUR package

AUR package recipe for [Visudio](https://visudio.xyz), the audio-reactive ambient display visualizer.

Visudio is proprietary software, so the package downloads the official signed-by-checksum Linux x64 binary from the project's release CDN rather than rebuilding source.

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
