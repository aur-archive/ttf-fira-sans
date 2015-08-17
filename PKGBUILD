# Maintainer: Markus Weimar <mail at markusweimar dot de>
pkgname=ttf-fira-sans
epoch=1
pkgver=3.111
pkgrel=1
depends=('fontconfig' 'xorg-font-utils')
pkgdesc="A sans-serif typeface designed for Firefox OS."
arch=('any')
url="https://www.mozilla.org/en-US/styleguide/products/firefox-os/typeface/"
license=('custom:OFL')
source=("http://www.markusweimar.de/public/ttf-fira-sans-3.111.tar.xz")
install=${pkgname}.install
md5sums=('2b842c2f7b46d9ed4d745978b5ccef68')

package() {
  cd ${srcdir}/ttf-fira-sans-${pkgver}
  install -d ${pkgdir}/usr/share/fonts/TTF/
  install -m644 *.ttf ${pkgdir}/usr/share/fonts/TTF/
  install -D -m644 OFL.txt ${pkgdir}/usr/share/licenses/${pkgname}/OFL.txt
}
