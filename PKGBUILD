pkgname=bt-dualboot-arhc
_pkgname=bt_dualboot
pkgver=1.1.0
pkgrel=5
pkgdesc="Sync Bluetooth for dualboot Linux and Windows"
arch=('any')
license=('GPL-3.0-only')
makedepends=('git' 'python-installer' 'python-wheel' 'python-build' 'python-poetry')
depends=('python' 'chntpw')

build(){
	python -m build --wheel --no-isolation
}

package() {
	python -m installer --destdir="$pkgdir" dist/*.whl
}