# Maintainer: Peter Cai <peter at typeblog dot net>
pkgname=netease-cloud-music
pkgver=1.2.0.2
_pkgrel=-1
pkgrel=1
pkgdesc="Netease Cloud Music, converted from .deb package"
arch=("x86_64")
url="http://music.163.com/"
license=('custom')
depends=(
	"alsa-lib" "gtk2" "nss" "libxss"
	"qt5-multimedia" "qt5-x11extras"
	"gst-libav" "gst-plugins-base"
	"gst-plugins-good" "gst-plugins-ugly"
	"gnome-themes-standard" "gconf" "atk"
	"glibc" "cairo" "vlc" "fontconfig"
	"dbus" "expat" "gdk-pixbuf2"
	"glib2" "pango" "libpulse" "sqlite"
	"gcc-libs" "libx11" "zlib" "qcef"
	"taglib" "libxext" "libxtst"
)
source=(
	"http://packages.deepin.com/deepin/pool/main/n/netease-cloud-music/netease-cloud-music_${pkgver}${_pkgrel}_amd64.deb"
	"http://music.163.com/html/web2/service.html"
)
md5sums=('408ee3d039d3f886dac286dbeac6a149'
         'SKIP')

package() {
  cd ${srcdir}
  tar -xvf data.tar.xz -C ${pkgdir}
  install -D -m644 service.html ${pkgdir}/usr/share/licenses/$pkgname/license.html
}
