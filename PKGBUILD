#Maintainer: swindlesmccoop <https://swindlesmccoop.xyz>
#Contact: swindlesmccoop@waifu.club
pkgname="nyaa-cli"
pkgver=1
pkgrel=1
pkgdesc="Quickly download torrents from nyaa.si through the terminal"
arch=("any")
url="https://git.cbps.xyz/swindlesmccoop/nyaa-cli"
depends=("fzf" "git" "transmission-cli")
license=("custom")
md5sums=("SKIP")
source=("git+https://gitlab.com/swindlesmccoop/nyaa-cli.git")

pkgver() {
        cd "$pkgname"
        printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
        cd "$pkgname"
        install -Dm755 ./nyaa "$pkgdir/usr/bin/nyaa"
}
