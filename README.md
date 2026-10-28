# Simple Music Player App

A lightweight and modern Android music player built with **Kotlin** and **XML**, designed to play local audio tracks with a clean user interface, album art display, real-time progress tracking, and interactive playback controls.

---

## Features
* **Local Audio Playback:** Seamlessly plays local `.mp3` tracks bundled inside the app resources (`res/raw`).
* **Interactive Media Controls:** Play, pause, and seek through tracks using a responsive progress bar (`SeekBar`).
* **Dynamic UI & Metadata:** Displays song titles, artist names, and custom album artwork.
* **Live Time Tracking:** Automatically updates current playback time and total duration.

---

## Tech Stack & Environment
* **Language:** Kotlin
* **UI:** XML Layouts, Material Components, ConstraintLayout
* **Core Components:** `MediaPlayer`, `Handler`, `SeekBar`, `ImageView`
* **Target SDK:** API Level 34 (Android 14)
* **Minimum SDK:** API Level 24 (Android 7.0)
* **Build System:** Gradle (`build.gradle.kts`)

---

## Project Structure
```text
Simple_music_Player_UI/
│
├── app/
│   ├── src/main/
│   │   ├── java/com/example/simplemusicplayerui/
│   │   │   └── MainActivity.kt       # Core playback & UI binding logic
│   │   ├── res/
│   │   │   ├── drawable/             # Album art & vector assets
│   │   │   ├── layout/               # activity_main.xml UI layout
│   │   │   ├── raw/                  # Local audio files (e.g., senjitaley.mp3)
│   │   │   └── values/               # Themes, colors, and strings
│   │   └── AndroidManifest.xml       # App manifest configuration
│   │
│   └── build.gradle.kts              # App-level build script
└── build.gradle.kts                  # Project-level build script

# How to Run the App

Follow these steps to run the Simple Music Player app on your Android Studio emulator or physical Android device:

---

## 1. Prerequisites Check
* Ensure **Android Studio** is open and the Gradle sync has completed successfully.
* Ensure your audio file is placed at `app/src/main/res/raw/senjitaley.mp3`.
* Ensure your image file is placed at `app/src/main/res/drawable/senjitaley_poster.jpg`.

---

## 2. Option A: Running on an Emulator (Virtual Device)
1. In the top toolbar of Android Studio, click the **Device Manager** icon (or go to **Tools > Device Manager**).
2. Click **Create Device** if you do not have an active emulator.
3. Select a phone model (e.g., **Pixel 6** or **Pixel 7**) and click **Next**.
4. Choose a system image (e.g., **API 34 / Android 14**) and click **Finish**.
5. Select your newly created emulator from the target device dropdown menu next to the green **Play (▶)** button.
6. Click the green **Play (▶) / Run 'app'** button (or press `Shift + F10`).

---

## 3. Option B: Running on a Physical Android Phone
1. On your Android phone, go to **Settings > About Phone** and tap **Build Number** 7 times to enable **Developer Options**.
2. Go back to **Settings > System > Developer Options** and turn on **USB Debugging**.
3. Connect your phone to your laptop/PC using a USB cable.
4. If a prompt appears on your phone screen asking to allow USB debugging, tap **Allow**.
5. In Android Studio, select your physical device name from the target device dropdown menu in the top toolbar.
6. Click the green **Play (▶) / Run 'app'** button (or press `Shift + F10`).

---

## 4. Troubleshooting Steps
If you run into build issues before launching:
1. Go to the top menu and select **Build > Clean Project**.
2. Once finished, select **Build > Rebuild Project**.
3. Click **Sync Project with Gradle Files** from the top right toolbar if prompted.
4. Click **Run** again.
