# Maintainer: David McInnis <davidm at eagles dot ewu dot edu>

pkgname=python-dicttoxml
pkgver=1.6.6
pkgrel=4
pkgdesc="Converts a Python dictionary or other native data type into a valid XML string."
url="https://github.com/quandyfactory/dicttoxml"
arch=('any')
license=('GPL2')
makedepends=('python-setuptools')
source=(https://pypi.python.org/packages/source/d/dicttoxml/dicttoxml-$pkgver.tar.gz)
sha256sums=('8229dcbadbe8a417b5e221b0bd56dff8a8ffd250951e6e95d51d5c5e2a77cc68')


package () {
  pkgdesc+=" (Python3.x)"
  depends=('python')

  cd $srcdir/dicttoxml-$pkgver
  python setup.py install --root="${pkgdir}" --optimize=1
  
  install -D README.markdown $pkgdir/usr/share/doc/$pkgname/README.md
  install -D LICENCE.txt $pkgdir/usr/share/licenses/$pkgname/LICENSE.txt
}
