# 📦 Dependency Management

## Preferred Tool: Swift Package Manager (SPM)
- Native integration with Xcode.
- Avoid CocoaPods where possible.

## Rules
- Version lock packages.
- Update dependencies quarterly.
- Define dependencies in `Package.swift`.

## Example
```
.package(url: "https://github.com/realm/realm-cocoa.git", from: "10.0.0")
```