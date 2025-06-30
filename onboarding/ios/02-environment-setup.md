# ⚙️ Environment Setup

## Required Tools
- **Xcode** (latest stable release via App Store)
- **Swift Package Manager** (integrated into Xcode)
- **CocoaPods** (for legacy projects)
- **Homebrew** (optional but recommended for installing tools like SwiftLint, SwiftFormat, etc.)
- **Simulator** (iOS, iPadOS, watchOS, tvOS simulators included with Xcode)
- **Fastlane** (for automating builds, tests, and distribution)


## Lint and Formatter
- **SwiftLint**: Enforce style and conventions. Install via Homebrew:
  ```sh
  brew install swiftlint
  ```
  - Integrate with Xcode as a build phase for automatic linting.
  - Configure rules in `.swiftlint.yml` at the project root.
- **SwiftFormat**: Auto-formatting Swift code. Install via Homebrew:
  ```sh
  brew install swiftformat
  ```
  - Can be run manually or as a pre-commit hook.
  - Configure rules in `.swiftformat` at the project root.
  - **To run SwiftFormat manually on your project:**
    ```sh
    swiftformat .
    ```
    This will format all Swift files in the current directory and subdirectories according to your configuration.

## Recommended Xcode Settings
- Enable "Treat Warnings as Errors" for stricter code quality.
- Use "New Build System" (default in recent Xcode versions).
- Set up code signing and provisioning profiles for all targets.
- Enable "Enable Test Coverage" in the scheme for code coverage reports.

## Pre-commit Hooks (Optional)
> **WORK IN PROGRESS:** This section is under review and will be refined later.
