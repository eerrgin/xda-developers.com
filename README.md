# DeviceScope

DeviceScope is an Android system-information dashboard built with Kotlin and Jetpack Compose. It presents useful device, Android, display, memory, and battery details in a clean Material 3 interface.

> Status: personal open-source project / prototype. Values are read from Android APIs available to ordinary apps; some hardware fields may be unavailable or restricted on certain devices.

## Features

- Android version, API level, manufacturer, model, device codename, and build fingerprint
- Display resolution, density, and refresh rate
- Memory overview (total and available RAM)
- Battery level and charging state
- Runtime permission-free dashboard
- Material 3 UI with dark/light system theme support
- Small, modular Kotlin codebase

## Tech stack

- Kotlin
- Jetpack Compose
- Material 3
- Android framework APIs

## Build

1. Open this folder in Android Studio (Giraffe or newer recommended).
2. Allow Gradle to sync.
3. Run the `app` configuration on an Android device or emulator.

Requirements: JDK 17, Android SDK 35.

## Project structure

```text
DeviceScope/
├── app/
│   ├── src/main/
│   │   ├── java/dev/devicescope/
│   │   │   ├── MainActivity.kt
│   │   │   └── DeviceInfo.kt
│   │   └── AndroidManifest.xml
│   └── build.gradle.kts
├── build.gradle.kts
├── settings.gradle.kts
└── gradle.properties
```

## Notes

- RAM values are system-wide estimates reported by `ActivityManager.MemoryInfo`.
- Display values describe the default display and can differ from external displays.
- The app does not upload, collect, or transmit device information.
- This repository is not affiliated with XDA Developers.

## License

MIT. See [LICENSE](LICENSE).
