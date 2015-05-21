pkgname=papirus-icon-theme-git
_pkgname=papirus-icon-theme
pkgver=2015.05.21
pkgrel=1
pkgdesc="Modded and adaptive Paper icon theme for KDE."
arch=('any')
url="https://github.com/varlesh/papirus-icon-theme"
license=('GPL3')
depends=()
makedepends=('git')
optdepends=()
provides=('moka-icons-git')
conflicts=('moka-icons-git')
source=('git+https://github.com/varlesh/papirus-icon-theme.git')
md5sums=('SKIP')

pkgver() {
  cd $srcdir/$_pkgname
}

package() {

  # create theme dirs
  install -d -m 755 "$pkgdir"/usr/share/icons/papirus

  # install theme
  cd $srcdir/papirus-icon-theme/papirus
  cp -r . "$pkgdir"/usr/share/icons/papirus/
}
