<p align="center">
  <img src="icon_hyperlight.png" alt="HyperLight" width="120">
</p>

<h1 align="center">HyperLight</h1>

<p align="center">
  <b>Light up your HyperOS</b><br>
  <span>可高度自定义的 HyperOS 柔光玻璃 · 系统美化模块</span>
</p>

<p align="center">
  <a href="./README.md">简体中文</a> ·
  <a href="./README_EN.md">English</a>
</p>

<p align="center">
  <a href="https://github.com/KiminonawaResa/HyperLight/releases/latest"><img src="https://img.shields.io/github/v/release/KiminonawaResa/HyperLight?display_name=tag&label=release" alt="Release"></a>
  <a href="https://github.com/KiminonawaResa/HyperLight/stargazers"><img src="https://img.shields.io/github/stars/KiminonawaResa/HyperLight?style=flat&label=stars" alt="Stars"></a>
  <a href="https://github.com/KiminonawaResa/HyperLight/issues"><img src="https://img.shields.io/github/issues/KiminonawaResa/HyperLight" alt="Issues"></a>
  <img src="https://img.shields.io/badge/Android-16%2B-3DDC84?logo=android&logoColor=white" alt="Android">
  <img src="https://img.shields.io/badge/Xposed-API%20101-5C6BC0" alt="Xposed API">
  <img src="https://img.shields.io/badge/version-1.2.0-informational" alt="Version">
</p>

---

## 简介

HyperLight 是一个可高度自定义 **HyperOS 柔光玻璃**、且集成众多独有特色功能的 **系统美化模块**。  
面向通知栏、控制中心、锁屏等系统界面，带来统一、精致的视觉体验。

| 核心能力 | 说明 |
| :--- | :--- |
| **柔光玻璃** | 模糊、光影、折射、混色、预设等全参数可调（主推稳定能力） |
| **高光材质** | 补全 / 强制启用高光，厚度与描边分档，混色独立配置 |
| **液态玻璃** | 真液态玻璃渲染，长期 Beta，功耗与性能需自行权衡 |
| **界面定制** | 时钟、堆叠通知、音量条、锁屏、图标配色等 |

## 功能

<details>
<summary><b>柔光玻璃 / 高光材质</b></summary>

- **柔光玻璃**：模糊半径、柔光强度、饱和度、亮度、折射、反射、方向光、内部着色、烧灼等
- 分场景亮度：锁屏、悬浮通知、侧边音量条、侧边栏与负一屏
- 自定义混色（通知中心 / 控制中心磁贴与组件）
- 内置预设 + 自定义预设保存 / 导入 / 分享
- **高光材质**：超轻 ~ 超厚分档；纯净 / 叠加 / 信息系列
- 描边：小 / 中 / 大；可启用实时动态描边与高阶自定义
- 材质混色：浅色 / 深色分组，可按组件单独管理

</details>

<details>
<summary><b>液态玻璃</b> · 长期 Beta</summary>

- 折射、色散、景深、高光描边等渲染参数可调
- 触摸光晕、光学边距、捕获缩放与刷新档位
- 启用时会引导推荐配置，并提醒功耗上升与短期卡顿

</details>

<details>
<summary><b>通知 / 锁屏</b> · <code>com.android.systemui</code></summary>

- 柔光玻璃统一、背景模糊混色、头部渐变模糊
- 长文本自动展开、禁止收纳为通知组 / 历史
- 堆叠通知：起始线、模糊透明度渐变、时钟跟随
- 居中大时钟：字重、布局、玻璃、日期格式、标题行
- 锁屏：快捷按钮背景（高光 / 液态 / 柔光）、指纹图标、堆叠下沉、景深避让
- 通知文本与悬浮通知文本颜色；Toast 模糊

</details>

<details>
<summary><b>控制中心</b> · <code>miui.systemui.plugin</code></summary>

- 柔光玻璃 / 高光材质 / 液态玻璃
- 磁贴圆角；图标颜色（浅 / 深 / 跟随 / 反跟随 / 自定义）
- 细音量条与按压动画（可实时调参）
- 阴影、手电筒通知混色

</details>

<details>
<summary><b>其他</b></summary>

- 负一屏组件、安全中心侧边栏接入柔光玻璃与混色
- 背屏左滑手势注入
- 息屏与锁屏编辑景深相关调整
- 系统设置模块入口；强制色彩风格高级模式 / 高光材质
- 配置备份：剪贴板与 JSON 导入导出

</details>

## 兼容性

| 项目 | 要求 |
| :--- | :--- |
| 系统 | **HyperOS 4**（本分支 1.2.0+） |
| Android | **16+**（minSdk 36 / targetSdk 37） |
| 框架 | 支持 Xposed API **101** 的 LSPosed |
| 前提 | 解锁 Bootloader + Root（Magisk / KernelSU） |
| 设备 | 仅手机；平板不适配且不接受相关反馈 |

> HyperOS 3 请使用最后适配版本 [1.1.7](https://github.com/KiminonawaResa/HyperLight/releases/tag/1.1.7)。

## 安装

1. 解锁 Bootloader，并获取 Root
2. 安装支持 API 101 的 LSPosed
3. 安装 [HyperLight APK](https://github.com/KiminonawaResa/HyperLight/releases/latest)
4. 在 LSPosed 中启用模块，并勾选作用域：

   | 包名 | 组件 |
   | :--- | :--- |
   | `com.android.systemui` | 通知 / 锁屏 |
   | `miui.systemui.plugin` | 控制中心 |
   | `com.miui.securitycenter` | 安全中心 |
   | `com.miui.personalassistant` | 智能助理（负一屏） |
   | `com.android.settings` | 系统设置 |
   | `com.xiaomi.subscreencenter` | 背屏 |
   | `com.miui.aod` | 息屏与锁屏编辑 |

5. 重启设备或相关应用
6. 打开 HyperLight，按需启用柔光玻璃 / 高光 / 液态玻璃并调参

## 反馈

请通过 [Issues](https://github.com/KiminonawaResa/HyperLight/issues) 提交，并附上：

1. LSPosed 详细日志（设置 → 日志 → 详细日志）
2. 机型与系统版本
3. 复现步骤与预期 / 实际行为
4. 相关截图

## 技术栈

- Kotlin · Java · Jetpack Compose
- Xposed API 101 · libxposed
- [MiuiX](https://github.com/miuix-kotlin-multiplatform/miuix) · Haze · Capsule

## 许可证

本项目仅供学习交流使用。

## 社区

- Telegram 群组：[HyperLight](https://t.me/+8M40i3aiAEc0ZTg1)
- 开发者：愛君の名は / KiminonawaResa
- 液态玻璃渲染代码：Aymon