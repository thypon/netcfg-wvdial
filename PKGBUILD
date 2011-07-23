# Maintainer: Thypon <virus@gmx.us>
pkgname=netcfg-wvdial
pkgver=0.1
pkgrel=1
pkgdesc="OpenVPN support for wvdial"
arch=(i686 x86_64)
url="https://github.com/thypon/netcfg-wvdial"
license=('MIT')
depends=('netcfg>=2.5' 'wvdial' 'dtach')
source=(wvdial.example wvdial)
ums=('111293ebdc568b301763b6c39d1c25fa'
         '8e25517a26ea995a9d1aadb7bb893de8')

build() {
  install -Dm644 $srcdir/wvdial.example $pkgdir/etc/network.d/examples/wvdial
  install -Dm755 $srcdir/wvdial $pkgdir/usr/lib/network/connections/wvdial
}

