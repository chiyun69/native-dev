# 📏 Coding Standards

## Naming Conventions
- Classes/Structs/Enums: `PascalCase`
- Variables/Properties: `camelCase`
- Constants: `UPPER_SNAKE_CASE`
- Protocols: End with `Protocol`

## Modularity
- Feature-based modules.
- Shared utilities in `Core` module.

## Swift Best Practices
- Avoid force unwraps (`!`).
- Use dependency injection.
- Write unit tests alongside new code.

## SwiftUI UI Guidelines
- Use `@State`, `@Binding`, `@ObservedObject` properly.
- Keep views small and composable.
- Prefer `NavigationStack` over deprecated `NavigationView`.