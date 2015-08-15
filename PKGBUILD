# Maintainer: Tristelune <tristelune_at_archlinux_dot_info>
# Contributor: Felipe Hommen <felibank_at_gmail.com>
# Contributor: moostik <mooostik_at_gmail.com>

pkgname=geogebra5-beta
pkgver=5.0.7.0
pkgrel=1
pkgdesc="Dynamic mathematics software with interactive graphics (2D and 3D), algebra and spreadsheet"
arch=('any')
url="http://www.geogebra.org/"
license=('GPL3 CCPL:by-nc-sa')
depends=('java-runtime' 'desktop-file-utils' 'hicolor-icon-theme' 'gsl' 'xdg-utils')
optdepends=()
conflicts=('geogebra')
#install='geogebra5-beta.install'
source=("http://download.geogebra.org/installers/5.0/GeoGebra-Linux-Portable-${pkgver}.tar.bz2"
		"geogebra")
md5sums=('19e77e24842417cddf7edacab4be5bc4'
         'b07c806e70d08709689903f4d47fa40f')

package() {

	cd "${srcdir}/GeoGebra-Linux-Portable-${pkgver}/geogebra/"
	install -dm 755 "${pkgdir}/usr/bin"
	install -dm 755 "${pkgdir}/usr/share/geogebra5-beta"
	cp * "${pkgdir}/usr/share/geogebra5-beta"
	cp ${srcdir}/geogebra ${pkgdir}/usr/bin
	

#mv ${pkgdir}/usr/bin/${pkgname} ${pkgdir}/usr/bin/${pkgname}-jogl2
#ln -s /usr/bin/${pkgname}-jogl1 ${pkgdir}/usr/bin/${pkgname} # We will use jogl1. jogl2 is in RC stage and doesn't work with some GPUs.
}

