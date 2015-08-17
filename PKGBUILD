# Manteiner: Elia Notarangelo < elia dot notarangelo at gmail dot com>
# Contributor: ale_xiovk < alexiobash at gmail dot com >

pkgname=wipetrash
pkgver=0.6
pkgrel=1
pkgdesc="a gtkdialog frontend gui for wipe trash and temporary files"
arch=('any')
url="http://www.xfce-italia.it/index.php?topic=660.0"
license=('GPL')
depends=('gtkdialog' 'zenity' 'wipe' 'xterm' 'sudo')
source=("http://master.dl.sourceforge.net/project/archmind/wipetrash/$pkgname-$pkgver.tar.gz")


build() {
	cd ${srcdir}/${pkgname}-${pkgver}

	BIN_DIR=${pkgdir}/usr/bin
	CONFIG_DIR=${pkgdir}/usr/share/${pkgname}
	ICON_DIR=${pkgdir}/usr/share/icons
	DESK_DIR=${pkgdir}/usr/share/applications

	install -d ${BIN_DIR} ${CONFIG_DIR} ${ICON_DIR} ${DESK_DIR}

	install -D COPYING wipetrash-lunch.sh ${CONFIG_DIR}
	install -D wipetrash.desktop ${DESK_DIR}
	install -D wipetrash.png ${ICON_DIR}
	install -D wipetrash ${BIN_DIR}
}


md5sums=('1d1b3593b75e5de232ccc52f843969cd')
