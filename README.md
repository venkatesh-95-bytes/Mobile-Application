# Workout Interval Timer

A lightweight mobile web app packaged as an Android app with Capacitor.

## Overview

This project uses:
- Vite for frontend bundling
- Capacitor for native Android packaging
- Android project in the `android/` folder

The app is configured in `capacitor.config.json` with the bundle output directory `dist` and the Android package ID `com.example.app`.

## Project Structure

```bash
.
├── android/                 # Android native project
├── dist/                    # Production build output
├── node_modules/            # Installed dependencies
├── www/                     # Static assets / web source root
├── capacitor.config.json    # Capacitor configuration
├── package.json             # NPM scripts and dependencies
├── vite.config.js           # Vite config
├── package-lock.json        # Lock file
└── README.md                # Project documentation
```

## Prerequisites

Before running the project, make sure you have:

- Node.js 18+ and npm
- Android Studio with Android SDK installed
- Java JDK (required for Android builds)
- An Android emulator or a connected Android device

## Installation

```bash
npm install
```

## Development

Start the Vite dev server:

```bash
npm run dev
```

This serves the app locally for web development.

## Production Build

Build the web app for production:

```bash
npm run build
```

This generates the static files in the `dist` folder.

## Android Sync and Run

Sync the web build with the Capacitor Android project:

```bash
npm run android:sync
```

Open the Android project in Android Studio:

```bash
npm run android:open
```

Run on an emulator or device:

```bash
npm run android:run
```

## Useful Commands

```bash
npm run dev          # start local development server
npm run build        # build web assets
npm run preview      # preview production build
npm run android:sync # sync Android project with web build
npm run android:open # open Android project in Android Studio
npm run android:run  # run app on Android device/emulator
```

## Notes

- The app is built as a web app first and then wrapped for Android using Capacitor.
- After changing app code, run `npm run build` and then `npm run android:sync` before testing in Android.
- If you change native Android code, open the project in Android Studio and build/run from there.

## License

This project does not currently include a license file. Add one if you plan to publish or distribute the app.
