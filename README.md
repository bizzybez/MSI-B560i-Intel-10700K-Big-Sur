# MSI B560i Intel 10700K Big-Sur
This was a hastily put together build (went with the 500 series board because it was half the price of the 400 series ITX boards) and I got a great Black Friday deal on the 10700k, so the Board/CPU upgrade from my previous build (AMD) was around $300. Also went with an NZXT H1 case, which looks pretty awesome compared to the relatively large ATX case I had before. 

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
