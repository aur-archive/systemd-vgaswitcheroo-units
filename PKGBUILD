# Maintainer: Adam Kürthy  <adikurthy at gmail dot com>
# Maintainer: Michael Bentlage <Mi.Bentlage at gmail dot com>
pkgname=systemd-vgaswitcheroo-units
pkgver=1.2
pkgrel=2
pkgdesc="Disable discrete GPU at boot for AMD/Intel dual stuff"
arch=('any')
# Based on the project "vgaswitcheroo_systemd" on github. (See URL)
url="https://github.com/fredoche/vgaswitcheroo_systemd"
license=('GPL')
depends=('systemd')
install=systemd-vgaswitcheroo-units.install
source=('vgaswitcheroo.service'
	'vgaswitcheroo_start.sh'
	'vgaswitcheroo_stop.sh')
package() {
  install -Dm644 "${srcdir}/vgaswitcheroo.service" "${pkgdir}/usr/lib/systemd/system/vgaswitcheroo.service"
  install -Dm755 "${srcdir}/vgaswitcheroo_start.sh" "${pkgdir}/usr/bin/vgaswitcheroo_start.sh"
  install -Dm755 "${srcdir}/vgaswitcheroo_stop.sh" "${pkgdir}/usr/bin/vgaswitcheroo_stop.sh"
}


md5sums=('f8a5c5422ed0b4eecff32028de0ca71e'
         '77840f9ba81f0fd281c1cab034fdf56a'
         '13ac1a25aa5eece63a986efc93206ee2')