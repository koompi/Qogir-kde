pkgname="qogir-theme-koompi"
pkgver="0.1.1"
pkgrel=1
pkgdesc="Qorgir theme by Vinceliuice ported to match KOOMPI branding"
arch=('any')
url="https://github.com/koompi/Qogir-kde"
license=('GPL3')
source=('git+https://github.com/koompi/Qogir-kde.git')
md5sums=('SKIP')

prepare() {
    cd "${srcdir}/Qogir-kde"
    git checkout koompi
}

build() {
    cd "${srcdir}/Qogir-kde"
    mkdir -p "${srcdir}/Qogir-kde/root"
    sh install.sh
}

package() {
    cp -r "${srcdir}/Qogir-kde/root/usr" "${pkgdir}"
}
