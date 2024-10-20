# Uniperf Kernel for Realme C35 (RMX3511)

## Overview
Welcome to the custom kernel for the **Realme C35 (RMX3511)**! This kernel is based on **Linux 5.4.254** and is designed to enhance your device’s performance and flexibility. It includes **Uniperf**, a performance and battery life oriented modifications, and **KernelSU**, a kernel-level rootkit providing extended control over your device.

<div align="center">
	
![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/rifsxd/android_t_kernel_realme_RMX3511/total?logo=github&label=Downloads&style=flat)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/rifsxd/android_t_kernel_realme_RMX3511?style=flat&label=Code%20Size)
[![Build kernel artifact](https://github.com/rifsxd/android_t_kernel_realme_RMX3511/actions/workflows/build_artifact.yml/badge.svg?branch=dev)](https://github.com/rifsxd/android_t_kernel_realme_RMX3511/actions/workflows/build_artifact.yml)

</div>

### Key Features:
- **Linux Kernel 5.4.254**: Stable and well-tested for Android devices.
- **Uniperf (Modifications)**: Improved performance and battery life tuning to maximize device efficiency.
- **KernelSU (Rootkit)**: Full root access with security measures in place.
- **SuSFS Patch**: Hide SU traces, Suspicious mounts and more.
- **Android 12 - 14 Support**: Designed to run on all major recent Android versions.

## Modifications

### 1. **Uniperf (CPU, Network, Ram, I/O, Latency and Battery Life Performance Modifications)**
This kernel integrates the **Uniperf** module for boosting performance and battery life. Key enhancements include:
- Dynamic CPU frequency scaling
- Improved task scheduling for reduced latency
- Enhanced memory management and I/O handling
- BBR Network congestion algorithm
- Ram optimized modifications. Example: KSM and a lot more.
- Interactive CPU governor as default 
- Added BFQ I/O scheduler
- Disabled debug logs

### 2. **KernelSU (Rootkit)**
Gain full control over your device with **KernelSU**. This feature allows root access, offering:
- Ability to run root-only applications.
- Custom control over device processes and configurations.
- Root with security management to avoid unintentional exploitation.
- Better hiding of root detection

### 3. **Additional Tweaks**
- Optimized battery life without sacrificing performance.
- Built-in support for various I/O schedulers.
- Improved power management for extended screen-on time.

## Compatibility

| Feature         | Supported Versions          |
|-----------------|-----------------------------|
| Device          | Realme C35 (RMX3511)        |
| Android Versions| Android 12 - 14             |
| Kernel Version  | 5.4.xxx                     |

## Installation

### Requirements:
1. **Unlocked bootloader** on your Realme C35.
2. A custom recovery like **TWRP**.
3. Backup your data before proceeding.

### Flashing the Kernel:

**METHOD 1**
1. Download the Anykernel3-xxx.zip from [Releases](https://guthub.com/rifsxd/android_t_kernel_realme_rmx3511/releases).
2. Boot into **TWRP** recovery.
3. Install the Anykernel3-xxx.zip and reboot.

**METHOD 2**
1. Download the boot.img from [Releases](https://guthub.com/rifsxd/android_t_kernel_realme_rmx3511/releases).
2. Reboot into bootloader.
3. Flash the kernel image:
    ```
    fastboot flash boot_a/boot_b boot.img
    ```
4. Reboot your device and enjoy the enhanced performance!

### Rooting with KernelSU:
After flashing the kernel, KernelSU should be active. You can install the KernelSU root manager app to manage root permissions.

## Bug Reports & Contributions
If you encounter any issues or want to contribute to the development of this kernel, feel free to open an issue or pull request on the [GitHub Repository](https://guthub.com/rifsxd/android_t_kernel_realme_rmx3511).

## Credits
- **Uniperf** for performance, battery life, ram, latency & network enhancements.
- [KernelSU](https://github.com/tiann/kernelsu) for root access.
- Special thanks to the **Android kernel development community**.
