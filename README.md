# Winter Arc Tracker – APK project

The app itself is www/index.html. Your ticks are saved on the phone and it works offline.

## Option A – build the APK in the cloud (no Android Studio needed)
1. Create a free GitHub account and a new repository.
2. Upload EVERYTHING in this folder, including the hidden ".github" folder (easiest from a computer: drag the folder contents into the repo page).
3. Open the repo's "Actions" tab -> "Build APK" -> wait about 5 minutes for the green tick.
4. Open the finished run, download the "WinterArcTracker-apk" file, unzip it, and you get app-debug.apk.
5. Send app-debug.apk to your phone, open it, and allow "Install unknown apps" when asked.

## Option B – build on your own computer
Needs Node.js 20+, Java 17 and Android Studio.
    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug        (on Windows: gradlew.bat assembleDebug)
The APK is at android/app/build/outputs/apk/debug/app-debug.apk

Note: this is a debug APK for personal use, not for the Play Store.
