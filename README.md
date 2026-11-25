# Iris — Material 3 Theme Studio & System Theming Engine

Iris is a cross-platform Material 3 theme design studio and system theming engine for Android and Desktop (Qt 6 with a **Vulkan 1.3 & DirectX 12_1** rendering architecture). Iris allows designers and developers to generate WCAG-compliant color palettes from seed colors, wallpapers, or images, inspect contrast ratios, preview live Material 3 components, and export theme tokens directly to Compose, Qt, CSS, or Android XML resources.

---

## ⚡ Core Subsystems & Status Matrix

| Subsystem | Features & Capabilities | Status / Roadmap |
|---|---|---|
| **Graphics Engine** | **Vulkan 1.3 & DirectX 12_1** desktop viewport | Active |
| **Material 3 HCT Engine** | Seed color extraction, HCT color space arithmetic, WCAG AA/AAA contrast checker | Active |
| **Color Harmonization** | Extended color harmonization, custom color role builder, auto dark/light balancer | Roadmap |
| **Wallpaper Sampler** | Desktop & Android wallpaper color sampling, dominant color clustering | Active |
| **Dynamic Monet System** | Android 12+ Monet engine exporter, multi-region image palette sampler | Roadmap |
| **Component Preview** | Real-time Material 3 component preview (Buttons, Cards, Nav, Chips, Dialogs) | Active |
| **Multi-Format Exporter** | Export to Compose `ColorScheme`, Qt QML QPalette, CSS variables, Android XML | Active / Expanding |

---

## 🎨 Key Features & Subsystem Breakdown

### 🎨 Material 3 Palette Generator (`palettes`)
- **Current**: HCT (Hue, Chroma, Tone) color space palette generation, seed color extraction, tonal palettes (Primary, Secondary, Tertiary, Neutral, Neutral Variant, Error), and contrast verification (WCAG AA/AAA).
- **Planned / Roadmap**: Custom color role mapping, harmonized extended colors, and automatic dark/light contrast balancing.

### 🖼️ Wallpaper Color Extractor (`wallpaper`)
- **Current**: Wallpaper image color sampling, dominant color clustering, and dynamic system theme preview.
- **Planned / Roadmap**: Live wallpaper color tracking, multi-region image palette generation, and Android 12+ Monomorphic Monet theme exporter.

### 💻 Live Component Preview & Exporter (`exporter`)
- **Current**: Real-time component previews (Buttons, Cards, Navigation Bars, Chips, Dialogs) across Light, Dark, High Contrast, and Reduced Contrast modes; export to Jetpack Compose `ColorScheme` and JSON theme catalogs.
- **Planned / Roadmap**: Export to Qt QML QPalette / Material styles, CSS custom properties, Flutter ThemeData, and Android `colors.xml`.

---

## 🏗️ Architecture & Technology Stack

- **Graphics APIs**: Vulkan 1.3 & DirectX 12_1.
- **Android App**: Kotlin, Jetpack Compose, Material 3.
- **Desktop Shell**: Qt 6.12, QML, C++20.
- **Color Engine**: `material-color-utilities` (HCT color space arithmetic).
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

### Desktop (Windows)
```bat
build.bat Release
run.bat
```

### Android
```bash
./gradlew assembleDebug
```

---

## 📜 License

Iris is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
