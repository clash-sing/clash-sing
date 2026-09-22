# Clash Sing

English | [中文简体](README_CN.md)

A high-performance cross-platform proxy client developed with Flutter and powered by the [sing-box](https://github.com/SagerNet/sing-box) kernel, featuring support for sing-box, Clash, and V2Ray subscriptions.

[![Release](https://img.shields.io/github/v/release/clash-sing/clash-sing)](https://github.com/clash-sing/clash-sing/releases)
[![License](https://img.shields.io/github/license/clash-sing/clash-sing)](LICENSE)

## 🌟 Features

- **High-Performance Kernel**: Powered by `sing-box` 1.14.1 for extreme performance and stability.
- **In-House Core Plugin**: Utilizes the self-developed [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) plugin for efficient communication between Flutter and the sing-box kernel.
- **Subscription Compatibility**: Supports direct import and conversion of sing-box, Clash, and V2Ray subscriptions.
- **Android TV Support (Beta)**: Phones and Android TVs share a single APK; the app detects the device form factor at launch and switches to a TV interface with remote-control (D-pad) navigation and LAN web import (QR code or URL push) for subscriptions. The TV interface is currently in preview and under active development.
- **Desktop Experience**: Windows build featuring system tray, auto-start, and system proxy management. Works on both amd64 and arm64 Windows with a single installer (on arm64 devices the kernel and system service run natively).
- **Modern UI**: Developed with Flutter, providing a fluid, beautiful, and responsive user interface.
- **State Management**: Uses Riverpod 3.0 for reactive state management.
- **Fast Persistence**: Based on MMKV for millisecond-level data access.

## 📱 Platform Support

The project is currently under active development. Platform support progress is as follows:

| Platform             | Status              | Remarks                                                                                                       |
| :------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------ |
| **Android**    | ✅ Supported        | Provides universal and per-architecture (arm64/v7a/x64) builds                                                |
| **Android TV** | 🧪 Beta             | Shares the same APK as phones; automatically switches to the TV interface (preview, under active development) |
| **Windows**    | ✅ Supported        | Single x64 installer for both amd64 & arm64 devices (kernel runs natively on arm64)                           |
| **macOS**      | ☐️ In Development | Planned support                                                                                               |
| **iOS**        | ☐️ Planned        | Pending adaptation                                                                                            |
| **Linux**      | ☐️ Planned        | Pending adaptation                                                                                            |

Both the Android (including Android TV) and Windows builds support sing-box, Clash, and V2Ray subscriptions.

## 🚀 Download & Installation

You can visit the [Releases page](https://github.com/clash-sing/clash_sing_app/releases) to download the latest installation packages.

- **Android** (all packages work on both phones and Android TVs; the TV interface appears automatically on TV devices; the TV interface is currently in beta):
  - `universal`: Includes 64-bit architectures (arm64/x86_64), larger size, suitable for most modern devices.
  - `arm64-v8a`: Recommended version, suitable for most modern 64-bit Android phones.
  - `armeabi-v7a`: Suitable for older 32-bit Android devices and TV boxes.
  - `x86_64`: Suitable for Android emulators or certain tablets.
- **Windows**:
  - `x64`: Installer for both amd64 and arm64 Windows — on arm64 devices (e.g. Snapdragon laptops) the app UI runs under Windows' built-in x64 emulation while the sing-box kernel and system service run natively as arm64; install over an existing version to upgrade.

## 🛠️ Architecture Overview

- **Core**: Integrates the [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) plugin for kernel communication.
- **Logic**: Uses `Riverpod` for business logic and state subscriptions.
- **Data**: Uses `MMKV` to store user settings and configuration files.
- **Theme**: Full Material 3 theme support, including dark mode and dynamic color adaptation.

## 🤝 Contributing

Feedback via Issues or contributions through Pull Requests are welcome.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

**Disclaimer**: This tool is for learning and research purposes only. Please use it in compliance with local laws and regulations.

