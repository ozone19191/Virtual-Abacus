# Virtual Abacus

A Kotlin Android project for a Japanese soroban-style virtual abacus with a wood appearance, bead interactions, reset, multiple digit columns, and sound.

## Build

The easiest build route is the included GitHub Actions workflow. See [PHONE-ONLY-CLOUD-BUILD.md](PHONE-ONLY-CLOUD-BUILD.md) for instructions to build using only an Android phone.

For local builds, use Android SDK Platform 35, JDK 17, and Gradle 8.9, then run `gradle assembleDebug` from this directory.

The source project has not yet been compiled or device-tested; build and test the generated APK before relying on it.
