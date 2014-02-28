# OSX86 Drivers for Acer Aspire 4752
Mostly all components (except wi-fi) are working. Also HDMI audio works fine (tested on Mavericks 10.9.2)

------
Todo funciona, menos el wifi. También el audio HDMI (Cougar Point)

### Howto (Chameleon)

1. Copy DSDT.aml to /
2. Copy SSDT.aml to /Extra
3. Install provided kexts to /System/Library/Extensions
   
  Notice for AppleBCM5701Ethernet, you need to delete first     /System/Library/Extensions/IONetworkingFamily.kext/Contents/PlugIns/AppleBCM5701Ethernet.kext, then install the patched one.

4. Reboot and boot with -v -f options

For Clover, you need to mount your efi partition and replace DSDT.aml / SSDT.aml from EFI/CLOVER/ACPI/patched/ and overwrite (if exist) them with the ones provided here.

All the greetings are for the respective developers of the drivers.


