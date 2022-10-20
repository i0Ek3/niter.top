+++
author = "i0Ek3"
date = "2022-06-18"
title = "Enable Removed Features and Apps on xiaomi.eu ROM"
tags = [
    "xiaomi.eu, MIUI, Magisk",
]
categories = [
    "PK",
]

+++

I reused my Android phone Redmi K30 Pro, so I need to install a stable ROM on it, boom, xiaomi.eu is here. But xiaomi.eu ROM reduced some features or apps from China version, so I need to flash magisk and localize modules to enable these features and apps. Before that, you should know what is xiaomi.eu and knows how to install eu ROMs on your phone.


## Prerequisites

- Unlock your phone
- xiaomi.eu ROM(weekly or stable version), [download here](https://sourceforge.net/projects/xiaomi-eu-multilang-miui-roms/files/xiaomi.eu/)
- Localize module files, [download here](https://minamigo-my.sharepoint.com/:f:/g/personal/koizumishouta_minamigo_onmicrosoft_com/EgLhpcA_G_5IugTq10F90r0BzUbaO7aHamxpZCUUgBgefg?e=VVvXXd)
- Magisk app, [download here](https://github.com/topjohnwu/Magisk/releases)
- Original boot/recovery image, used to patching
- LSPosed.zip, [download here](https://github.com/LSPosed/LSPosed/releases)

Or if you have the same phone with mine, download all of these files from [here(pwd: q2u5)](https://www.aliyundrive.com/s/H5e9kpQZwQ2).


## Steps

- Download the files mentioned above
- Install xiaomi.eu ROM on your phone, reboot and set it up
- Install Magisk app on your phone, check 
- Copy original boot/recovery image to your phone
- Open Magisk app and patching boot/recovery image
- After then, copy modified boot/recovery image to your computer
- Reboot phone to bootloader/fastboot mode, flash the modified boot/recovery image by corresponding command
    - `fastboot flash boot /path/to/magisk_patched.img` for pathced boot image
    - `fastboot flash recovery /path/to/magisk_patched.img` for patched recovery image
- After flashed, reboot your phone
- After phone rebooted, copy MIUI EU localize modules file to your phone
- And then, open Magisk app to install MIUI EU localize modules file, follow the prompts
- After then, reboot your phone, then you got a hacked xiaomi.eu ROM on your phone


## Summary

Living comfortably without anybody's help. 

The official installation tutorial is not detailed enough and needs to be carefully pondered so as not to damage the phone.


## References

- [Install Localize Modules](https://blog.minamigo.moe/archives/184)
- [Install Magisk](https://topjohnwu.github.io/Magisk/install.html)
