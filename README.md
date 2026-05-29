# Vibration App

[![Made with Kotlin](https://img.shields.io/badge/Made%20with-Kotlin-blue.svg)](https://kotlinlang.org/)
[![Made with Love](https://img.shields.io/badge/Made%20with-Love-red.svg)](https://shields.io/)
[![Android 8.1](https://img.shields.io/badge/Android-6.0-brightgreen.svg?logo=android)](https://developer.android.com/about/versions/marshmallow)


An Android application built with Jetpack Compose to explore and test haptic feedback through various vibration patterns and text-to-morse translation.

## Features

### 1. Vibration Presets (30 Patterns)
*   Includes a library of 30 distinct vibration patterns.
*   Features iconic rhythms like **"Shave and a Haircut"**.
*   Includes utility patterns like **SOS**, **Heartbeat**, **Gallop**, and various pulse speeds.
*   One-tap "Stop All" functionality to immediately cancel vibrations.

### 2. Text to Morse Code
*   A dedicated tab for custom vibrations.
*   Translates real-time text input into Morse code symbols (`.` and `-`).
*   Converts Morse code into tactile vibrations with standard timing:
    *   **Dot**: 150ms vibration.
    *   **Dash**: 450ms vibration.
    *   **Gaps**: Accurate intervals between characters and words.

## Implementation Details

*   **Language**: Kotlin
*   **UI Framework**: Jetpack Compose
*   **Navigation**: Horizontal Pager with TabRow for seamless swiping between features.
*   **API Support**: 
    *   Uses `VibratorManager` for Android 12+ (API 31).
    *   Uses `VibrationEffect` for Android 8.0+ (API 26).
    *   Backward compatibility for older devices.

## Permissions

The app requires the following permission in `AndroidManifest.xml`:
