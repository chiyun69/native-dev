# 📦 Dependency Management

## Preferred Tool: Gradle
- Version catalog via `libs.versions.toml`.
- Enforce dependency rules in `build.gradle.kts`

## Example
```
implementation(libs.androidx.core.ktx)
implementation(libs.hilt)
```