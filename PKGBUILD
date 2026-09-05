pkgname=ogulniega
pkgver=0.11
pkgrel=1
pkgdesc="Ogulniega Minecraft launcher"
arch=('x86_64')
url="https://github.com/PolishBytes/ogulniega-launcher-bin-files"
license=('LicenseRef-Proprietary')

depends=('gtk3' 'webkit2gtk-4.1' 'libsoup3')
options=('!strip')

_commit='f5532642b59fcc941b55be11524545f351554623'
source=("${url}/archive/${_commit}.tar.gz")
sha256sums=('88261216bc36b20d51aa7b808ea089a7d581f877b7210077d6d5e65a691a49a0')

package() {
    cd "$srcdir/ogulniega-launcher-bin-files-${_commit}"

    install -Dm755 files/bin/ogulniega "$pkgdir/usr/bin/ogulniega"
    cp -dr --no-preserve=ownership files/share "$pkgdir/usr/"
}
