# Quiz App

An Android quiz application developed as part of a collaborative academic assignment. The app retrieves trivia questions from the [Open Trivia Database](https://opentdb.com/), uses Firebase for account and score-related functionality, and presents individual and global score information.

> **Project context:** Group assignment. The contribution section below identifies the work I personally completed.

## Screenshots

> **Add your image:** Save a screenshot of the app's home or entry screen as `assets/screenshots/home-screen.png`, then replace this placeholder with `![Quiz app home screen](assets/screenshots/home-screen.png)`.

> **Add your image:** Save a screenshot showing a trivia question as `assets/screenshots/quiz-screen.png`, then replace this placeholder with `![Quiz question screen](assets/screenshots/quiz-screen.png)`.

> **Add your image:** Save a screenshot of the global leaderboard as `assets/screenshots/leaderboard.png`, then replace this placeholder with `![Global leaderboard](assets/screenshots/leaderboard.png)`.

> **Add your image:** Save a screenshot of the signed-in user's score as `assets/screenshots/individual-score.png`, then replace this placeholder with `![Individual score](assets/screenshots/individual-score.png)`.

## Features

- **Trivia questions:** Requests one question at a time from the Open Trivia Database API.
- **Account access:** Firebase-backed user login using a Google account.
- **Score tracking:** Records and retrieves quiz scores through Firebase.
- **Global scores:** Displays a global high-score view based on stored user scores.
- **Individual scores:** Displays the signed-in user's own score information.

The question request used by the application is based on:

```text
https://opentdb.com/api.php?amount=1
```

The endpoint requests one trivia question per API call. Refer to the [Open Trivia Database API documentation](https://opentdb.com/api_config.php) for available parameters and usage details.

## My Contribution

This was a group assignment. My main contributions were:

- Implementing the Firebase integration used by the application.
- Implementing the scoring system.
- Connecting score data to the individual score and global high-score views.

The application was developed collaboratively, so these contributions should not be interpreted as sole authorship of the entire project.

## Technology Stack

- **Platform:** Android
- **Language:** Confirm the application language from the source modules before adding a language badge.
- **Authentication and data:** Firebase
- **Trivia data source:** Open Trivia Database API
- **Build system:** Gradle

## Getting Started

### Prerequisites

- Android Studio with a compatible Android SDK.
- A compatible JDK configured for the project's Gradle version.
- Access to the Firebase project configuration required by the application.

### Open the Project

1. Clone or download this repository.
2. Open the repository root in Android Studio.
3. Add the Firebase configuration required for your authorised development environment.
4. Allow Gradle to sync and resolve dependencies.
5. Select an Android emulator or connected device and run the app.

### Build a Debug APK

On macOS or Linux:

```bash
./gradlew assembleDebug
```

On Windows:

```bat
gradlew.bat assembleDebug
```

The generated APK is normally placed under `app/build/outputs/apk/debug/`.

## Repository Layout

```text
.
├── app/                    # Android application module
├── gradle/wrapper/         # Gradle Wrapper files
├── assets/
│   └── screenshots/        # Add application screenshots here
├── build.gradle.kts        # Root build configuration
├── settings.gradle.kts     # Gradle project settings
├── gradlew                 # Gradle Wrapper (Unix-like systems)
└── gradlew.bat             # Gradle Wrapper (Windows)
```

## External Services

- [Open Trivia Database](https://opentdb.com/) provides trivia question data.
- [Firebase](https://firebase.google.com/) supports the application's account and score-related functionality.

Make sure any Firebase configuration files or secrets committed to a public repository are safe for public distribution. Never commit service-account keys or private credentials.

## Academic Context

This repository contains a group assignment. Add teammate names and a contribution breakdown only with their agreement.

## License

Add a `LICENSE` file if you intend to grant others permission to use, modify, or distribute this code. Until a licence is specified, do not assume that public visibility grants reuse rights.
