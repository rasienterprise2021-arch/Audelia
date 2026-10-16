# Audelia Android project

This wraps the current Audelia HTML prototype in an Android WebView app. It is a starter/debug build, not a production release.

## Build APK

Requirements: JDK 17, Android SDK platform 35 and build tools, Gradle 8.9.

Run from this folder:

```bash
gradle assembleDebug
```

The APK is written to `app/build/outputs/apk/debug/app-debug.apk`.

## GitHub Actions build

Push this project to a GitHub repository, then open **Actions → Build Audelia APK → Run workflow**. Download `audelia-debug-apk` from the workflow run's Artifacts section.

## Prototype limitations

- This embeds the existing HTML prototype; it is not a complete production app.
- Login is a visual demo, with no real account/backend.
- Imported books and poster previews are currently session-only; persistence and full PDF/EPUB rendering are not implemented.
- This is a debug APK; a signed release APK requires a signing key and release configuration.
