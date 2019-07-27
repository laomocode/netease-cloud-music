# Maintainer: Peter Cai <peter at typeblog dot net>
pkgname=netease-cloud-music
pkgver=1.2.1
pkgrel=1
pkgdesc="Netease Cloud Music, converted from .deb package"
arch=("x86_64")
url="http://music.163.com/"
license=('custom')
depends=('qcef')
source=(
	"data.tar.xz"
	"http://music.163.com/html/web2/service.html"
)
md5sums=('7b87119b7a44b8a7522f6cd1994feda7'
         'SKIP')

package() {
  cd ${srcdir}
  tar -xvf data.tar.xz -C ${pkgdir}
  install -D -m644 service.html ${pkgdir}/usr/share/licenses/$pkgname/license.html
}
