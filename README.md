### Resigned-realme_trinket-ROM

![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/zxrovx/Resigned-realme_trinket-ROM?include_prereleases)

**Description**

This repository contains Android ROMs that have been re-signed by zxrovx with the aim of ensuring that Android devices can pass security verifications such as Device Integrity or CTS (Compatibility Test Suite). Re-signing ROMs is essential for users who want to run applications requiring high security or access to specific services that require a verified device.

**Guide**

System and vendor files must be repacked with the UKA tool (Unpacker Kitchen Android), and the AVB.img file must be deleted before being compressed again

AVB.IMG LOCATION: 
/data/local/UnpackerSystem/config
( In system and vendor Directory )

- Copy Value Or Fill In system_size.txt And vendor_size.txt
- In UKA, look for the Compress Menu to .br, then look for compress according to size (number 2)
- Choose which one you want to compress first, system or vendor
- when the vendor copies vendor_size.txt and pastes it there, and vice versa on the system as well
- For vendors, when choosing a version, choose number 4
- Compress Level Choose 7 When You Want Small Size Files (HIGH COMPRESSION LEVEL), Or 5 and 6 when you want to compress with the (STANDARD COMPRESSION LEVEL)
- When you have finished, move all the files to the directory in /sdcard, it's up to you what folder you want to create
- Don't forget META-INF And other folders when available
- Compress all files into .zip extension with compression level (FASTEST)
- OK, after that you can delete other files that are no longer needed, don't forget to enter UKA, and select number 12 to clean the UKA directory, after that number 8 to clean everything in UKA
- After that, you can flash the zip that you compressed earlier containing the system and vendor files and other files that you repacked


**Credit**
Developed by zxrovx and available at [Resigned-realme_trinket-ROM](https://github.com/zxrovx/Resigned-realme_trinket-ROM).
