# Maintainer: Custom Processing Unlimited <cpunltd[at]gmail[dot]com>
# Contributors: Wey (Archlinux forum user)
pkgname=cafepilot-server
pkgname1=CafePilot_Server
pkgver=2.4.0
pkgrel=3
pkgdesc="CafePilot is a cross-platform (Windows and Linux) client/server software suite that makes managing an Internet cafe of any size a breeze. This is the server program."
url="http://www.cafepilot.com"
arch=('any')
license=('GPL')
depends=('java-runtime')
# optdepends=('*')
# makedepends=()
# conflicts=()
# replaces=()
# backup=()
# install='*.install'
source=("http://sourceforge.net/projects/cafepilot/files/CafePilot/CafePilot%20Server%20and%20Client/CafePilot_Server.zip/download"
        "cafepilot-server.sh")
md5sums=('037926db71933273bf414029fe095f88'
         '2608e8d9a54306c1e652610765301e22')

package() {
  cd "${srcdir}"
  install -Dm755 $pkgname.sh $pkgdir/usr/bin/$pkgname.sh
  install -Dm644 $pkgname1.jar $pkgdir/opt/$pkgname1/$pkgname1.jar
  cp -r "$srcdir"/lib/ "$pkgdir"/opt/$pkgname1/
}

# vim:set ts=2 sw=2 et:
