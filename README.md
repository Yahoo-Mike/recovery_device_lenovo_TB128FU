# TWRP device tree for Lenovo Tab M10 Plus Gen 3 wifi (TB-128FU)
![Lenovo Tab M10 Plus Gen 3](https://p4-ofp.static.pub/fes/cms/2022/02/10/mzr7bhnqxvv3n35809y8blhsklcjpj515071.png "Lenovo Smart Tab M10 Plus Gen 3 (TB-128FU)")
## Release info
This is an unoffical build.  Install at your own risk.

There are five flavours of this tablet.  This TWRP will not work on all of them.
model    |   series    |     SOC       | LTE | will this TWRP work?
--------:|:-----------:|:-------------:|:---:|:--------------------
TB-328FU | ZAAE*,ZAAG* | UniSoc T610   |  -  |   no
TB-328FX | ZAAF*,ZAAH* | UniSoc T610   |  y  |   no 
TB-125FU | ZAAJ*,ZAAK* | MTK Helio G80 |  -  |   no
TB-128FU | ZAAM*,ZAAS* | QCom SDM680   |  -  |   yes
TB-128XU | ZAAN*,ZAAT* | QCom SDM680   |  y  |   possibly (TBA)

The TB-128FU has similar specs to the Lenovo Xiaoxin Pad 2022 and Moto Tab G62, so it might work on them too.

For more information, see the [XDA Developer's thread](https://forum.xda-developers.com/P11/development/recovery-twrp-3-3-x-lenovo-smart-tab-m10-plus-t4005859) . 

## About Device

Component    | Specs
------------:|:-------------------------------------------------------------------
Chipset      | Qualcomm Snapdragon 680 (SM6225)
CPU          | Kryo 265 Octa-core: 4x Cortex-A73 @2.4 GHz + 4x Cortex-A53 @1.9 GHz
GPU          | Qualcomm Adreno 610
Memory       | 4GB or 6GB LPDDR4X (soldered)
Android      | 12.0 (shipped with)
Storage      | 32GB, 64GB or 128GB (eMMC or uMCP)
MicroSD      | Up to 1 TB
Battery      | 7700 mAh, Li-Po (non-removable)
Display      | 2000x1200 pixels, 10.61", 400 nits
Front Camera | 8.0 MP, fixed focus
Rear Camera  | 8.0 MP, auto focus
Wifi         | 802.11a/b/g/n/ac dual band
Bluetooth    | v5.1
USB          | USB-C 2.0 (charging/storage/OTG)
Release Date | October 2022 (India)

## To build
Build with [minimal AOSP TWRP for Android 12.1](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/tree/twrp-12.1) 

```
. build/envsetup.sh
lunch twrp_TB128FU-eng
mka recoveryimage
```
