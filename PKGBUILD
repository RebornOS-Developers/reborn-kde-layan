# Maintainer: cookiesource aka Cookie Alice <cookiesource@rebornos.org>
# Co maintainers: RebornOS Team <team@rebornos.org>
# Website: https://www.rebornos.org
# Support: https://discord.gg/cU5s6MPpQH
# Forum: https://rebornos.discourse.group/
pkgname=rebornos-kde-layan.git
_pkgname=rebornos-kde-layan
_destname1="/etc/skel/.config/"
_destname2="/etc/skel/.local/share/"
_destname3="/etc/xdg/"
pkgver=0.1
pkgrel=1
pkgdesc="RebornOS Layan theme configuration"
arch=('any')
url="https://github.com/cookiesource/rebornos-kde-layan"
license=('GPL2')
makedepends=('git')
depends=()
conflicts=('rebornos-kde-sweet')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${_pkgname}::"git+https://github.com/cookiesource/${_pkgname}.git")
sha256sums=('SKIP')
install='postinstall.install'
package() {

	install -dm755 ${pkgdir}${_destname1}
	cp -r  ${srcdir}/${_pkgname}${_destname1}* ${pkgdir}${_destname1}

	install -dm755 ${pkgdir}${_destname2}
	cp -r  ${srcdir}/${_pkgname}${_destname2}* ${pkgdir}${_destname2}

	install -dm755 ${pkgdir}${_destname3}
	cp -r  ${srcdir}/${_pkgname}${_destname3}* ${pkgdir}${_destname3}	
}
