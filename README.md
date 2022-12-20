# Gigabyte Z690 Hackintosh EFI

Latest working macOS: Ventura 13.0.1 

Current OpenCore: 0.8.6

![Screenshot 2022-12-13 at 10 30 30 PM](https://user-images.githubusercontent.com/9337847/207340643-182129ca-b1b9-498c-8b8b-99e821397188.png)

* CPU Benchmark

![Screenshot 2022-12-20 at 1 38 59 PM](https://user-images.githubusercontent.com/9337847/208586303-16629b20-b0bc-4330-89df-44befae378c9.png)

* GPU Benchmark

![Screenshot 2022-12-20 at 1 40 52 PM](https://user-images.githubusercontent.com/9337847/208586332-e8e1f9b5-137f-42dc-be44-4da4da247969.png)


## Hardware
* Mainboard : Gigabyte Z690 Aorus Elite DDR5
* CPU : Intel i7-12700K
* VGA : ASUS Radeon RX6660 DUAL 8G D6 8GB
* SSD : Samsung 980 M.2 NVME 1TB MZ-V8V1T0BW
* Network : FV-T919(BCM94360)

## What works
* Audio
* HDMI/DP
* All USB ports
* WIFI / Bluetooth
* iCloud
* Airplay
* Universal Control

## What doesn't work
* Sidecar (Black Screen, due to the lack of supported iGPU)

## Bios Configuration
* Bios Configuration
* Hyper Threading - Enabled
* All P-Cores and E-Cores - Enabled
* CFG-Lock - off
* Above 4G decoding - on
* Fast Boot - off
* XHCI Hand-off - on

## Changelog
* v0.1
  * Initial release.
* v0.2 
  * Fixing somtimes black screen issue after verbose on boot.
    * Remove boot-args -v debug=0x100 keepsyms=1
    * Set in Misc > Debug, AppleDebug = False, ApplePanic = False, DisableWatchDog = True, Target = 0

## Reference
* <https://chriswayg.gitbook.io/opencore-visual-beginners-guide/advanced-topics/using-alder-lake>
* <https://www.reddit.com/r/hackintosh/comments/jwc8s5/comment/gcuz69f/?utm_source=share&utm_medium=web2x&context=3>
