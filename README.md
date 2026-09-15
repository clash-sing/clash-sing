# Clash Sing

English | [中文简体](README_CN.md)

A high-performance cross-platform proxy client developed with Flutter and powered by the [sing-box](https://github.com/SagerNet/sing-box) kernel, featuring support for sing-box, Clash, and V2Ray subscriptions.

[![Release](https://img.shields.io/github/v/release/clash-sing/clash-sing)](https://github.com/clash-sing/clash-sing/releases)
[![License](https://img.shields.io/github/license/clash-sing/clash-sing)](LICENSE)

## 🌟 Features

- **High-Performance Kernel**: Powered by `sing-box` 1.14.1 for extreme performance and stability.
- **In-House Core Plugin**: Utilizes the self-developed [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) plugin for efficient communication between Flutter and the sing-box kernel.
- **Subscription Compatibility**: Supports direct import and conversion of sing-box, Clash, and V2Ray subscriptions.
- **Desktop Experience**: Windows build featuring system tray, auto-start, and system proxy management.
- **Modern UI**: Developed with Flutter, providing a fluid, beautiful, and responsive user interface.
- **State Management**: Uses Riverpod 3.0 for reactive state management.
- **Fast Persistence**: Based on MMKV for millisecond-level data access.

## 📱 Platform Support

The project is currently under active development. Platform support progress is as follows:

| Platform | Status | Remarks |
| :--- | :--- | :--- |
| **Android** | ✅ Supported | Provides universal and per-architecture (arm64/v7a/x64) builds |
| **Windows** | ✅ Supported | Provides installer package (x64), with system tray and auto-start |
| **macOS** | ☐️ In Development | Planned support |
| **iOS** | ☐️ Planned | Pending adaptation |
| **Linux** | ☐️ Planned | Pending adaptation |

Both the Android and Windows builds support sing-box, Clash, and V2Ray subscriptions.

## 🚀 Download & Installation

You can visit the [Releases page](https://github.com/clash-sing/clash-sing/releases) to download the latest installation packages.

- **Android**:
    - `universal`: Includes all architectures, larger size, suitable for all phones.
    - `arm64-v8a`: Recommended version, suitable for most modern 64-bit Android phones.
    - `armeabi-v7a`: Suitable for older 32-bit Android devices.
    - `x86_64`: Suitable for Android emulators or certain tablets.
- **Windows**:
    - `x64`: Installer package for 64-bit Windows; install over an existing version to upgrade.

## 🛠️ Architecture Overview

- **Core**: Integrates the [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) plugin for kernel communication.
- **Logic**: Uses `Riverpod` for business logic and state subscriptions.
- **Data**: Uses `MMKV` to store user settings and configuration files.
- **Theme**: Full Material 3 theme support, including dark mode and dynamic color adaptation.

## 🤝 Contributing

Feedback via Issues or contributions through Pull Requests are welcome.

## 📄 License

This project is licensed under the [GPL-3.0 License](LICENSE).

---

**Disclaimer**: This tool is for learning and research purposes only. Please use it in compliance with local laws and regulations.
