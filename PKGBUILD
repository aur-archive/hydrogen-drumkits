# Maintainer: Daniele Paolella <danielepaolella@email.it>
# Contributor: Artem Borisovskiy
pkgname=hydrogen-drumkits
pkgver=20100812
pkgrel=2
pkgdesc="Hydrogen drum kits"
arch=(any)
url="http://www.hydrogen-music.org/hcms/node/16"
license=('GPL2')
depends=(hydrogen)
changelog=ChangeLog
_sourcebase=http://downloads.sourceforge.net/project/hydrogen/Sound%20Libraries/Main%20sound%20libraries
source=($_sourcebase/VariBreaks.h2drumkit
        $_sourcebase/3355606kit.h2drumkit
        $_sourcebase/HipHop-1.h2drumkit
        $_sourcebase/HipHop-2.h2drumkit
        $_sourcebase/Synthie-1.h2drumkit
        $_sourcebase/TD-7kit.h2drumkit
        $_sourcebase/Techno-1.h2drumkit
        $_sourcebase/TR808909.h2drumkit
        $_sourcebase/Boss_DR-110.h2drumkit
        $_sourcebase/ErnysPercussion.h2drumkit
        $_sourcebase/ColomboAcousticDrumkit.h2drumkit
        $_sourcebase/YamahaVintageKit.h2drumkit
        $_sourcebase/EasternHop-1.h2drumkit
        $_sourcebase/K-27_Trash_Kit.h2drumkit
        $_sourcebase/Classic-808.h2drumkit
        $_sourcebase/Classic-626.h2drumkit
        $_sourcebase/ElectricEmpireKit.h2drumkit
        $_sourcebase/HardElectro1.h2drumkit
        $_sourcebase/Millo-Drums_v.1.h2drumkit
        $_sourcebase/Millo_MultiLayered2.h2drumkit
        $_sourcebase/Millo_MultiLayered3.h2drumkit
        $_sourcebase/deathmetal-drumkit.h2drumkit
        $_sourcebase/BJA_Pacific.h2drumkit
        $_sourcebase/circAfrique.h2drumkit)
md5sums=('a9c305829cd23c28ffd1647cb5c0bdfd'
         '5dad41a4f0fb5a9fda0af98b9f553060'
         '7f52d6ac56a31f5b618657d40d4eb86e'
         '217f38ebf2849b20ff3a5dca1994be08'
         '33f02627ac1489e4ab52c5f078c538b9'
         '635274624e0a739c51b70f72a58cfcec'
         'f91912fc88361dd8954c11f2e602aa25'
         '1db9cce82fbdaebac1ab4608be5853ea'
         'fb8ca90e4aa054a24fb07aa768b54d18'
         '0e96f5971d5db887a186d5739c12ab77'
         'cb11827e185ab5a6906967901495884b'
         '8f63997dd789179fa009f84cc515fb3e'
         '8750fcbe186e49a89bc18a9237ee6604'
         'f445c60d4625a6bfe6bb9dbac1ac0aa7'
         'c08d5093fc28a30a7542f0c89493e807'
         '86dbdb8d2f9b12690e92211d36c6fe7d'
         'df1bd778148cc25d8f63a8cc7aa91fcb'
         'f953edf3f4227d786df59b544370e379'
         '4c895d59c3bc5f3322d14789de345be2'
         '2da5b8ee87bce3e67464c61ba0b722dd'
         '79ca7360784ec72959aa07c3c584d76c'
         '0465025dcf6659657b773874d168c27b'
         'cde7a74a06edde3b5f85435c29909891'
         'e9d8604d2089abc764e54d1f209900b7')

package() {
	local _drumkitsdir="$pkgdir/usr/share/hydrogen/data/drumkits"
	local _drumkits=('VariBreaks'
	                 '3355606kit'
	                 'HipHop-1'
	                 'HipHop-2'
	                 'Synthie-1'
	                 'TD-7kit'
	                 'Techno-1'
	                 'TR808909'
	                 'Boss DR-110'
	                 'ErnysPercussion'
	                 'ColomboAcousticDrumkit'
	                 'YamahaVintageKit'
	                 'EasternHop-1'
	                 'K-27_Trash_Kit'
	                 'Classic-808'
	                 'Classic-626'
	                 'ElectricEmpireKit'
	                 'HardElectro1'
	                 'Millo-Drums_v.1'
	                 'Millo_MultiLayered2'
	                 'Millo_MultiLayered3'
	                 'DeathMetal'
	                 'BJA_Pacific'
	                 'circAfrique v4')
	install -d "$_drumkitsdir"
	for _drumkit in "${_drumkits[@]}"; do
		cp -a "$srcdir/$_drumkit" "$_drumkitsdir"
	done
	find "$_drumkitsdir" -name LICENCE -delete
	find "$_drumkitsdir" -type d -exec chmod 755 {} \;
	find "$_drumkitsdir" -type f -exec chmod 644 {} \;
}
