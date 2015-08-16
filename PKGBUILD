# Contributor: Andrea Scarpino <andrea@archlinux.org>
# Contributor: Tobias Powalowski <tpowa@archlinux.org>

pkgname=libmal
pkgver=0.44.1
pkgrel=1
depends=('pilot-link>=0.12.1')
license=("MPL")
options=('!libtool')
pkgdesc="A convenience library of the object files contained in Tom Whittaker's malsync distribution"
arch=(i686 x86_64)
url="http://jasonday.home.att.net"
source=(http://www.jlogday.com/code/${pkgname}/${pkgname}-${pkgver}.tar.gz)
md5sums=('e9a3f8c7c825497c990e28e5e175e11c')

build(){
  cd ${srcdir}/${pkgname}-${pkgver}
  ./configure --prefix=/usr
  make || return 1
  make DESTDIR=${pkgdir} install
}
