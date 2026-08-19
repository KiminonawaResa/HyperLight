<p align="center">
  <img src="icon_hyperlight.png" alt="HyperLight logo" width="160" />
</p>

<h1 align="center">HyperLight</h1>

<p align="center">
  An Xposed module that brings highlight blur visual effects to Xiaomi HyperOS 3.<br>
  Covers system launcher, notification shade, control center and other system components by<br>
  invoking the internal MaterialToken API via reflection, injecting full OS3 highlight material<br>
  style on devices or scenarios that lack it, with material color blend and stroke customization.
</p>

<p align="center">
  <a href="./README.md">简体中文</a> · <a href="https://github.com/KiminonawaResa/HyperLight">Project Home</a>
</p>

<p align="center">
  <a href="https://github.com/KiminonawaResa/HyperLight/releases"><img src="https://img.shields.io/github/v/release/KiminonawaResa/HyperLight?display_name=tag" alt="GitHub release"></a>
  <a href="https://github.com/KiminonawaResa/HyperLight/stargazers"><img src="https://img.shields.io/github/stars/KiminonawaResa/HyperLight" alt="GitHub stars"></a>
  <a href="https://github.com/KiminonawaResa/HyperLight/issues"><img src="https://img.shields.io/github/issues/KiminonawaResa/HyperLight" alt="GitHub issues"></a>
  <a href="https://developer.android.com/"><img src="https://img.shields.io/badge/Android-15%2B-3DDC84?logo=android&logoColor=white" alt="Android"></a>
  <a href="https://github.com/LSPosed/LSPosed"><img src="https://img.shields.io/badge/Framework-LSPosed%20%2F%20Xposed-5C6BC0" alt="Framework"></a>
</p>

---

## Features

### Launcher (com.miui.home)
- Folder / widget / shortcut menu highlight blur
- Custom dock bar
- Custom desktop grid layout (rows, columns, padding)
- Custom icon size
- Recent tasks card corner radius
- Haptic feedback on recent tasks swipe
- Auto-hide navigation bar
- Gyroscope-based dynamic blur

### Notification Shade (com.android.systemui)
- Notification shade highlight blur
- Custom blur radius
- Notification blend color customization
- Long text auto-expand
- Header gradient blur effect
- Custom centered large clock
- Clock / date font weight adjustment
- Clock / date layout customization
- Date format customization
- Lockscreen shortcut button background blur
- Toast notification blur
- Navigation bar hooks
- Gyroscope-based dynamic blur

### Control Center (miui.systemui.plugin)
- Control center highlight blur (tiles, cards, media, brightness, volume, device center, etc.)
- Shadow effect support
- Icon color customization (Light / Dark / Follow System)
- Tile corner radius adjustment
- iOS-style thin volume bar
- Volume bar expand animation
- Gyroscope-based dynamic blur

### Other
- Personal Assistant widget blur optimization
- Security Center side toolbox blur optimization
- Sub-screen left swipe gesture injection
- Module entry in system settings
- Force enable advanced color style mode
- Force enable highlight material on Android 15 / mid-range devices

## Compatibility

- Minimum Android: Android 15 (API 35)
- Target Android: Android 16 (API 36)
- Supported system: HyperOS 3.x
- Xposed framework: LSPosed
- Only supports mobile devices; tablets and other non-mobile devices are not compatible

## Installation

1. Install LSPosed framework
2. Download and install HyperLight
3. Enable the module in LSPosed Manager
4. Select the following scopes:
   - `com.android.systemui`
   - `com.miui.home`
   - `com.miui.securitycenter`
   - `com.miui.personalassistant`
   - `miui.systemui.plugin`
   - `com.android.settings`
   - `com.xiaomi.subscreencenter`
5. Reboot the device or restart the relevant apps
6. Open HyperLight to configure

## Bug Reports

Please submit feedback in Issues with the following information:

1. Xposed framework logs (LSPosed: Settings -> Logs -> Verbose logs)
2. Device model and system version
3. Steps to reproduce
4. Expected vs actual behavior
5. Screenshots

## Tech Stack

- Kotlin + Java
- Jetpack Compose
- Xposed Framework (XposedBridgeApi-89)
- MiuiX KMP UI

## License

This project is for educational and personal use only.

## Acknowledgments

- [MiuiX](https://github.com/miuix-kotlin-multiplatform/miuix) - UI component library

## Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=KiminonawaResa/HyperLight&type=Date)](https://star-history.dera.page/#KiminonawaResa/HyperLight&Date)

## Communication & Discussion

Telegram Group: [HyperLight](https://t.me/+8M40i3aiAEc0ZTg1)