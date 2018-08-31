Readme:
==
Description:
--
```
This code is separated from qsdk and partially modified from the Makefile.
```
Preconditions
--
```
Select a compiled openwrt tree, clone the code to the openwrt/package/
directory, and execute "make menuconfig" to configure it.
LEDE code tree does not work, error is reported when compiling
```
Compile configuration (ar750s)
--
```
	Target System (Atheros AR7xxx/AR9xxx) --->
	Boot Loaders --->
		<*> GL-uboot-ar750s.................... U-boot for AR750S
```
Compile configuration (ar750)
--
```
	Target System (Atheros AR7xxx/AR9xxx) --->
	Boot Loaders --->
		<*> GL-uboot-ar750.......................... U-boot for AR750S
```
Compile configuration (x750-4g)
--
```
	Target System (Atheros AR7xxx/AR9xxx) --->
	Boot Loaders --->
		<*> GL-uboot-x750-4g.................... U-boot for x750-4g
```
make package/uboot-gl-ar750-ar750s-x750/compile V=s

The compiled binary is in the openwrt/bin/ar71xx/ directory
