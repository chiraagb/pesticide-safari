# Pesticide for Safari (Unofficial Port)

This is a port of the "Pesticide - Advanced CSS Debugger" extension for Safari on macOS and iOS. It allows you to debug CSS layouts by outlining every element on the page.

## Prerequisites
* A Mac with macOS 11.0 (Big Sur) or later.
* **Xcode** (Free from the Mac App Store).

## How to Install & Run (macOS)

Since this is an open-source developer build, you must build it on your own machine.

### 1. Download
Clone this repository to your Mac:
```bash
git clone https://github.com/chiraagb/pesticide-safari.git
```

### 2. Open in Xcode
Double-click the file named `Pesticide - Advanced CSS Debugger.xcodeproj`.

### 3. Fix Signing (Required)
You must sign the app with your Apple ID to run it.
1.  In Xcode, click the **Project Name** (Blue icon) at the top of the left sidebar.
2.  Select the **"Signing & Capabilities"** tab in the center panel.
3.  In the "Targets" list on the left, you will see multiple targets. You must fix the signing for **macOS (App)** and **macOS (Extension)**:
    * Select the target.
    * Under "Team", select **Add an Account...** and log in with your Apple ID.
    * Select your **"Personal Team"**.
    * If you see a red error about "Bundle Identifier", add a random number to the end of the text (e.g. `com.yourname.pesticide.mac`).

### 4. Build and Run
1.  Click the **Scheme** menu (next to the Play button in the top left) and ensure **macOS (App)** is selected.
2.  Click the **Play Button** (▶️).
3.  The app will launch. Click "Open in Safari Extensions Preferences".

### 5. Enable in Safari
1.  In Safari, go to **Settings > Extensions**.
2.  Enable the **Pesticide** extension.
3.  *Troubleshooting:* If the extension doesn't appear, go to **Settings > Advanced** and check **"Show features for web developers"**, then check **"Allow Unsigned Extensions"** in the **Develop** menu.

## iOS / iPadOS Support
This project also contains targets for iOS. To run on a device, connect your iPhone to your Mac, select the **iOS (App)** scheme in Xcode, and press Play.

## Credits & Attribution

This project is an unofficial Safari port of the **Pesticide - Advanced CSS Debugger** Chrome Extension.

* **Original Concept:** [Pesticide](https://github.com/mrmrs/pesticide) by Paul Molluzzo (mrmrs).
* **Advanced Version:** [Pesticide - Advanced CSS Debugger](https://chromewebstore.google.com/detail/pesticide-advanced-css-de/jeebpgmphhagpecfiophljpkhncoajcg) by Extension Rocks.

All logic and CSS belong to the original authors; this repo merely repackages it as a Safari Web Extension.

