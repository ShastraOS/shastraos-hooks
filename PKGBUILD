# Maintainer: Vivek Pal <31vivekpal@gmail.com>

pkgname="shastraos-hooks"
pkgver=0.1
pkgrel=1
pkgdesc='Pacman hooks for ShastraOS ISOs'
arch=('any')
license=('GPL3')
url="https://github.com/shastra-os/$pkgname"
depends=(libnotify)

source=(
       	'https://raw.githubusercontent.com/vivekpal1/shastraos-hooks/main/hooks-misc'
		'https://raw.githubusercontent.com/vivekpal1/shastraos-hooks/main/hooks-misc.hook'
		'https://raw.githubusercontent.com/vivekpal1/shastraos-hooks/main/hooks-runner'
		'https://raw.githubusercontent.com/vivekpal1/shastraos-hooks/main/hooks-runner.hook'
		'https://raw.githubusercontent.com/vivekpal1/shastraos-hooks/main/reboot-required'
)

sha512sums=(
			'f6f4d4355dbe78c73b9130fbc73f291c4fd83f0c99af8b5dc91f9690da685c3fad32856abbb2a504e5e5eb764866d488c93bc64eec940799c832e22f9d496497'
            '261213881e2ec0683fb54ee1aae2f837928c1339a23d7da86d25467ff6c3191963f3eefe59f21c251db9b86b84d7e8cc2af59312e977e3f6bc4186d40065de9d'
            '0333a47461c273c5ef539cc3514a6d61d045a6f855e6db896001955712afca8ed834e5c0457c29ced7dab4c043d06dbf374e76e2ef5ba8ab98e928ce030a69b5'
            '1ffd9127298840e7640e5617ba24e2746885dc8d8b9c044f3528072e2cf16e8e2a61f5306754225846cd9b48884030e2b32777e2b5b80f35dd466cae89036a1c'
	    	'b208d91ac62c320b7903fcdd42ef3f16f71149d2454cdf2fb3af9c21bfb45bb6bbae97cdb80014e6401bdfea8a8096598a287a284e9d02bc176ebd2a63d9f3ae'
            )

package() {
	local hooks=${pkgdir}/usr/share/libalpm/hooks
	local bin=${pkgdir}/usr/bin
	
	install -Dm644 hooks-misc           	"$hooks"/hooks-misc
	install -Dm644 hooks-misc.hook     	    "$hooks"/hooks-misc.hook
	install -Dm644 hooks-runner       	    "$hooks"/hooks-runner
	install -Dm644 hooks-runner.hook  	    "$hooks"/hooks-runner.hook
	install -Dm644 reboot-required    	    "$hooks"/reboot-required
}
