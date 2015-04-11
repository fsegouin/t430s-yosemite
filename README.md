# t430s-yosemite
Kexts &amp; DSDT/SSDT files for Lenovo T430s

Please make sure you edit your config.plist - the plist file included
needs an SMBIOS & Rt variables. Use Clover Configurator to fix this. I suggest
you use MacBookPro9,2.

## System specs

**System:** Lenovo T430s

**CPU:** Intel Core i5 3320M (2,6 GHz)

**Graphics:** Intel HD Graphics HD4000, 1600x900

**SSD:** Samsung 840 Pro 256GB

**Audio:** Realtek ALC269VC

**WLAN:** TP-Link TL-WN725N (RTL8188CUS)

### What works

* Audio (Tried patching AppleHDA with no luck, now using VoodooHDA)
* Sleep (Kernel panic if your WLAN dongle is still connected at sleep)
* Touchpad
* Media keys (Volume Up/Down, Mute, Play, etc)
* Battery
* Brightness (Fn+P Brightness up / Fn+K Brightness down)
* All USB ports
* WLAN (With dongle)
* LAN
* Mini DisplayPort
* Webcam
* HD4000 with full QE/CI

### What doesn't work
* BT (Kernel panic at boot with all kexts I tried)
* VGA (Will never work since Apple removed VGA support)
* Integrated WLAN card (No kext available)
