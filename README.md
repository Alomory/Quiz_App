# Quiz App

An Android quiz application built as a collaborative academic project. It retrieves trivia questions from the [Open Trivia Database](https://opentdb.com/), supports Google sign-in through Firebase Authentication, and records scores for individual results and a global leaderboard.

## Screenshot/s

![Quiz app home screen](https://alomory.com/img/quiz-app.png)


## Features

- Fetch trivia questions from the Open Trivia Database.
- Sign in using a Google account with Firebase Authentication.
- Calculate and store quiz scores.
- View individual scores and a global leaderboard.

The app requests one question per API call:

```text
https://opentdb.com/api.php?amount=1
```

## Technology

- Kotlin
- Android and Jetpack Compose
- Firebase Authentication
- Firebase database services
- Open Trivia Database
- Gradle

## Run locally

**Requirements:** Android Studio, JDK 17, Android SDK, an Android emulator or device, and internet access.

1. Clone the repository and open its root directory in Android Studio.
2. Add a Firebase Android app matching the application ID configured in the project.
3. Enable Google as a sign-in provider in Firebase Authentication.
4. Configure the Firebase database used by the app.
5. Add the Firebase `google-services.json` file to the `app/` directory.
6. Configure the SHA certificate fingerprint in Firebase if required for Google sign-in.
7. Sync the project with Gradle and run the `app` configuration.

Do not commit private keys, service-account credentials, or signing secrets.

### Build a debug APK

Run the Gradle Wrapper from the repository root.

**Windows PowerShell**

```powershell
.\gradlew.bat :app:assembleDebug
```

**macOS / Linux**

```bash
./gradlew :app:assembleDebug
```

The APK is generated at `app/build/outputs/apk/debug/app-debug.apk`.

## Project structure

The Android app module contains the application source, resources, and tests. Main Kotlin code is grouped by feature and UI concern.

```text
app/src/
├── main/
│   ├── java/com/example/quizapp/
│   │   ├── profile/
│   │   ├── sign_in/
│   │   └── ui/theme/
│   └── res/
├── test/
└── androidTest/

gradle/wrapper/
```

## Contribution

This project was developed as a group assignment. My contributions focused on the Firebase integration and the quiz scoring system, including the score data used for individual results and the global leaderboard.

## License

Distributed under the MIT License. See [LICENSE](LICENSE).
