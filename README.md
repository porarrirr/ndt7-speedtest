# NDT7 Speed Test

English | [日本語](README.ja.md)

A Flutter app for measuring download and upload performance on iOS and Android using Measurement Lab's NDT7 infrastructure. No self-hosted measurement server is required.

## Features

- Consent screen before the first measurement
- Manual download and upload speed tests
- Live progress for each test phase
- Local result history with Wi-Fi and mobile filtering
- Detailed result view and text sharing
- Option to withdraw consent from Settings

Measurements use Measurement Lab's service and are subject to its data-handling practices. Test history saved by the app remains on the device unless you choose to share it.

## Build

```bash
flutter pub get
flutter analyze
flutter test
flutter build apk --debug
```

GitHub Actions can produce an Android debug APK and an unsigned iOS build artifact. An unsigned iOS artifact is not a normal App Store or device-installable release.
