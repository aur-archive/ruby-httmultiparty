# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Anatol Pomozov <anatol.pomozov@gmail.com>

_gemname=httmultiparty
pkgname=ruby-$_gemname
pkgver=0.3.16
pkgrel=1
pkgdesc='HTTMultiParty is a thin wrapper around HTTParty to provide multipart uploads.'
arch=(any)
url='https://github.com/jwagener/httmultiparty'
license=(MIT)
depends=(ruby ruby-httparty ruby-multipart-post ruby-mimemagic)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('f4923f5cb0072e2e761ce81edcfc94b893c986d1')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
