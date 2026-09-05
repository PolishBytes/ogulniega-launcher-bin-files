pkgname=ogulniega-git
pkgver=1
pkgrel=1
pkgdesc="Ogulniega Minecraft launcher"
arch=('x86_64')
url="https://github.com/PolishBytes/ogulniega-launcher-bin-files"

depends=('gtk3' 'webkit2gtk-4.1' 'libsoup3')
makedepends=('git')
options=('!strip')

provides=('ogulniega')
conflicts=('ogulniega')

source=("git+${url}.git")
sha256sums=('SKIP')

pkgver() {
    cd ogulniega-launcher-bin-files
    printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cd "$srcdir/ogulniega-launcher-bin-files"

    install -Dm755 files/bin/ogulniega "$pkgdir/usr/bin/ogulniega"
    cp -dr --no-preserve=ownership files/share "$pkgdir/usr/"
}
