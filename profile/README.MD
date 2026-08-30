## xiaomi-plato-devs
<img align="right" height="180" src="https://i02.appmifile.com/898_operator_sg/26/08/2022/fc94660da1d6dd006f7589327bb72813.png">

This organization contains trees to build AOSP for Xiaomi 12T.
<br>Get started by adding [local_manifest](https://github.com/mt6895-plato/local_manifest) to your ROM. (`.repo/local_manifests/plato.xml`)

Current Branch: 
  - `16.2` (Android 16 QPR2) (for now - there are some which hasn't fixed yet i think)
  - `17.0` (Android 17 QPR0)

All credits goes to [xiaomi-mediatek-devs](https://github.com/xiaomi-mediatek-devs), [xiaomi-mt6895-devs](https://github.com/xiaomi-mt6895-devs), and [XagaForge](https://github.com/XagaForge) for all of the trees.

### Required trees:
* [Xiaomi 12T Device Tree](https://github.com/mt6895-plato/android_device_xiaomi_plato) (`android_device_xiaomi_plato`)
* [Xiaomi 12T Vendor Tree](https://gitlab.com/archcloudy/android_vendor_xiaomi_plato) (`android_vendor_xiaomi_plato`)
* [MT6895 Common Tree](https://github.com/mt6895-plato/android_device_xiaomi_mt6895-common) (`android_device_xiaomi_mt6895-common`)
* [MT6895 Vendor Tree](https://github.com/mt6895-plato/android_vendor_xiaomi_mt6895-common) (`android_vendor_xiaomi_mt6895-common`)
* [MT6895 Kernel Tree](https://github.com/mt6895-plato/android_kernel_xiaomi_mt6895) (`android_kernel_xiaomi_mt6895`)

### Other required trees:
* [Mediatek Sepolicy](https://github.com/mt6895-plato/android_device_mediatek_sepolicy_vndr) (`android_device_mediatek_sepolicy_vndr`)
* [Mediatek Hardware](https://github.com/mt6895-plato/android_hardware_mediatek) (`android_hardware_mediatek`)
* [Xiaomi Hardware](https://github.com/mt6895-plato/android_hardware_xiaomi) (`android_hardware_xiaomi`)

### Optional trees (MiuiCamera (WIP))
* [plato-MiuiCamera Device Tree](https://github.com/mt6895-plato/android_device_xiaomi_plato-miuicamera) (`android_device_xiaomi_plato-miuicamera`)
* [plato-MiuiCamera Vendor Tree](https://gitlab.com/archcloudy/android_vendor_xiaomi_plato-miuicamera) (`android_vendor_xiaomi_plato-miuicamera`)

### Required Patches
* [Return false for GetDeviceLockStatus() if fenrir=true](https://github.com/XagaForge/android_system_core/commit/f443c69db2291f7c156be86ba21ee0d7543ab4e7) (`android_system_core`)
* [Add xiaomi packages to the whitelist](https://github.com/mt6895-plato/android_build_soong/commit/cb80ea9a80796518350ab7193ceaf5649ddde091) (`android_build_soong`)
* [Whitelist Camera Extensions](https://github.com/mt6895-plato/android_build_soong/commit/08657b478323a9451b9d31aaa32891c98df8fe24) (`android_build_soong`)
