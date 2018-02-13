# Maintainer: Asger Hautop Drewsen <asgerdrewsen@gmail.com>
pkgname=us_da-layout
pkgver=0.1.0
pkgrel=1
pkgdesc="US keyboard layout with level 3-4 æøå"
arch=('any')
url="https://github.com/Tyilo/us_da-layout"
license=('GPL')
depends=('xkeyboard-config' 'moreutils')
source=("us_da" "install-us_da-layout" "us_da-layout.hook")
install=us_da-layout.install

package() {
	install -Dm 644 "${srcdir}/us_da" "${pkgdir}/usr/share/X11/xkb/symbols/us_da"
	install -Dm 755 "${srcdir}/install-us_da-layout" "${pkgdir}/usr/share/libalpm/scripts/install-us_da-layout"
	install -Dm 644 "${srcdir}/us_da-layout.hook" "${pkgdir}/usr/share/libalpm/hooks/us_da-layout.hook"
}

sha256sums=('5f9e7e69a69a0c604640c9dd26ab56331af2027dc0ca42a9695feaa138f1e457'
            '9aa50c86a44ea0c4e2ca9eac34aab914a8f260e754b3e2d4c2b45da15b8c203c'
            '79a7cb2c8773b6489c5c8fe1b1db5f53b4e08c90ba8a6ad33e2ce66f362d3906')
