pkgname=clipmenu-fork
_gitname=clipmenu
pkgver=6.2.0.r20
pkgrel=1
pkgdesc='Clipboard management using dmenu'
url='https://github.com/thomasave/clipmenu'
arch=('any')
license=('Public Domain')
depends=(dmenu xsel clipnotify rofi)
provides=(clipmenu)
conflicts=(clipmenu)
makedepends=(git)

source=(clipmenu clipmenud clipdel clipctl clipmenud.service)
md5sums=('SKIP' 'SKIP' 'SKIP' 'SKIP' 'SKIP')

package() {
    install -D -m755 clipmenu "${pkgdir?}/usr/bin/clipmenu"
    install -D -m755 clipmenud "${pkgdir?}/usr/bin/clipmenud"
    install -D -m755 clipdel "${pkgdir?}/usr/bin/clipdel"
    install -D -m755 clipctl "${pkgdir?}/usr/bin/clipctl"
    install -D -m755 clipmenud.service "${pkgdir?}/usr/lib/systemd/user/clipmenud.service"
}
