<p align="center">
  <img src="icon_hyperlight.png" alt="HyperLight logo" width="160" />
</p>

<h1 align="center">HyperLight</h1>

<p align="center">
  为小米 HyperOS 3 补全高光模糊（Highlight Blur）视觉效果的 Xposed 模块。<br>
  覆盖桌面、通知栏、控制中心等系统组件，通过反射调用系统内部 MaterialToken 接口，<br>
  为不支持高光模糊的设备或场景注入完整的OS3高光材质风格，并提供材质混色与描边的自定义选项。
</p>

<p align="center">
  <a href="./README_EN.md">English</a> · <a href="https://github.com/KiminonawaResa/HyperLight">项目主页</a>
</p>

<p align="center">
  <a href="https://github.com/KiminonawaResa/HyperLight/releases"><img src="https://img.shields.io/github/v/release/KiminonawaResa/HyperLight?display_name=tag" alt="GitHub release"></a>
  <a href="https://github.com/KiminonawaResa/HyperLight/stargazers"><img src="https://img.shields.io/github/stars/KiminonawaResa/HyperLight" alt="GitHub stars"></a>
  <a href="https://github.com/KiminonawaResa/HyperLight/issues"><img src="https://img.shields.io/github/issues/KiminonawaResa/HyperLight" alt="GitHub issues"></a>
  <a href="https://developer.android.com/"><img src="https://img.shields.io/badge/Android-15%2B-3DDC84?logo=android&logoColor=white" alt="Android"></a>
  <a href="https://github.com/LSPosed/LSPosed"><img src="https://img.shields.io/badge/Framework-LSPosed%20%2F%20Xposed-5C6BC0" alt="Framework"></a>
</p>

---

## 功能

### 桌面 (com.miui.home)
- 文件夹 / 小部件 / 快捷菜单高光模糊
- 自定义 Dock 栏
- 自定义桌面网格布局（行数、列数、间距）
- 自定义图标大小
- 最近任务卡片圆角
- 最近任务滑动振动反馈
- 自动隐藏导航栏
- 陀螺仪动态模糊效果

### 通知栏 (com.android.systemui)
- 通知栏高光模糊
- 自定义模糊半径
- 通知混合颜色自定义
- 长文本自动展开
- 头部渐变模糊效果
- 自定义居中大时钟
- 时钟 / 日期字体粗细调节
- 时钟 / 日期布局自定义
- 日期格式自定义
- 锁屏快捷按钮背景模糊
- Toast 通知模糊
- 导航栏相关 Hook
- 陀螺仪动态模糊效果

### 控制中心 (miui.systemui.plugin)
- 控制中心高光模糊（磁贴、卡片、媒体、亮度、音量、设备中心等）
- 阴影效果支持
- 图标颜色自定义（浅色 / 深色 / 跟随系统）
- 磁贴圆角调节
- iOS 风格细音量条
- 音量条展开动画
- 陀螺仪动态模糊效果

### 其他
- 个人助手小部件模糊优化
- 安全中心侧边工具箱模糊优化
- 副屏左滑手势注入
- 系统设置中添加模块入口
- 强制启用高级色彩风格模式
- 强制在 Android 15 / 中端设备上启用高光材质

## 兼容性

- 最低 Android 版本：Android 15 (API 35)
- 目标 Android 版本：Android 16 (API 36)
- 支持系统：HyperOS 3.x
- Xposed 框架：LSPosed
- 仅支持手机设备，平板等非手机设备均不适配

## 安装

1. 安装 LSPosed 框架
2. 下载并安装 HyperLight
3. 在 LSPosed 管理器中启用模块
4. 勾选以下作用域：
   - `com.android.systemui`
   - `com.miui.home`
   - `com.miui.securitycenter`
   - `com.miui.personalassistant`
   - `miui.systemui.plugin`
   - `com.android.settings`
   - `com.xiaomi.subscreencenter`
5. 重启设备或重启相关应用
6. 打开 HyperLight 进行配置

## 问题反馈

在 Issues 中提交反馈，请附带：

1. Xposed 框架日志（LSPosed: 设置 → 日志 → 详细日志）
2. 设备型号和系统版本
3. 复现步骤
4. 预期行为和实际行为
5. 相关截图

## 技术栈

- Kotlin + Java
- Jetpack Compose
- Xposed Framework (XposedBridgeApi-89)
- MiuiX KMP UI

## 许可证

本项目仅供学习交流使用。

## 致谢

- [MiuiX](https://github.com/miuix-kotlin-multiplatform/miuix) - UI 组件库

## Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=KiminonawaResa/HyperLight&type=Date)](https://star-history.dera.page/#KiminonawaResa/HyperLight&Date)

## 交流与讨论

Telegram 群组：[HyperLight](https://t.me/+8M40i3aiAEc0ZTg1)