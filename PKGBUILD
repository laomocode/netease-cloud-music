# Maintainer: Peter Cai <peter at typeblog dot net>
pkgname=netease-cloud-music
pkgver=1.2.0.2
_pkgdate=20190428
pkgrel=1
pkgdesc="Netease Cloud Music, converted from .deb package"
arch=("x86_64")
url="http://music.163.com/"
license=('custom')
depends=('qcef')
source=(
	"https://mirrors.cloud.tencent.com/deepin/pool/main/n/netease-cloud-music/netease-cloud-music_${pkgver}-1%2Bstable_amd64.deb"
	"http://music.163.com/html/web2/service.html"
)
md5sums=('aca82e6f98d3110161eba515b833230f'
         'SKIP')

package() {
  cd ${srcdir}
  tar -xvf data.tar.xz -C ${pkgdir}
  install -D -m644 service.html ${pkgdir}/usr/share/licenses/$pkgname/license.html
}
