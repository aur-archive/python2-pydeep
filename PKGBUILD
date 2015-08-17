# Maintainer: Justin Capella

pkgname=python2-pydeep
pkgver=0.2
pkgrel=1
pkgdesc="This is the Python interface to ssdeep."
arch=(any)
url=(http://pypi.python.org/pypi/python-pydeep/)
license=(PSF)
depends=(python2 ssdeep)
makedepends=(python2-distribute)
source=(http://pypi.python.org/packages/source/p/pydeep/pydeep-$pkgver.tar.gz)
sha256sums=('5caee269f9b38317036cf29877c5229013e422e1086b45b7c720a128c10b14f0')
sha512sums=('78bcf181d35bb7a1ab3f1eefae9cc03408f96dcbb36aeec78f4437d6b90f3f20d623e427c0f57047dff4b5b087539a3f056167e4c9f9da688ed8a6ca737aff98')

build() {
    cd pydeep-$pkgver/
    python2 setup.py build
}

package() {
    cd pydeep-$pkgver/
    python2 setup.py install --root="$pkgdir" --optimize=1
}
