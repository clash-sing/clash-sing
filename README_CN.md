# Clash Sing

[English](README.md) | 中文简体

一个基于 Flutter 开发、集成 [sing-box](https://github.com/SagerNet/sing-box) 内核的高性能跨平台代理客户端，支持 sing-box、Clash、V2Ray 订阅。

[![Release](https://img.shields.io/github/v/release/clash-sing/clash-sing)](https://github.com/clash-sing/clash-sing/releases)
[![License](https://img.shields.io/github/license/clash-sing/clash-sing)](LICENSE)

## 🌟 特性

- **高性能内核**: 由 `sing-box` 强力驱动，提供极致的性能和稳定性。
- **自研核心插件**: 采用自研的 [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) 插件，实现 Flutter 与 sing-box 内核的高效通信。
- **订阅兼容**: 支持 sing-box、Clash、V2Ray 订阅的导入与转换。
- **桌面体验**: Windows 端支持系统托盘常驻、开机自启与系统代理管理。
- **现代 UI**: 采用 Flutter 开发，提供流畅、美观且支持响应式的用户界面。
- **状态管理**: 使用 Riverpod 3.0 进行响应式状态管理。
- **快速持久化**: 基于 MMKV 提供毫秒级的数据存取。

## 📱 平台支持

目前项目处于活跃开发阶段，平台支持进度如下：

| 平台 | 状态 | 备注 |
| :--- | :--- | :--- |
| **Android** | ✅ 已支持 | 提供通用版本及分架构版本 (arm64/v7a/x64) |
| **Windows** | ✅ 已支持 | 提供安装包 (x64)，支持系统托盘与开机自启 |
| **macOS** | ☐️ 开发中 | 计划支持 |
| **iOS** | ☐️ 计划中 | 待适配 |
| **Linux** | ☐️ 计划中 | 待适配 |

Android 与 Windows 端均已支持 sing-box、Clash、V2Ray 订阅。

## 🚀 下载安装

您可以前往 [Releases 页面](https://github.com/clash-sing/clash-sing/releases) 下载最新的安装包。

- **Android**:
    - `universal`: 包含所有架构，体积较大，适合所有手机。
    - `arm64-v8a`: 推荐版本，适用于现代绝大多数 64 位安卓手机。
    - `armeabi-v7a`: 适用于旧款 32 位安卓设备。
    - `x86_64`: 适用于安卓模拟器或部分平板。
- **Windows**:
    - `x64`: 适用于 64 位 Windows 的安装包，覆盖安装即可完成升级。

## 🛠️ 架构概览

- **Core**: 集成 [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) 插件进行内核通信。
- **Logic**: 使用 `Riverpod` 处理业务逻辑与状态订阅。
- **Data**: 使用 `MMKV` 存储用户设置和配置文件。
- **Theme**: 完善的 Material 3 主题支持，包括深色模式和动态色彩适配。

## 🤝 贡献

欢迎通过 Issue 提交反馈，或提交 Pull Request 贡献代码。

## 📄 开源协议

本项目采用 [GPL-3.0 License](LICENSE) 开源。

---

**免责声明**: 本工具仅供学习和研究使用，请在遵守当地法律法规的前提下使用。
