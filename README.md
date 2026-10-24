# San Paloma Android project

This is an Android Studio project wrapping the included San Paloma: Street Run HTML5 game in an offline Android WebView.

## Build an APK with Android Studio
1. Open this folder in Android Studio.
2. Allow it to install the required Android SDK (API 35) and Gradle components.
3. Choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. The debug APK will be at `app/build/outputs/apk/debug/app-debug.apk`.

## Build using GitHub Actions
1. Create a new GitHub repository and upload/push all files in this folder.
2. Open the repository's **Actions** tab.
3. Run **Build San Paloma APK** (or push to `main`/`master`).
4. Download the `San-Paloma-debug-APK` artifact from the completed workflow run. It contains `app-debug.apk`.

The APK built by this workflow is a debug APK suitable for testing/sideloading. It is not Play Store-signed.

## Game
The game runs offline and uses on-screen touch controls. The original ZIP's configuration files are preserved separately in the previous project archive; the original archive did not include the original game's source entry point or assets, so this Android project packages the newly created Street Run starter game.
