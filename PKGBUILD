# Maintainer: Visudio Contributors <info@visudio.xyz>
pkgname=visudio
pkgver=1.0.8
pkgrel=1
pkgdesc='Audio-reactive ambient display perimeter glow for Linux'
arch=('x86_64')
url='https://visudio.xyz'
license=('LicenseRef-Proprietary')
depends=('alsa-lib' 'brotli' 'gcc-libs' 'glibc' 'libx11' 'openssl' 'pipewire' 'wayland' 'zlib' 'zstd')
optdepends=('libvulkan: Vulkan rendering support' 'vulkan-intel: Intel Vulkan backend' 'vulkan-radeon: AMD Vulkan backend')
options=('!strip')
source=("https://visudio.xyz/downloads/visudio-linux-x86_64")
sha256sums=('af5a347faf5264b7fc90fa7e8aafc4845adad00074ecf5e804de92040b3089bd')

package() {
  install -Dm755 "$srcdir/visudio-linux-x86_64" "$pkgdir/usr/bin/visudio"
  install -Dm644 "$startdir/assets/visudio.desktop" "$pkgdir/usr/share/applications/visudio.desktop"
  install -Dm644 "$startdir/assets/visudio.svg" "$pkgdir/usr/share/icons/hicolor/scalable/apps/visudio.svg"
  install -Dm644 "$startdir/LICENSE" "$pkgdir/usr/share/licenses/visudio/LICENSE"
}
