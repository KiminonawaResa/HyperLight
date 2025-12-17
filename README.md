# HyperLight

[简体中文](#简体中文) | [English](#english)

---

## 简体中文

### 项目简介

HyperLight 是一个为 HyperOS 3 补全高光模糊效果的 Xposed 模块，为桌面、通知栏和控制中心带来统一的视觉体验。

### 功能特性

**系统桌面 (com.miui.home)**
- 文件夹高光模糊效果

**系统界面 (com.android.systemui)**
- 通知栏高光模糊效果

**控制中心 (miui.systemui.plugin)**
- 控制中心高光模糊效果
- 阴影效果支持
- 图标颜色自定义（浅色/深色/跟随系统）

### 版本适配

- 模块版本：1.0.0
- 目标 Android 版本：Android 16
- 支持系统：HyperOS 3.x
- Xposed 框架：LSPosed / Xposed

### 安装使用

1. 安装 Xposed 框架（推荐 LSPosed）
2. 下载安装 HyperLight 模块
3. 在 Xposed 管理器中启用模块
4. 勾选作用域：`com.miui.home` 和 `com.android.systemui`
5. 重启系统桌面和系统界面
6. 打开 HyperLight 应用进行设置

### 问题反馈

遇到问题请在 Issues 提交反馈，务必附带：

1. Xposed 框架日志（LSPosed: 设置 → 日志 → 详细日志）
2. 详细问题描述：
   - 设备型号
   - 系统版本
   - 复现步骤
   - 预期行为和实际行为
   - 相关截图

注意：不包含日志的 Issue 可能无法得到有效处理。

### 技术栈

- Xposed Framework
- Kotlin + Java
- Jetpack Compose
- MiuiX UI Components

### 致谢

- MiuiX - UI 组件库

### 开发者

愛君の名は

---

## English

### Introduction

HyperLight is an Xposed module that completes the highlight blur effects for HyperOS 3, bringing a unified visual experience to the desktop, notification shade, and control center.

### Features

**System Launcher (com.miui.home)**
- Folder highlight blur effect

**System UI (com.android.systemui)**
- Notification shade highlight blur effect

**Control Center (miui.systemui.plugin)**
- Control center highlight blur effect
- Shadow effect support
- Icon color customization (Light/Dark/Follow System)

### Compatibility

- Module Version: 1.0.0
- Target Android: Android 16
- Supported System: HyperOS 3.x
- Xposed Framework: LSPosed / Xposed

### Installation

1. Install Xposed framework (LSPosed recommended)
2. Download and install HyperLight module
3. Enable the module in Xposed Manager
4. Select scopes: `com.miui.home` and `com.android.systemui`
5. Restart System Launcher and System UI
6. Open HyperLight app for customization

### Bug Reports

Please submit feedback in Issues with the following information required:

1. Xposed Framework Logs (LSPosed: Settings → Logs → Verbose logs)
2. Detailed problem description:
   - Device model
   - System version
   - Steps to reproduce
   - Expected vs actual behavior
   - Related screenshots

Note: Issues without logs may not be effectively addressed.

### Tech Stack

- Xposed Framework
- Kotlin + Java
- Jetpack Compose
- MiuiX UI Components

### Acknowledgments

- MiuiX - UI Component Library

### Developer

愛君の名は
