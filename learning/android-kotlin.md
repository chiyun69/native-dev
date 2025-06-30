# Android Jetpack Compose

This guide provides a structured and practical roadmap for mastering Jetpack Compose and Kotlin, Android’s modern toolkit for building native user interfaces. Whether you are a beginner or an experienced developer, this resource will help you understand core concepts, best practices, and advanced techniques for building robust, efficient, and beautiful Android apps with Compose.

---

> **Example Project:**
> For a comprehensive, real-world example covering all topics in this guide, see the open-source repository: [Learning_JetpackCompose (GitHub)](https://github.com/chiyun69/Learning_JetpackCompose)

---

## 1. Basics of Jetpack Compose

- **Understand Declarative UI**  
  Learn how Compose differs from the traditional View-based system by focusing on building UI with declarative programming.
- **Setup Environment**  
  Install Android Studio (latest version) and configure the project for Jetpack Compose.
- **Composables**  
  Explore `@Composable` functions to create UI elements and understand UI hierarchy.
- **Previewing UIs**  
  Use the `@Preview` annotation to visualize your UI within Android Studio.
- **References:**
  - [Jetpack Compose Overview](https://developer.android.com/jetpack/compose)
  - [Set up Jetpack Compose](https://developer.android.com/jetpack/compose/setup)
  - [Compose Pathway (Codelabs)](https://developer.android.com/courses/pathways/compose)
  - [Compose Basics](https://developer.android.com/jetpack/compose/tutorial)

---

## 2. Building UI Components

- **Basic Composables**  
  Text, Button, Image, Column, Row, Box, etc.
- **Modifiers**  
  Styling, padding, size, and interactions.
- **Alignment and Arrangement**
- **Lists and Grids**
- **Constraints**
- **References:**
  - [Compose Layouts](https://developer.android.com/jetpack/compose/layouts)
  - [Compose Modifiers](https://developer.android.com/jetpack/compose/modifiers)
  - [Compose Foundation Components](https://developer.android.com/reference/kotlin/androidx/compose/foundation/package-summary)
  - [Compose Material Components](https://developer.android.com/reference/kotlin/androidx/compose/material/package-summary)

---

## 3. Layouts and Design

- **Layouts**  
  Master layout composables such as Column, Row, Box, LazyColumn, and LazyRow.
- **Containers**
- **ConstraintLayout**  
  Use ConstraintLayout for more complex UI designs.
- **Material Design in Compose**
- **Theming**  
  Create custom themes, typography, and color palettes in Compose.
- **References:**
  - [Layouts in Compose](https://developer.android.com/jetpack/compose/layouts/basics)
  - [ConstraintLayout in Compose](https://developer.android.com/jetpack/compose/layouts/constraintlayout)
  - [Material Design Components](https://developer.android.com/jetpack/compose/material)
  - [Theming in Compose](https://developer.android.com/jetpack/compose/themes)

---

## 4. Navigation and Routing

- **Navigation Basics with Jetpack Compose**
- **Building Navigation Graphs**
- **Passing Data Between Screens**  
  Using arguments.
- **Deep Linking and Navigation Actions**
- **References:**
  - [Navigation in Compose](https://developer.android.com/jetpack/compose/navigation)
  - [Navigation Compose Library](https://developer.android.com/jetpack/compose/navigation-library)
  - [Deep Links in Compose](https://developer.android.com/jetpack/compose/navigation#deeplinks)

---

## 5. User Input and Interactions

- **Handling User Input Events**
- **State Management in Compose**
- **References:**
  - [User Input in Compose](https://developer.android.com/jetpack/compose/text/user-input)
  - [State in Compose](https://developer.android.com/jetpack/compose/state)
  - [Gestures in Compose](https://developer.android.com/jetpack/compose/gestures)

---

## 6. State and Side-Effects

- **State Hoisting**  
  Separate state management from composables for better reusability.
- **Managing App State with Mutable State**
- **Using ViewModels and LiveData in Jetpack Compose**
- **Unidirectional Data Flow in Compose**
- **Side Effects**  
  Understand side effects with functions like `LaunchedEffect`, `DisposableEffect`, and `rememberCoroutineScope`.
- **References:**
  - [State and Side-effects in Compose](https://developer.android.com/jetpack/compose/state)
  - [Side-effects in Compose](https://developer.android.com/jetpack/compose/side-effects)
  - [ViewModel in Compose](https://developer.android.com/jetpack/compose/state#viewmodel)

---

## 7. Working with ViewModels

- **MVVM Architecture**  
  Integrate ViewModel with Jetpack Compose.
- **LiveData & StateFlow**  
  Manage reactive data streams with LiveData and StateFlow in Compose.
- **Passing Data Between Screens Using ViewModels**
- **References:**
  - [ViewModel and Compose](https://developer.android.com/jetpack/compose/state#viewmodel)
  - [LiveData and Compose](https://developer.android.com/topic/libraries/architecture/livedata)
  - [StateFlow and Compose](https://developer.android.com/kotlin/flow/stateflow-and-sharedflow)
  - [MVVM on Android](https://developer.android.com/jetpack/guide)

---

## 8. API Requests

- **Ktor**  
  A framework for building asynchronous server-side and client-side applications with ease.
- **Caching and Offline Capabilities**
- **References:**
  - [Ktor Client Guide](https://ktor.io/docs/getting-started-ktor-client.html)
  - [Networking in Compose](https://developer.android.com/jetpack/compose/networking)
  - [Retrofit (Alternative)](https://square.github.io/retrofit/)

---

## 9. Data Storage Locally

- **Data Storage with SharedPreferences**
- **Persisting Data with Room**  
  DAOs, Entities.
- **References:**
  - [Data Storage Options](https://developer.android.com/training/data-storage)
  - [Room Persistence Library](https://developer.android.com/jetpack/androidx/releases/room)
  - [SharedPreferences](https://developer.android.com/training/data-storage/shared-preferences)

---

## 10. Dependency Injection

- **Hilt**
- **References:**
  - [Dependency Injection on Android](https://developer.android.com/training/dependency-injection)
  - [Hilt Documentation](https://developer.android.com/training/dependency-injection/hilt-android)
  - [Dagger (Underlying Library)](https://dagger.dev/)

---

## 11. Animations and Motion

- **Basic Animations**  
  Use `animate*AsState` for simple animations (e.g., `animateFloatAsState`).
- **Advanced Animations**  
  Explore `AnimatedVisibility`, transitions, and custom animations.
- **Complex Motion Behaviors and Choreography**
- **References:**
  - [Animations in Compose](https://developer.android.com/jetpack/compose/animation)
  - [Animation APIs](https://developer.android.com/reference/kotlin/androidx/compose/animation/package-summary)
  - [MotionLayout in Compose](https://developer.android.com/jetpack/compose/layouts/motionlayout)

---

## 12. Testing and Debugging

- **UI Testing**  
  Use `ComposeTestRule` and Espresso for UI tests.
- **Unit Testing**  
  Write unit tests for composables and business logic.
- **Debugging Jetpack Compose Apps**
- **Using the Layout Inspector and Hierarchy Viewer**
- **References:**
  - [Testing in Compose](https://developer.android.com/jetpack/compose/testing)
  - [Debugging Compose](https://developer.android.com/jetpack/compose/tooling)
  - [Espresso Testing](https://developer.android.com/training/testing/espresso)
  - [Layout Inspector](https://developer.android.com/studio/debug/layout-inspector)

---

## 13. Performance Optimization

- **Recomposition**  
  Understand what causes recomposition and how to avoid unnecessary recompositions.
- **Performance Tips**  
  Optimize performance with `DerivedStateOf` and `remember`.
- **Optimizing Layouts and Lists**
- **Android Studio Profiler**
- **References:**
  - [Performance in Compose](https://developer.android.com/jetpack/compose/performance)
  - [Recomposition in Compose](https://developer.android.com/jetpack/compose/performance#recomposition)
  - [Android Studio Profiler](https://developer.android.com/studio/profile)

---

## 14. Advanced Topics

- **Permissions on Android**
- **Custom Composables**  
  Build your own custom UI components.
- **Effect Handlers**  
  Dive into advanced side-effect handling.
- **Custom Layouts**  
  Create custom layout composables for complex designs.
- **Advanced Animation Techniques**
- **Jetpack Libraries**  
  (ViewModel, LiveData, Room, WorkManager)
- **References:**
  - [Permissions on Android](https://developer.android.com/training/permissions/requesting)
  - [Custom Layouts in Compose](https://developer.android.com/jetpack/compose/layouts/custom)
  - [Effect Handlers](https://developer.android.com/jetpack/compose/side-effects)
  - [Advanced Animation](https://developer.android.com/jetpack/compose/animation/advanced)
  - [Jetpack Libraries](https://developer.android.com/jetpack)

---
