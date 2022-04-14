# Maintainer: Diego Miguel <hello@diegomiguel.me>
# Maintainer: Gustavo Castro <gustawho@gmail.com>
# Contributor: Dmitry Porunov <dmitry@ykkz.de>

pkgname=ttf-apple-emoji
pkgver=15.4
pkgrel=1
pkgdesc='Apple Color Emoji is a color typeface used by iOS and macOS to display emoji'
arch=('any')
url='https://github.com/samuelngs/apple-emoji-linux'
license=('unknown')
provides=(emoji-font)
depends=()
conflicts=(
    'noto-fonts-emoji'
    'ttf-symbola'
    'ttf-joypixels'
    'ttf-twemoji-color'
    'ttf-whatsapp-emoji'
)

source=(
    AppleColorEmoji.ttf::$url/releases/download/ios-15.4/AppleColorEmoji.ttf
)

sha512sums=('8ecae021ec66ff373a85b69a5a4012f27483507053f754bf0d556c1b71526b2cf6e512188c33f66842f7a74305851f4f894abe21281e8233529f54a9ab56eefa')

package() {
    install -dm 755 "${pkgdir}/usr/share/fonts/TTF"
    install -m 644 AppleColorEmoji.ttf "${pkgdir}/usr/share/fonts/TTF/"
}
