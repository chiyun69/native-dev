# ✅ Code Review & QA

## Review Checklist

### Critical
- No sensitive data (API keys, secrets) committed.
- Proper use of secure storage (e.g., Keychain, Encrypted Core Data) and permissions.
- Error handling for exceptions and edge cases.
- Remove/minimize debug logs in production; never log sensitive info.
- No unresolved merge conflict markers.
- Dependencies are up to date and free of known vulnerabilities.

### High
- Code style compliance (SwiftLint, formatting, naming conventions).
- Test coverage targets (unit, UI, snapshot tests).
- Avoid blocking the main thread (UI responsiveness).
- Performance: avoid memory leaks, retain cycles, unnecessary allocations, and main thread work.

### Medium
- No hardcoded strings (all user-facing strings are externalized in Localizable.strings).
- Accessibility: labels, traits, dynamic type, color contrast, VoiceOver support.
- Public functions/classes have documentation comments (/// or /** ... */).

