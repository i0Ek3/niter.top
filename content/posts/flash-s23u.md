+++

author = "i0Ek3"
date = "2023-11-25"
title = "Using Hong Kong Version(TGY) Firmware on China Version(CHC) S23U(SM-S9180) with macOS(Apple Chip) 
tags = [
    "Sharing",
]
categories = [
    "BG",
]

+++

# Using Hong Kong Version(TGY) Firmware on China Version(CHC) S23U(SM-S9180) with macOS(Apple Chip)

## Create a Virtual Machine for Windows(ARM)

Just follow the steps to create the VM via Parallels Desktop on your macOS(Apple Chip), after then enter the virtual Windows 11 stand by.

## Download Firmware and Tools

- [SamFirm](https://samfirmtool.com)(or [download TGY firmware manually](https://samfw.com/firmware/SM-S9180))
  - [Check Model/Code](https://www.sxrom.com)
  - ![](![s9180-choose-version](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-choose-version.6ua0eculvjpc.jpg))
  - ![](![s9180-download-TGY-firmware](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-download-TGY-firmware.8sz078ad1fc.jpg))
- [Odin](https://odindownloader.com)
- [Android USB Driver for Samsung Smartphone](https://developer.samsung.com/android-usb-driver)
- [Samsung Switch](https://www.samsung.com/global/download/)

After this, install all of these files on your virtual Windows, follow the order below:

- Android USB Driver
- Samsung Switch
  - to install Microsoft VC++ X86 2008/2010 deps automatically instead of manually, because SamFirm needs it and you cannot install the 2008/2010 version on Windows 11(ARM)
- SamFirm
- Odin

## Flash Firmware on Odin

- Unpackage TGY firmware and remain these four part(AP/BL/CP/CSC_OSZ)
  - ![](![s9180-remain-four-part](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-remain-four-part.73cf3cm28neo.jpg))
- Open Odin 3.14.4 and load these four parts, it will be take a while, just be patient
  - ![](![s9180-AP-loading](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-AP-loading.780sjc5xbnuo.jpg))
  - ![](![s9180-loading-packages](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-loading-packages.5dsom5r4nw5c.jpg))

- Power off the phone, press the volume Up + Down key for 5 seconds to enter the flash mode and then plug the USB-C cable between the phone and PC(choose option to connect the virtual Windows)

- After connecting the phone and virtual Windows, you will see this sign(0:[COM5] for my device)
- And then click the Start button until the big PASS showed for you, this step may take 5 minutes
  - ![](![s9180-start-to-flashing](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-start-to-flashing.3jqkx5h29q2o.jpg))
  - ![](![s9180-flash-success](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-flash-success.6w27jni0gqkg.jpg))

## Fixing Issues

### 1. Stuck on SetupConnection

If you plug in the cable before Odin loads the package, and then you will see the error message, so load the package for Odin first then plug in the cable.

![](![s9180-issue-stuck-on-setup-connection](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-issue-stuck-on-setup-connection.fyjy9bn6em0.jpg))

### 2. Complete(Write) opertion failed

During the flashing process, I used the official USC-C cable, which caused this issue. After I changed the USB-C cable, the issue was solved.

![](![s9180-complete(wirte)-operation-failed-issue](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-complete(wirte)-operation-failed-issue.33kr9i80uwzk.jpg))

### 3. An error has occurred while updating the device software

Don't worry, when you see this error message, which means you're still in flash mode, just re-flash the firmware on Odin can fix this issue. Of course, if you want to power off the phone, you can press the volume Down key + Power key for 3 seconds at a time. But this is a dead loop, and you will see it again.

![](![s9180-error-occurred](https://cdn.statically.io/gh/i0Ek3/apichost@main/20231125/s9180-error-occurred.1pe515uq2mww.jpg))

Yep, you almost there, enjoy~

## References

- https://blog.lucyqin.cn/?p=789
