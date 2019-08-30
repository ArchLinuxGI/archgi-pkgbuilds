
pkgname=arch-calamares-netinstall
_pkgname=arch-calamares-netinstall
_destname="/etc/calamares"
#_licensedir="/usr/share/arcolinux/licenses/"
pkgver=0.1
pkgrel=1
pkgdesc="calamares for arcolinux"
arch=('any')
url="https://github.com/ThavaNix/arch-calamares-netinstall.git"
#license=('')
makedepends=('git')
conflicts=('arcolinux-calamares-git-git' 'arcolinux-calamares-dev-git' 'calamares-netinstall' )
depends=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${_pkgname}::"git+https://github.com/ThavaNix/arch-calamares-netinstall.git")
sha256sums=('SKIP')
install='readme.install'
package() {
	mkdir -p "${pkgdir}${_licensedir}${_pkgname}"
	mv "${srcdir}/${_pkgname}/"LICENSE "${pkgdir}${_licensedir}${_pkgname}/LICENSE"
	mkdir -p "${pkgdir}${_destname}"
	cp -r "${srcdir}/${_pkgname}/calamares/"* "${pkgdir}${_destname}"
}