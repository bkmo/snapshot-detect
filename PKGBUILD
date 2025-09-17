# bkmo original

pkgname=snapshot-detect
pkgver=1.0
pkgrel=1
pkgdesc="Notify when booted into btrfs snapshot"
arch=('any')
url="https://github.com/bkmo/snapshot-detect"
license=('GPL3')
depends=('btrfs-progs')
optdepends=('snapper: For snapper support')
makedepends=('git')
provides=('snapshot-detect')
source=($url/archive/refs/tags/$pkgver.tar.gz)
md5sums=('SKIP')

package() {
 cd $pkgname-$pkgver
 install -Dm755 snapshot-detect -t "$pkgdir/usr/bin/"
 install -Dm644 snapshot-detect.desktop -t "$pkgdir/etc/xdg/autostart/"
}
