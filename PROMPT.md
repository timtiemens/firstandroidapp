### Prompt: Bare-bones Android app that displays two colors (3s each)

You are an Android and Kotlin expert. Generate a minimal Android Studio project in Kotlin using Jetpack Compose that shows a full-screen color for 3 seconds, then switches to a second color for 3 seconds, then remains on the second color (no looping, no navigation).

Requirements:
- Min SDK 21, target the latest stable.
- Single-activity app (no fragments).
- Use Jetpack Compose.
- Use `LaunchedEffect` with coroutine `delay` for the 3-second timing.
- Package name: `com.example.twocolors`.
- Colors: first `Color.Red` for 3 seconds, then `Color.Blue`.
- Keep it truly bare bones: no unnecessary files, no theming beyond what’s required to compile, no comments.

Deliverables (output exact files with complete content):
- `settings.gradle.kts`
- `build.gradle.kts` (project)
- `app/build.gradle.kts` (module)
- `app/src/main/AndroidManifest.xml`
- `app/src/main/java/com/example/twocolors/MainActivity.kt`

Constraints:
- Output only code blocks for the files above in this order, with no extra explanation before, between, or after the code blocks.
- Ensure imports are complete and the project compiles as-is with Gradle.
- Use Compose to render a `Box` that fills the screen and sets its background color based on state; use a `LaunchedEffect` to wait 3 seconds, then change the color once.

Finally, include a short command-only section at the end with how to build and run via Gradle, as code blocks only:
- `./gradlew assembleDebug`
- `./gradlew installDebug`
