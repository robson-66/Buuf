pkgname=buuf
pkgver=1.0
pkgrel=1
pkgdesc="Based on Mattahan's artwork in devianart cc-by-nc-sa 2.5"
arch=('any')
url="https://git.disroot.org/eudaimon/buuf-nestort"
license=('GPL')
source=("Buuf.tar.gz")
sha256sums=('SKIP')

package() {
  install -d -m755 $pkgdir/usr/share/icons

  cd $srcdir
  mv Buuf $pkgdir/usr/share/icons/
  
  find $pkgdir/usr -type f -exec chmod 644 {} \;
  find $pkgdir/usr -type d -exec chmod 755 {} \;
  find $pkgdir/usr -type f -name '.directory' -delete
}
