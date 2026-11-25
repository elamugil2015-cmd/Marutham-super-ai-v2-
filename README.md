# Marutham Super AI — Android starter project

This is a Kotlin + Jetpack Compose Android Studio starter for the app concept combining:
- AI chat interface
- Tamil/English-ready message UI
- Study, Robotics, Code and All AI modes
- Android speech-to-text input
- File picker attachment entry point
- Dark futuristic interface

## Important
This project is a UI prototype. It does **not** yet connect to OpenAI, Gemini, or another live AI model. The Send action currently displays a setup notice.

## Open and run
1. Install Android Studio (current stable version).
2. Choose **Open** and select this project folder.
3. Allow Gradle sync and install any requested Android SDK components.
4. Run on an Android phone or emulator.

To build an APK in Android Studio: **Build → Build Bundle(s) / APK(s) → Build APK(s)**.

## Next development stage
Add a secure backend API (recommended) that calls the selected AI provider. Do not put private OpenAI or Gemini API keys inside the Android app. The backend should expose an authenticated endpoint such as `POST /chat` and return the assistant response.

Suggested backend response shape:
```json
{ "reply": "Hello! How can I help?" }
```

Then replace the demo response in `MainActivity.kt` with an HTTPS request to that backend. Image understanding and PDF extraction should be implemented server-side or through dedicated Android libraries, with user consent for uploads.

## App identity
Name: Marutham Super AI
Application ID: `com.marutham.superai`
Minimum Android: 8.0 (API 26)
