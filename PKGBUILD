# Maintainer: Frtz Qe <nextlxqt@gmail.com>

pkgname=lext-theme-narc-colors
upstream_pkgver="a3008f8"
pkgdesc="LXQt theme: Narc-Colors, incl. palettes and wallpapers ($upstream_pkgver)"

# root of upstream archive
upstreamRoot="Narc-Colors-Theme"

# Intentionally not following the release and version numbering of Lubuntu
pkgver=1
pkgrel=1

arch=('any')
url="https://github.com/lext-next/lext-theme-narc-colors"
license=('GPL-2.0')

depends=('lxqt-panel')
source=("git+https://codeberg.org/MrReplikant/Narc-Colors-Theme.git")

sha256sums=('SKIP')  # for testing; replace with real checksum later                                                                                                                          

#install=install.install

package() {                                                                                                                                                                                   

    install -d "$pkgdir/usr/share/lxqt/themes"
    install -d "$pkgdir/usr/share/lxqt/palettes"
    install -d "$pkgdir/usr/share/lxqt/wallpapers"

    cp -r "$srcdir"/$upstreamRoot/Narc-Colors "$pkgdir"/usr/share/lxqt/themes
    cp -r "$srcdir"/$upstreamRoot/palettes "$pkgdir"/usr/share/lxqt
    cp -rv "$srcdir"/$upstreamRoot/wallpapers "$pkgdir"/usr/share/lxqt
}
