# Maintainer: DarkXero <info@techxero.com>
pkgname=dark-cala-cfg
_destname1="/etc"
pkgver=3.3.0
pkgrel=4
pkgdesc="calamares 3.3 Config for XeroLinux"
arch=('any')
url="https://github.com/DarkXero-dev"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('calamares-config-dev')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
