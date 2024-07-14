pkgname=pacman-aliases
pkgver=1.0
pkgrel=1
pkgdesc="Custom Pacman Aliases script for Arch Linux"
arch=('any')
license=('MIT')
source=('pacman-aliases')
sha256sums=('SKIP')
depends=('nano')

package() {
    install -Dm755 "$srcdir/pacman-aliases" "$pkgdir/usr/local/bin/pacman"
}