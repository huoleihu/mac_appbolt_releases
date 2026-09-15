# AppBolt

**macOS 菜单栏应用锁** —— 常驻菜单栏，一键锁定你指定的应用。未解锁前，受保护的应用无法被启动。

## 功能

- 🔐 **一键锁定**：在设置里勾选要保护的应用，菜单栏快速开关，锁定后无法被误启动或被他人打开。
- 📋 **受保护列表**：集中管理受保护应用，随时增删，状态在菜单栏实时显示。
- ⚡ **菜单栏常驻**：轻量常驻，不打扰工作流，需要时一键唤醒设置。
- 🔄 **自动更新**：内置 Sparkle，新版本自动推送，打开应用即可一键升级。
- 🎟️ **激活授权**：14 天免费试用，到期后输入激活码继续使用，绑定本机。
- 🍎 **原生体验**：纯 macOS 原生实现，贴合系统外观与交互，轻量无负担。

## 下载

前往 [Releases](https://github.com/huoleihu/mac_appbolt_releases/releases/latest) 下载最新版 `AppBolt-x.y.z.dmg`。

- 支持 **macOS 12+**
- 通过 **Sparkle** 自动更新（已配置 `appcast.xml`）

## 关于本仓库

本仓库是 **AppBolt 的发布分发仓库**，仅承载对外发布产物：

| 文件 | 作用 |
|---|---|
| `AppBolt-x.y.z.dmg` | 安装包（GitHub Release 直链下载） |
| `appcast.xml` | Sparkle 更新源，供应用内「检查更新」拉取 |
| `index.html` | 产品落地页（GitHub Pages 自动托管） |
| `appVersion.appbolt.json` | 版本信息清单（由前端服务读取） |

应用**源码**不在本仓库；发布流程由 `mac_appBolt` 工程里的 `Scripts/build_and_release.sh` 一键完成（编译 → 签名 → 打包 → 生成 appcast → 推送到本仓库 → 建 Release → 更新版本清单）。
