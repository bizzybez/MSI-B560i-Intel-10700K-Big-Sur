# MSI B560i Intel 10700K Big Sur
This was a hastily put together build (went with the 500 series board because it was half the price of the 400 series ITX boards) and I got a great Black Friday deal on the 10700k, so the Board/CPU upgrade from my previous build (AMD) was around $300. Also went with an NZXT H1 case, which looks pretty awesome compared to the relatively large ATX case I had before. 

-Specs:
  - CPU: Intel 10700K (Comet Lake)
  - Mobo: MSI B560i (500 Series Intel)
  - GPU: AMD RX480

Notes: I haven't tested the iGPU (but I don't think it works). Bluetooth works. USB works. Sleep doesn't work. HDMI audio out works. Ethernet works. Adobe Apps don't crash, which is a nice change from my previous AMDOSX build (although there has been progress on that front).

All of this as of Dec 7, 2021.

## EFI STRUCTURE (OpenCore 0.7.6)

- ACPI
  - SSDT-AWAC-DISABLE.aml
  - SSDT-EC-USBX.aml
  - SSDT-PLUG.aml
  - SSDT-PMC.aml
  - SSDT-SBUS-MCHC.aml

- Drivers
  - HfsPlus.efi
  - OpenCanopy.efi
  - OpenRuntime.efi

- Kexts
  - AppleALC.kext
  - CPUFriend.kext
  - CPUFriendlyDataProvider.kext
  - CtlnaAHCIPort.kext
  - IntelBluetoothFirmware.kext
  - IntelBluetoothinjector.kext
  - Lilu.kext
  - LuxyRTL8125Ethernet.kext
  - NVMeFix.kext
  - RestrictEvents.kext
  - SMCProcessor.kext
  - SMCSuperIO.kext
  - USBToolBox.kext
  - UTBMap.kext
  - VirtualSMC.kext
  - WhateverGreen.kext

The config is only partially working. Uploaded for information purposes only. A few things aren't working yet, so if you get them to work let me know :)
