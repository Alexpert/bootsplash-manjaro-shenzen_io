pkgbase=bootsplash-themes
pkgname=('bootsplash-theme-manjaro-shenzen_io')
pkgver=0.2
pkgrel=2
url="https://lists.freedesktop.org/archives/dri-devel/2017-December/160242.html"
arch=('x86_64')
license=('GPL')

depends=()
builddepends=('imagemagick')
options=('!libtool' '!emptydirs')

source=('bootsplash-packer'
	'bootsplash-manjaro-shenzen_io.sh'
	'bootsplash-manjaro-shenzen_io.initcpio_install'
	'spinner.gif'
	'shenzen_io.png')

sha256sums=('SKIP'
            'SKIP'
            'SKIP'
            'SKIP'
            'SKIP')

build() {
  cd "$srcdir"
  sh ./bootsplash-manjaro-shenzen_io.sh
}

package_bootsplash-theme-manjaro-shenzen_io() {
  pkgdesc="Bootsplash Theme with Shenzen IO logo"
  cd "$srcdir"

  install -Dm644 "$srcdir/bootsplash-manjaro-shenzen_io" "$pkgdir/usr/lib/firmware/bootsplash-themes/manjaro-shenzen_io/bootsplash"
  install -Dm644 "$srcdir/bootsplash-manjaro-shenzen_io.initcpio_install" "$pkgdir/usr/lib/initcpio/install/bootsplash-manjaro-shenzen_io"
} 
