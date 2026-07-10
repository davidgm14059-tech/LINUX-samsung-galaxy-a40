# Building the project
## getting started
### 1. install wsl
> [!NOTE]
> if you're using linux, you can skip this step, but
> if you're on windows and don't have wsl, to install it you need to
> open powershell as administrator, then run the following command:

```cmd
wsl --install
```
when installed, reboot your pc, if that dosen't work, you need to install it on microsoft store

now you need to install the following packages:

```cmd
sudo apt update
sudo apt install build-essential uuid-dev iasl git gcc-aarch64-linux-gnu g++-aarch64-linux-gnu python3 python3-distutils python3-pip nasm python-is-python3
```
### 2. prequisites
[bootloader unlocked](blunlock.md) (you MUST unlock the bootloader, otherwise you can't flash this)

[twrp](https://twrp.me/samsung/samsunggalaxya40.html)

[uefi image](https://github.com/davidgm14059-tech/windows-samsung-galaxy-a40/releases/download/newuefi/boot-a40-working.img)

[odin3](https://odindownload.com/download/)

[ADB and fastboot tools](https://github.com/fawazahmed0/Latest-adb-fastboot-installer-for-windows)

WoA drivers for a40 (no drivers yet)

microSD card (or usb and OTG)

### 3. installing twrp
> [!IMPORTANT]
> for installing twrp first you need to unlock the bootloader, if you did that before, skip this text

1. reboot the phone into download mode (if you don't know how to reboot in download mode, follow the frist steps of the guide for unlocking bootloader)
2. press vol up normally (no long press)
3. open odin3
4. click AP field and select TWRP tar file
5. click Userdata field and select the vbmeta file
6. click start
7. wait

### flashing image
> [!WARNING]
> DO NOT REBOOT YOUR PHONE IN THIS STEP, IF YOU REBOOT IT, YOUR PHONE WILL BE BRICKED

1. download uefi image
2. sideload it into a microSD or OTG
3. mount the OTG or microSD
4. flash the image that says "boot-a40" or something similar but the name needs to say "boot-a40" to prove that is uefi file
5. once it flashed, reboot your phone

> [!NOTE]
> now you will see renegade project logo and boot menu, if you select continue boot will bring you to efi shell until i
> fix this, apparently it's normal and happened to me, if did not happen to you, or you have an idea, make a issue with this tag on title: "[DISCUSSION]", otherwise if you have a problem,
> put in the title of your issue this tag: "[PROBLEM]"
