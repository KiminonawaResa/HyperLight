<p align="center">
  <img src="icon_hyperlight.png" alt="HyperLight" width="120">
</p>

<h1 align="center">HyperLight</h1>

<p align="center">
  <b>Light up your HyperOS</b><br>
  <span>Highly customizable soft glass · system beautification for HyperOS</span>
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

## Overview

HyperLight is a **highly customizable soft-glass module for HyperOS** that also packs many unique customization features — a **system beautification module** for the notification shade, control center, lockscreen, and more.

| Core | Description |
| :--- | :--- |
| **Soft Glass** | Full control over blur, gloss, refraction, blend colors, and presets (primary stable capability) |
| **Highlight Material** | Complete / force-enable highlight; thickness & stroke tiers; independent blend colors |
| **Liquid Glass** | True liquid-glass rendering — long-term Beta; mind battery and performance |
| **UI Tweaks** | Clock, stacked notifications, volume bar, lockscreen, icon colors, and more |

## Features

<details>
<summary><b>Soft Glass / Highlight Material</b></summary>

- **Soft glass**: blur radius, luminance, saturation, brightness, refraction, reflection, directional light, inner tint, bloom, and more
- Per-scene background brightness: lockscreen, heads-up, volume bar, sidebar & negative-one screen
- Custom blend colors for notification center / control center tiles & widgets
- Built-in presets + save / import / share custom presets
- **Highlight material**: extra-thin to extra-thick tiers; pure / overlay / info series
- Strokes: small / medium / large; optional realtime dynamic stroke & advanced tuning
- Material blend colors: light / dark groups, per-component management

</details>

<details>
<summary><b>Liquid Glass</b> · long-term Beta</summary>

- Tunable refraction, chromatic aberration, depth, and highlight stroke
- Touch glow, optical padding, capture scale, and refresh tiers
- Enabling applies recommended defaults and warns about higher power use and initial jank

</details>

<details>
<summary><b>Notification / Lockscreen</b> · <code>com.android.systemui</code></summary>

- Unified soft glass, blend color, header gradient blur
- Long-text auto-expand; disable history fold / notification groups
- Stacked notifications: start line, blur opacity gradient, clock follow
- Centered large clock: weight, layout, glass, date format, title row
- Lockscreen: button backgrounds (highlight / liquid / soft), fingerprint icon, stack sink, depth avoid
- Notification & heads-up text colors; toast blur

</details>

<details>
<summary><b>Control Center</b> · <code>miui.systemui.plugin</code></summary>

- Soft glass / highlight material / liquid glass
- Tile corner radius; icon colors (light / dark / follow / anti-follow / custom)
- Thin volume bar with nudge animation (live-tunable)
- Shadows; flashlight notification blend

</details>

<details>
<summary><b>Other</b></summary>

- Personal Assistant widgets & Security Center toolbox with soft glass / blend
- Sub-screen left-swipe gesture injection
- AOD / lockscreen-edit depth-related tweaks
- Settings module entry; force advanced color style / highlight material
- Config backup via clipboard and JSON import / export

</details>

## Compatibility

| Item | Requirement |
| :--- | :--- |
| System | **HyperOS 4** (this branch, 1.2.0+) |
| Android | **16+** (minSdk 36 / targetSdk 37) |
| Framework | LSPosed with Xposed API **101** |
| Prerequisites | Bootloader unlocked + Root (Magisk / KernelSU) |
| Device | Phones only; tablets unsupported |

> For HyperOS 3, use the last supported release [1.1.7](https://github.com/KiminonawaResa/HyperLight/releases/tag/1.1.7-2(API_101)-LiquidGlass).

## Installation

1. Unlock Bootloader and obtain Root
2. Install an LSPosed build that supports API 101
3. Install the [HyperLight APK](https://github.com/KiminonawaResa/HyperLight/releases/latest)
4. Enable the module in LSPosed and select scopes:

   | Package | Component |
   | :--- | :--- |
   | `com.android.systemui` | Notification / lockscreen |
   | `miui.systemui.plugin` | Control center |
   | `com.miui.securitycenter` | Security Center |
   | `com.miui.personalassistant` | Personal Assistant |
   | `com.android.settings` | System Settings |
   | `com.xiaomi.subscreencenter` | Sub-screen |
   | `com.miui.aod` | AOD / lockscreen edit |

5. Reboot the device or the relevant apps
6. Open HyperLight and enable soft glass / highlight / liquid glass as desired

## Bug reports

Please open an [Issue](https://github.com/KiminonawaResa/HyperLight/issues) and include:

1. LSPosed verbose logs (Settings → Logs → Verbose logs)
2. Device model and system version
3. Steps to reproduce and expected vs actual behavior
4. Screenshots if available

## Tech stack

- Kotlin · Java · Jetpack Compose
- Xposed API 101 · libxposed
- [MiuiX](https://github.com/miuix-kotlin-multiplatform/miuix) · Haze · Capsule

## License

For educational and personal use only.

## Community

- Telegram group: [HyperLight](https://t.me/+8M40i3aiAEc0ZTg1)
- Developer: 愛君の名は / KiminonawaResa
- Liquid glass rendering: Aymon