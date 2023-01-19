pkgname=blend-keyring
pkgver=2022.11.30
pkgrel=1
pkgdesc='blendOS PGP keyring'
url='https://github.com/blend-os/blend-keyring'
arch=('any')
license=('GPL')
install="${pkgname}.install"
source=('https://github.com/blend-os/blend-keyring/tarball/master')
validpgpkeys=('SKIP')
sha256sums=('SKIP')

package() {
	cd "$pkgdir"
 
	install -d usr/share/pacman/keyrings

	for f in blend.gpg blend-trusted blend-revoked; do
		install -m644 "$srcdir"/blend-os-blend-keyring-*/$f usr/share/pacman/keyrings/
	done
}
