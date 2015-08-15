# Maintainer:  TDY <tdy@archlinux.info>
# Contributor: Dmitry N. Shilov <stormblast@land.ru>

pkgname=divfixpp
pkgver=0.34
pkgrel=1
pkgdesc="A tool for repairing corrupted AVI file streams"
arch=('i686' 'x86_64')
url="http://divfixpp.sourceforge.net/"
license=('GPL')
depends=('wxgtk')
makedepends=('gettext')
source=(http://downloads.sourceforge.net/divfixpp/DivFix++_v$pkgver-src.tar.bz2)
md5sums=('a3809d7f325b10192c840c7fd5a1156e')

build() {
  cd "$srcdir/DivFix++_v$pkgver"
  make
}

package() {
  cd "$srcdir/DivFix++_v$pkgver"
  make DESTDIR="$pkgdir" install
  ln -sf DivFix++ "$pkgdir/usr/bin/divfixpp"
}

# vim:set ts=2 sw=2 et:
