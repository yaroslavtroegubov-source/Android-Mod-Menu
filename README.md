# Android-Mod-Menu (LGLTeam Reboot by NepMods)

![License](https://img.shields.io/github/license/NepMods/Android-Mod-Menu?style=flat-square)
![Maintenance](https://img.shields.io/badge/status-active-brightgreen?style=flat-square)
![Architectures](https://img.shields.io/badge/arch-ARM,%20ARM64,%20x86,%20x86_64-blue?style=flat-square)
![PRs](https://img.shields.io/badge/PRs-welcome-orange?style=flat-square)

> ⚙️ Rebooted version of the legendary LGLTeam Android Mod Menu. Fully maintained and modernized by **NepMods** to support all current Android versions and architectures.

![Description of gif](ModMenuDocs/output.gif)


---

## 📦 Features

- Floating mod menu framework for Android native games
- Supports `il2cpp`, Unity, and native binaries
- Java/C++ hybrid with a dynamic in-game overlay
- Menu styles: **LGL**, **DZ** with themes and layouts
- Fully compatible with **ARMv7**, **ARM64**, **x86**, and **x86_64**
- Feature-rich components: switches, sliders, input boxes, buttons, categories, spinners, etc.
- Minimal permissions, overlay without root required

---

## 🧱 Architecture

```
📁 app/src/main/java/com/android/support
├── base/                # Floating window manager
├── interfaces/          # Modular interface design for menus
├── ThemesData/          # LGL & DZ themed menu layouts and styles
└── *.java               # Main activity, launcher, preferences, etc.

📁 jni/
├── Includes/            # Utility classes (e.g., memory patching)
├── KittyMemory/         # Memory patching and scanning libs
├── Menu/                # JNI bridge and mod menu implementation
└── Main.cpp             # Entry point for native layer
```

---

## 📂 Getting Started

### Requirements

- Android Studio + NDK + CMake
- SDK 21+
- Rooted or non-rooted device (overlay permission required)

### Build

```bash
git clone https://github.com/NepMods/Android-Mod-Menu.git
cd Android-Mod-Menu
# Open in Android Studio or build using ndk-build / cmake
```

---

## 🧩 Components

- `FloatingWindowManager` — Creates and manages the draggable overlay
- `IFloatingBuilder` — Abstraction for service or activity-based windows
- `IMenuBuilder` — Builds mod feature lists and UI components
- `IMenuComponentFactory` — Generates switches, sliders, inputs, categories
- `DZTheme` / `LGLTheme` — Themed variants of the mod menu
- `KittyMemory` — Patching and memory manipulation utilities

---

## ✅ Contribution

This project is **actively maintained**.

- ✅ PRs welcome
- ✅ Issues open for bug reports & feature requests
- ✅ GPL-licensed, free to use, modify, and redistribute

---

## ⚠️ Disclaimer

This project is for **educational and personal learning purposes only**.  
Usage for cheating in competitive games or bypassing security in commercial software is **strictly discouraged**.

> This is a community revival project. Do **not** buy paid clones or get scammed on Telegram. This is and will remain **free**.

---

## 🧠 Credits

- Original Author: **LGLTeam** (archived)
- Contributors:
    - Octowolve / Escanor
    - VanHoevenTR
    - MrIkso
    - MJx0 (KittyMemory)
    - Rprop (And64InlineHook)
    - DZ Immortal

Reboot maintained by: **NepMods**.
