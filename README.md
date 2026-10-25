# iOS 26 Glass Launcher (Android project)

This is a native Android Studio source project for a launcher-style home screen.

## Included
- Android HOME + DEFAULT intent filter so Android can offer it as a default home app.
- Queries and lists launchable apps, their real icons, tap-to-launch.
- Search by installed app label.
- Glass-inspired translucent cards, gradient wallpaper, clock/date, dock.
- Arabic UI labels; no special permissions requested.

## Build an APK
1. Open this folder in Android Studio (recent version).
2. Allow Gradle sync and install Android SDK Platform 35 if prompted.
3. Use Build > Build Bundle(s) / APK(s) > Build APK(s).
4. The debug APK is normally created at `app/build/outputs/apk/debug/app-debug.apk`.
5. Transfer the APK to your Android phone and install it. Android may ask you to allow installs from that source.
6. Press Home and choose **Glass Launcher**. To change later, use Android Settings > Apps > Default apps > Home app.

## Important
This is project source, not a compiled APK. It has not been built or tested on a physical device in this environment because Android SDK/Gradle build tools are unavailable here. Target SDK 35 and Android package visibility behavior may vary by device; test app enumeration and default-home selection on your Android version. The weather and Wi-Fi status visuals are decorative placeholders, not live data. This is an iOS-inspired design and does not include Apple's proprietary assets.

## Build using only your phone (GitHub cloud build)
This project includes `.github/workflows/build.yml` so GitHub can compile the APK in the cloud.
1. In your phone browser, sign in to GitHub and create a new repository.
2. Upload the *contents* of this ZIP into the repository (extract the ZIP first in your phone's Files app).
3. Open the repository's Actions tab and select **Build Android APK**.
4. Tap **Run workflow** (if it did not run automatically after upload).
5. When the run finishes, open it and download the artifact named `iOS26-Glass-Launcher-APK`.
6. Extract the artifact ZIP to get `app-debug.apk`, then install it on your phone.
The workflow has been added but has not been run here; successful compilation is not yet verified.
