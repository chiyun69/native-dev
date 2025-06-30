# 🧪 QA Testing


## Testing on Real Devices with ADB
- **Connect your Android device via USB** and enable Developer Options and USB Debugging:
  1. On your device, go to **Settings → About phone** and tap **Build number** 7 times to enable Developer Options.
  2. In **Settings → Developer options**, enable **USB debugging**.
- **Verify device connection:**
  ```sh
  adb devices
  ```
  - Your device should appear in the list. If not, check your cable, drivers, and permissions.
- **Install an APK on the device:**
  ```sh
  adb install path/to/your-app.apk
  ```
- **Uninstall an app:**
  ```sh
  adb uninstall com.your.package.name
  ```
- **View device logs:**
  ```sh
  adb logcat
  ```
- **Screen mirroring (optional):**
  - Use [scrcpy](https://github.com/Genymobile/scrcpy) for real-time device screen mirroring and control from your computer.
  - **Installation on macOS:**
    ```sh
    brew install scrcpy
    ```
  - **Basic usage:**
    1. Connect your device via USB and ensure it is detected by `adb devices`.
    2. Start scrcpy:
       ```sh
       scrcpy
       ```
    3. The device screen will appear in a window. You can interact with it using your mouse and keyboard.
  - **Features:**
    - High performance, low latency mirroring.
    - Supports screen recording: `scrcpy --record file.mp4`
    - Wireless mode: Connect your device over Wi-Fi (after initial USB setup) and run `scrcpy` as usual.
    - Copy-paste and file drag-and-drop support.
  - **More options:** See the [scrcpy documentation](https://github.com/Genymobile/scrcpy#usage) for advanced features and command-line options.
- **Wireless ADB (optional):**
  1. Connect your device via USB and run:
     ```sh
     adb tcpip 5555
     adb connect <device-ip-address>:5555
     ```
  2. Disconnect USB. Your device is now connected over Wi-Fi.

## Live Reload Testing
- **Live reload** allows you to see code and UI changes instantly on your device or emulator without reinstalling the app each time.
- **Android Studio Hot Reload:**
  - When using Jetpack Compose, Android Studio supports "Apply Changes" and "Live Edit" for rapid UI iteration.
  - **Apply Changes:**
    - Click the "Apply Changes and Restart Activity" button (or use shortcut: `Ctrl+Alt+F10` / `Cmd+Ctrl+R` on macOS) to push code and resource changes to the running app without a full reinstall.
  - **Live Edit (Compose only):**
    - Enable Live Edit in Android Studio (Settings → Experimental → Live Edit) to see Compose UI changes reflected instantly as you type.
    - Works best for UI and preview changes; not all code changes are supported.
  - **Limitations:**
    - Some changes (e.g., manifest, Gradle, or deep logic changes) still require a full rebuild and reinstall.
- **References:**
  - [Apply Changes and Live Edit (Official Docs)](https://developer.android.com/studio/run#apply-changes)


## Firebase App Distribution
- **Firebase App Distribution** allows you to quickly distribute pre-release versions of your app to testers and gather feedback before releasing to production.
- **Tester Setup:**
  1. Testers will receive an email invitation from Firebase App Distribution.
  2. On their Android device, testers must:
     - Open the invitation email and tap the download link.
     - Sign in with the email address that was invited.
     - Download and install the app directly from the link.
     - If prompted, enable installation from unknown sources (Settings → Security → Install unknown apps → Allow from this source).
  3. For updates, testers will receive new email notifications or can use the Firebase App Tester app (if enabled).
  4. Testers can provide feedback or report issues directly through the Firebase App Distribution interface.


## Play Store Internal Testers
- **Play Store Internal Testing** allows you to quickly distribute your app to a small group of trusted testers via the Google Play Console before releasing to a wider audience.
  
- **Tester Experience:**
  - Testers receive an email invitation with a Play Store link to download the app.
  - They must accept the invitation and use a Google account included in the tester list.
  - Updates are delivered via the Play Store like a normal app update.
  - Testers can provide feedback directly to the team.


