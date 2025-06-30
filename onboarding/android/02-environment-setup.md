# ⚙️ Environment Setup

## Required Tools
- **Android Studio**
- **Gradle** (latest wrapper version)
- **ADB** (Android Debug Bridge)
- **Ktlint** for linting


## Lint and Formatter
- **Ktlint** for lint checks and formatting.
- **Detekt** for static code analysis.

### Ktlint Setup & Usage
- Add the plugin to your `build.gradle(.kts)` (project-level):
    ```Kotlin
    plugins {
        id("org.jlleitschuh.gradle.ktlint") version "12.1.0" apply false
    }
    ```

- Apply the plugin in your app/module `build.gradle(.kts)`:
    ```Kotlin
    plugins {
        id "org.jlleitschuh.gradle.ktlint"
    }
    ```

- Sync Gradle

- Ktlint is configured via `.editorconfig` file at the project root (rules are defined there).
    ```ini
    [*.{kt,kts}]
    indent_size=4
    max_line_length=120
    insert_final_newline=true
    ktlint_function_naming_ignore_when_annotated_with=Composable
    ktlint_standard_function-naming=disabled
    ```

- **Usage:**
  - Run lint checks: `./gradlew ktlintCheck`
  - Auto-format code: `./gradlew ktlintFormat`
- Ktlint will use the rules defined in `.editorconfig` automatically.

### Auto-format on Save in Android Studio
- To enable auto-format on save with Ktlint in Android Studio:
  1. Install the [Ktlint plugin for Android Studio](https://plugins.jetbrains.com/plugin/15041-ktlint) (Preferences → Plugins → Marketplace → search for "Ktlint").
  2. After installing, restart Android Studio.
  3. Go to **Preferences → Tools → Ktlint** and enable "Format on save".
  4. Now, every time you save a Kotlin file, Ktlint will automatically format it according to your `.editorconfig` rules.

