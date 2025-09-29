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

[uefi image](https://github.com/davidgm14059-tech/windows-samsung-galaxy-a40/releases/download/edk2-a40/boot-a40.img)

microSD card (or usb and OTG)

