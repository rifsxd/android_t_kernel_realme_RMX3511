# Uniperf Kernel for Realme C35 (RMX3511)

## Overview
Welcome to the custom kernel for the **Realme C35 (RMX3511)**! This kernel is based on **Linux 5.4.254** and is designed to enhance your device’s performance and flexibility. It includes **Uniperf**, a performance-oriented modifications, and **KernelSU**, a kernel-level rootkit providing extended control over your device.

### Key Features:
- **Linux Kernel 5.4.254**: Stable and well-tested for Android devices.
- **Uniperf (Modifications)**: Improved performance and battery life tuning to maximize device efficiency.
- **KernelSU (Rootkit)**: Full root access with security measures in place.
- **Android 12 - 14 Support**: Designed to run on all major recent Android versions.

## Modifications

### 1. **Uniperf (Performance amd Battery Life Modifications)**
This kernel integrates the **Uniperf** module for boosting performance and battery life. Key enhancements include:
- Dynamic CPU frequency scaling
- Improved task scheduling for reduced latency
- Enhanced memory management and I/O handling
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

| Feature         | Supported Versions         |
|-----------------|----------------------------|
| Device          | Realme C35 (RMX3511)        |
| Android Versions| Android 12 - 14             |
| Kernel Version  | 5.4.254                     |

## Installation

### Requirements:
1. **Unlocked bootloader** on your Realme C35.
2. A custom recovery like **TWRP**.
3. Backup your data before proceeding.

### Flashing the Kernel:
1. Download the kernel image from [Releases](#).
2. Boot into **TWRP** recovery.
3. Flash the kernel image:
    ```
    fastboot flash boot_a/boot_b boot.img
    ```
4. Reboot your device and enjoy the enhanced performance!

### Rooting with KernelSU:
After flashing the kernel, KernelSU should be active. You can install a root manager app to manage root permissions.

## Bug Reports & Contributions
If you encounter any issues or want to contribute to the development of this kernel, feel free to open an issue or pull request on the [GitHub Repository](#).

## Credits
- **Uniperf** for performance and battery life enhancements.
- **KernelSU** for root access.
- Special thanks to the **Android kernel development community**.
