# Maintainer: SGS <sgs at garudalinux dot org>

pkgname="uad-ng-bin"
pkgver=1.1.0
pkgrel=1
pkgdesc="Cross-platform GUI written in Rust using ADB to debloat non-rooted Android devices (next generation)"
arch=('x86_64')
url="https://github.com/sgse/universal-android-debloater-next-generation"
license=('GPL3')
depends=('android-tools' 'fontconfig' 'vulkan-icd-loader')
provides=('universal-android-debloater')
source=("$pkgname-$pkgver::$url/releases/download/$pkgver/uad-ng"
        "uad-ng.svg::$url/blob/main/resources/assets/uad-ng.svg?raw=true"
        "uad-ng.desktop")
b2sums=('SKIP'
        'SKIP'
        'SKIP')

package(){
 install -D -m 755 "uad-ng-bin-1.1.0" "$pkgdir/usr/bin/uad-ng"
 install -D -m 644 "uad-ng.desktop" -t "$pkgdir/usr/share/applications"
 install -D -m 644 "uad-ng.svg" -t "$pkgdir/usr/share/pixmaps"
}
