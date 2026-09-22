# Clash Sing

[English](README.md) | 中文简体

一个基于 Flutter 开发、集成 [sing-box](https://github.com/SagerNet/sing-box) 内核的高性能跨平台代理客户端，支持 sing-box、Clash、V2Ray 订阅。

[![Release](https://img.shields.io/github/v/release/clash-sing/clash-sing)](https://github.com/clash-sing/clash-sing/releases)
[![License](https://img.shields.io/github/license/clash-sing/clash-sing)](LICENSE)

## 🌟 特性

- **高性能内核**: 由 `sing-box`（1.14.1）强力驱动，提供极致的性能和稳定性。
- **自研核心插件**: 采用自研的 [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) 插件，实现 Flutter 与 sing-box 内核的高效通信。
- **订阅兼容**: 支持 sing-box、Clash、V2Ray 订阅的导入与转换。
- **Android TV 适配（Beta）**: 手机与 Android TV 共用同一 APK，运行时自动识别设备形态切换 TV 界面，支持遥控器 D-pad 操作与局域网 Web 导入订阅（扫码或链接推送）；TV 界面当前为预览版，持续完善中。
- **桌面体验**: Windows 端支持系统托盘常驻、开机自启与系统代理管理；单一安装包同时支持 amd64 与 arm64 设备（arm64 上内核与系统服务原生运行）。
- **现代 UI**: 采用 Flutter 开发，提供流畅、美观且支持响应式的用户界面。
- **状态管理**: 使用 Riverpod 3.0 进行响应式状态管理。
- **快速持久化**: 基于 MMKV 提供毫秒级的数据存取。

## 📱 平台支持

目前项目处于活跃开发阶段，平台支持进度如下：

| 平台                 | 状态        | 备注                                                             |
| :------------------- | :---------- | :--------------------------------------------------------------- |
| **Android**    | ✅ 已支持   | 提供通用版本及分架构版本 (arm64/v7a/x64)                         |
| **Android TV** | 🧪 Beta     | 与手机共用同一 APK，运行时自动切换 TV 界面（预览版，持续完善中） |
| **Windows**    | ✅ 已支持   | 单一 x64 安装包通吃 amd64 与 arm64 设备（arm64 上内核原生运行）  |
| **macOS**      | ☐️ 开发中 | 计划支持                                                         |
| **iOS**        | ☐️ 计划中 | 待适配                                                           |
| **Linux**      | ☐️ 计划中 | 待适配                                                           |

Android（含 Android TV）与 Windows 端均已支持 sing-box、Clash、V2Ray 订阅。

## 🚀 下载安装

您可以前往 [Releases 页面](https://github.com/clash-sing/clash_sing_app/releases) 下载最新的安装包。

- **Android**（各架构安装包均同时适配手机与 Android TV，TV 设备上启动后自动进入 TV 界面；TV 界面当前为 Beta 预览版）:
  - `universal`: 包含 64 位架构（arm64/x86_64），体积较大，适合绝大多数现代设备。
  - `arm64-v8a`: 推荐版本，适用于现代绝大多数 64 位安卓手机。
  - `armeabi-v7a`: 适用于旧款 32 位安卓设备及电视盒子。
  - `x86_64`: 适用于安卓模拟器或部分平板。
- **Windows**:
  - `x64`: 适用于 amd64 与 arm64 Windows 的安装包——arm64 设备（如骁龙笔记本）上应用 UI 由 Windows 内置的 x64 模拟层运行，而 sing-box 内核与系统服务以原生 arm64 运行；覆盖安装即可完成升级。

## 🛠️ 架构概览

- **Core**: 集成 [flutter_sing_box](https://github.com/clash-sing/flutter_sing_box) 插件进行内核通信。
- **Logic**: 使用 `Riverpod` 处理业务逻辑与状态订阅。
- **Data**: 使用 `MMKV` 存储用户设置和配置文件。
- **Theme**: 完善的 Material 3 主题支持，包括深色模式和动态色彩适配。

## 🤝 贡献

欢迎通过 Issue 提交反馈，或提交 Pull Request 贡献代码。

## 📄 开源协议

本项目采用 [MIT License](LICENSE) 开源。

---

**免责声明**: 本工具仅供学习和研究使用，请在遵守当地法律法规的前提下使用。
