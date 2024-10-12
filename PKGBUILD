# Maintainer: rarick <tyler dot rarick at gmail dot com>

pkgname=btrbk-snapshot
pkgver=1.0
pkgrel=1
pkgdesc="Automated Btrbk snapshot service and timer"
arch=('any')
license=('MIT')
depends=('btrbk')
makedepends=()
source=(
  'btrbk-snapshot.service'
  'btrbk-snapshot.timer'
)
sha256sums=('SKIP' 'SKIP')

package() {
  # Install systemd service and timer
  install -Dm644 "$srcdir/btrbk-snapshot.service" "$pkgdir/usr/lib/systemd/system/btrbk-snapshot.service"
  install -Dm644 "$srcdir/btrbk-snapshot.timer" "$pkgdir/usr/lib/systemd/system/btrbk-snapshot.timer"
}
