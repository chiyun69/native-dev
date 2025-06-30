# 🏗️ App Architecture

## Recommended Patterns
- **MVVM** with `ViewModel`, `State`.
- **Clean Architecture** for large projects.

## Principles
- **Single Responsibility** per class/module.
- **Dependency Injection** via **Hilt**.
- **Coroutines/Flow** for async operations.

## Example
```
View (Compose)
  ↕️ (state)
ViewModel
  ↕️ (repository)
UseCases
  ↕️ (data sources)
```