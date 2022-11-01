# hackintosh-b550m-pro4
opencore build for asrock b550m pro4
# AMD Ryzen Hackintosh - Opencore EFI for Asrock B550 / Gigabyte AOURUS ELITE V2 B550 series

![Screenshot 2022-11-02 at 01 02 48](https://user-images.githubusercontent.com/53318990/199350430-9eef59c6-0198-4886-91a8-0ecb6946d317.png)![Screenshot 2022-11-02 at 01 09 43](https://user-images.githubusercontent.com/53318990/199351516-76ba071c-82e7-420a-8d6f-c194ef1e78d6.png)

 - [[GeekBench5.4.5] Single/Multi-Core](https://browser.geekbench.com/v5/cpu/18373651)
 - [[GeekBench5.4.5] OpenCL](https://browser.geekbench.com/v5/compute/5807089)
## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 5 3600x @ 3.8GHz |
| Motherboard | Asrock B550m pro4 |
| RAM | 16GB (2 x 8GB) Corsair Vengeance RGB  |
| Audio Chipset | ALCS-1200A |
| GPU | Gigabyte RX 470  |
| Ethernet | RTL8111 1GbE |
| OS Disk (Nvme) | Samsung 970 EVO+ 250GB |

**macOS version**: Works with Monterey 12.3.1
**DualBoot to Windows**: Windows 11 Pro TPM disabled
**OpenCore version**: 0.8.5  

**SMBIOS**:  MacPro7,1

## Drivers & Kexts
 - [[Bootloader] OpenCore](https://github.com/acidanthera/OpenCorePkg)
 - [[Patch] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
 - [[Driver] FwRuntimeServices](https://github.com/acidanthera/OpenCorePkg)
 - [[Driver] HfsPlus](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)
 - [[Driver] OpenCanopyIcons](https://github.com/blackosx/OpenCanopyIcons)
 - [[Kext] Lilu](https://github.com/acidanthera/Lilu)
 - [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
 - [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
 - [[Kext] AppleMCEReporterDisabler](https://github.com/AMD-OSX/AMD_Vanilla/blob/opencore/Extra/AppleMCEReporterDisabler.kext.zip)
 - [[Kext] LucyRTL8125Ethernet](https://github.com/Mieze/LucyRTL8125Ethernet)
 - [[Kext] AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor)
 - [[Kext] SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)
 - [[Kext] SMCRadeonGPU](https://github.com/aluveitie/RadeonSensor)
 - [[Kext] USBPorts](https://dortania.github.io/OpenCore-Post-Install/usb/manual/manual.html#usb-mapping-the-manual-way)

## Working
- **Sleep/Wake**
- Ethernet 
	- Settings -> Network -> Ethernet -> Advenced -> Hardware: Set Configure from Automatically->Manually Then set Speed to 1000baseT, click ok and apply.

## Known issues
 - Mic > [See Details] (https://dortania.github.io/OpenCore-Post-Install/universal/audio.html#no-mic-on-amd) (Can be used USB Mics)
 - Hypervisor.framework (VirtualBox and XCode iOS emulator works)
 - Android Studio emulator (Can be replaced with Genymotion)
 - audio 
 - havent tested wifi/bt
## Apps that doesnt work
- Adobe Photoshop
- Autodesk AutoCad
 
## How to use
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as model select **MacPro7,1**.
  4. Boot it!  
## Cedits and links:
https://github.com/wildtigon/Hackintosh-Opencore-Asrock-B550M-Bigsur/blob/main/README.md
https://github.com/ToaRuGakusei/Ryzentosh-for-B550M-Pro4
r: u/beele
## Disclaimer

This documentation is published for the sole purpose of learning and tech enthusiasm and with no guarantees of any kind, I’m not responsible of any harm of any kind or loss of data that may occur.
