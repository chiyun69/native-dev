# 🧪 QA Testing

## Testing on Real Devices
- **Connect your iOS device via USB** and trust the computer.
- **Provisioning:**
  - Ensure your device UDID is added to the Apple Developer portal.
  - Use a valid development provisioning profile.
- **Build & Run:**
  - Use Xcode to build and run the app directly on the device.
  - For command-line install: `xcrun xcodebuild` or use `ios-deploy` for direct installation.
- **View device logs:**
  - Use Xcode's Devices and Simulators window or the `Console` app.


## Live Reload Testing
- **SwiftUI Previews:**
  - Use Xcode Previews for instant UI feedback as you edit SwiftUI code.
- **Hot Reload:**
  - Xcode automatically updates the preview canvas for SwiftUI changes.
  - For UIKit, use "Edit All in Scope" and Interface Builder for rapid UI iteration.
- **Limitations:**
  - Some changes (e.g., Info.plist, build settings, or deep logic changes) require a full rebuild and reinstall.
- **References:**
  - [SwiftUI Previews](https://developer.apple.com/documentation/swiftui/previews-in-xcode)
  - 


## TestFlight Distribution
- **TestFlight** allows you to distribute pre-release versions of your app to testers and gather feedback before App Store release.
- **Setup:**
  1. Testers receive an email invitation and install the TestFlight app from the App Store.
  2. Testers can install, update, and provide feedback directly through TestFlight.
  3. Testers can provide feedback directly to the team.

- **References:**
  - [Distribute an app using TestFlight](https://developer.apple.com/testflight/)
