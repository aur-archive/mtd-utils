# Contributor: Phil Pirozhkov <pirjsuka@gmail.com>
# Maintainer: Phil Pirozhkov <pirjsuka@gmail.com>
pkgname=mtd-utils
pkgver=1.5.0
pkgrel=2
pkgdesc="The mtd-utils package contains utilities related to handling MTD devices, and for dealing with FTL, NFTL JFFS2 etc."
arch=('i686' 'x86_64')
depends=('lzo2' 'util-linux')
url="http://www.linux-mtd.infradead.org/"
license=('GPLv2+')
md5sums=('7332f1143be4ba8ee2de3096cbd3b03b')
source=(ftp://ftp.infradead.org/pub/mtd-utils/${pkgname}-${pkgver}.tar.bz2)

build() {
  cd "$srcdir/$pkgname-$pkgver"

  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  make DESTDIR="$pkgdir/" install
}

# vim:set ts=2 sw=2 et:
