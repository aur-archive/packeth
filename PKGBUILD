# Maintainer: Rudy Matela <rudy.matela@gmail.com>
pkgname=packeth
pkgver=1.7.1
pkgrel=1
pkgdesc="A Linux GUI packet generator tool for ethernet."
depends=(gtk2)
source=("http://downloads.sourceforge.net/packeth/packETH-$pkgver.tar.bz2")
url="http://packeth.sourceforge.net/"
md5sums=('38403ec01072f13ba7f0145abf15b12d')
arch=('i686' 'x86_64')
license=('GPL')

build() {
  cd $srcdir/packETH-1.7
  ./configure --prefix=/usr
  /usr/bin/make
}

package() {
  cd $srcdir/packETH-1.7
  /usr/bin/make install DESTDIR=$pkgdir
}
