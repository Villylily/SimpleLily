# Simple Lily Development

Simple Lily is maintained by Villylily. Its Java sources retain legacy package and configuration identifiers for compatibility; the user-facing mod name is Simple Lily.

## Requirements

- Java Development Kit 25
- Minecraft 26.3 development dependencies, resolved by Gradle

## Build

From the project directory, run:

```powershell
.\gradlew.bat build
```

The distributable mod jar is written to `build/libs/`. To launch a development client, run:

```powershell
.\gradlew.bat runClient
```

On Linux or macOS, use `./gradlew` instead.

## Project layout

- `src/main/java/` contains the mod source.
- `src/main/resources/` contains Fabric metadata, mixin configuration, and assets.
- `build.gradle`, `settings.gradle`, and `gradle.properties` define the Gradle build.
- `gradle/wrapper/` and the Gradle wrapper scripts provide the pinned Gradle launcher.

## Dependencies and attribution

Fabric Loom resolves Minecraft, Fabric, Baritone, and other declared dependencies during the build. Do not upload generated `build/` or `.gradle/` directories as source.

This project includes work distributed under the MIT License. Preserve the repository's `LICENSE` file when redistributing source or binaries.
