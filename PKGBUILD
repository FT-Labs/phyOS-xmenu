# Maintainer: Arda Atci<phystecharda@gmail.com>
pkgname=xmenu-phyOS
pkgver=1
pkgrel=1
pkgdesc="xmenu build for phyOS"
arch=(x86_64)
url="git://github.com/PhyTech-R0/xmenu-phyOS"
license=('MIT')
depends=('imlib2' 'libxft-bgra' 'libxinerama' 'freetype2' 'libxcb' 'fontconfig')
makedepends=('git' 'make')
provides=("xmenu")
conflicts=("xmenu")
options=('zipman')
source=('git://github.com/PhyTech-R0/xmenu-phyOS')
md5sums=('SKIP')

build() {
	cd "$pkgname"
	make
}

package() {
	cd "$pkgname"
	make PREFIX=/usr/local/ MANDIR=/share/man/man1 DESTDIR="$pkgdir/" install
}
