# 🔐 Security & Privacy

## Secure Storage
- Never store sensitive data in plain text or in external storage.
- Use the **Android Keystore System** for cryptographic keys and operations:
  - Generate and store keys securely in the Keystore.
  - Use keys from the Keystore for encryption/decryption, signing, and authentication.
  - [Keystore documentation](https://developer.android.com/training/articles/keystore)
- Avoid storing sensitive information in logs, cache, or clipboard.
- Regularly audit storage locations for sensitive data leaks.
- For files, use internal app storage with proper file permissions and encryption if needed.
- Remove sensitive data from storage as soon as it is no longer needed.
- References:
  - [Android Keystore System](https://developer.android.com/training/articles/keystore)
  - [Best Practices for Storing Data](https://developer.android.com/topic/security/best-practices#storing-data)

## Permissions
- Request permissions at runtime using the Android permissions API.
- Explain why permissions are needed with clear, user-friendly dialogs before the system prompt.
- Only request permissions that are essential for app functionality.
- Handle permission denial gracefully and provide alternative flows if possible.
- Regularly review and minimize the list of requested permissions.
- Use the [Android permissions best practices](https://developer.android.com/training/permissions/requesting) to avoid unnecessary permission requests.
- For sensitive permissions (location, camera, microphone, storage):
  - Provide just-in-time explanations (rationale) using `shouldShowRequestPermissionRationale`.
  - Respect user choices and do not repeatedly prompt after denial.
  - For background location, request foreground location first, then background if needed.
- For special permissions (e.g., SYSTEM_ALERT_WINDOW, WRITE_SETTINGS), guide users to the appropriate settings screen.
- Document all permissions in your privacy policy.
- References:
  - [Request App Permissions](https://developer.android.com/training/permissions/requesting)
  - [Permission Rationale Best Practices](https://developer.android.com/training/permissions/usage-notes)
  - [Android Permission Groups](https://developer.android.com/reference/android/Manifest.permission)

## Data Protection
- Adhere to GDPR, CCPA.
- Minimize sensitive data collection.
- Only collect and store data that is strictly necessary for app functionality.
- Use data anonymization and pseudonymization where possible.
- Secure data in transit using HTTPS (TLS/SSL).
- Secure data at rest using encryption.
- Provide users with clear privacy policies and obtain explicit consent for data collection.
- Allow users to access, modify, or delete their personal data upon request.
- Regularly review and audit data access and storage practices.
- Implement data retention policies and securely delete data when no longer needed.
- Monitor for and respond to data breaches in accordance with legal requirements.
- Keep third-party SDKs and dependencies up to date and review their privacy practices.
- References:
  - [GDPR Compliance for Android](https://developer.android.com/topic/security/best-practices#gdpr)
  - [Android Data Safety](https://support.google.com/googleplay/android-developer/answer/10787469)
  - [Best Practices for User Data](https://developer.android.com/topic/security/best-practices)