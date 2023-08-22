# HACKINTOSH-EFI-FOR-HP-15-DA0064NK

HP 15-DA0064NK OpenCore EFI for MacOs Ventura and Below

![print-usb-bluetooh](https://github.com/versionbeta10/HACKINTOSH-EFI-FOR-HP-15-DA0064NK-/assets/53920740/eebfe9e4-123e-4141-ab83-e3fcd16c3290)

<div id="badges" align="center">
  <img src="https://img.shields.io/badge/EFI-OC-blue">
  <img src="https://img.shields.io/badge/macOS-Ventura_13.5.1-orange">
</div>

# NOTE TO KEEP

This EFI is only for this PC model so if you want to use on other devices then it is on you.

## Table of Contents

*   [Specifications](#specifications)
*   [What's Working](#whats-working)
*   [What's not Working](#whats-not-working)
*   [Bios Options](#bios-options)
*   [SSDTs Used](#ssdts-used)
*   [Bonus](#bonus)
*   [Screenshots](#screenshots)

## Specifications

| Item  | Info  |
| ------------ | ------------ |
| Model  | HP 15-da0064nk  |
| Bios Version  | G9CN32WW  |
| CPU  |  Intel® Core™ i3 7020U |
| IGPU  |  Intel HD Graphics 620 |
| DGPU | NVIDIA GeForce MX110  |
| SSD | PNY CS900 240GO SSD 2.5 for macOS / TEAM GROUP MP33 128GO SSD M.2 for Windows 11  |
| WIFI | Realtek RTL8723DE  |
| Ethernet  | Realtek RTL8111  |
| Opencore Version  | 0.9.4  |
| SMBIOS used  | MacBookPro14,1 (Keep this SMBIOS so you can receive system updates from APPLE)  |
| Target MacOS Version  | MacOS Ventura 13.5.1  |

## What's Working

| Item | Status | Notes |
| --- | --- | --- |
| CPU | ✅ |   |
| IGPU | ✅ | With some DeviceProperties |
| Brightness Control | ✅ |   |
| HDMI A/V out | ✅ |   |
| USB | ✅ | currently using USBInjectAll.kext |
| Keyboard | ✅ | Voodoops2controller Kext |
| Audio | ✅ | AppleALC kext working with layout-id 13 |
| Trackpad | ✅ | VoodooI2C |
| Ethernet | ✅ | RealtekRTL8111 Kext |
| Bluetooth | ✅ | Internal Intel combo card with IntelBluetoothFirmware.kext + BlueToolFixup Kext |
| AppleTV+ DRM | ✅ | Work with CFG_LINK_FIXED_MAP=1 |
| Shutdown/Reboot | ✅ |   |

## What's not Working

| Item | Status | Notes |
| --- | --- | --- |
| Sleep | ❓ |  |
| iServices |  ❓ | Problem with FaceTime |
| DGPU | ❌ | MX110 not supported |
| Wi-Fi | ❌ | RTL8723DE not supported (Using dongle instead) |
| Bluetooth | ❌ |  |

## Bios Options

*   Secure Boot **Disabled**
*   Boot Type **UEFI**
## SSDTs Used

| Table | Description |
| --- | --- |
| SSDT-Disable_DGPU | Disables the DGPU |
| SSDT-GPI0 | Fixing I2C trackpads |
| SSDT-PNLF | Fixing the Brightness for KabyLake systems |

## Bonus

OC startup theme using chris1111 [themes.](https://github.com/chris1111/My-Simple-OC-Themes)

The theme used in this OC :

![oc-theme](https://raw.githubusercontent.com/chris1111/My-Simple-OC-Themes/master/View%20Boot%200.7/Flavours-Ventura13.png)

## Screenshots

![src1](https://github.com/versionbeta10/HACKINTOSH-EFI-FOR-HP-15-DA0064NK-/assets/53920740/eb856c51-1d0d-4b52-9268-b7288d1fa18a)

![src3](https://github.com/versionbeta10/HACKINTOSH-EFI-FOR-HP-15-DA0064NK-/assets/53920740/ba45d9d4-4cfa-4fc7-ae33-2567bc46c3cd)

![src2](https://github.com/versionbeta10/HACKINTOSH-EFI-FOR-HP-15-DA0064NK-/assets/53920740/d77da6c5-86dd-402e-ac45-a97de7b29cc6)
