# Flag Smashers (country flag battle game)

Game code: `www/index.html` (single file, works offline). Open it in any phone browser to play right now.

## Get the APK (pick one)

**A. No setup, in the cloud (GitHub Actions)**
1. Create a new GitHub repo and upload this whole folder (keep the `.github` folder).
2. Open the repo's *Actions* tab -> *Build APK* -> wait ~5 minutes.
3. Download `FlagSmashers-apk` from the finished run, unzip it, install `app-debug.apk` on your phone (allow "install unknown apps").

**B. On your own computer** (needs Node 18+, JDK 17, Android Studio / SDK)
```
npm install
npx cap sync android
cd android && ./gradlew assembleDebug
```
APK: `android/app/build/outputs/apk/debug/app-debug.apk`

Change the game, then run `npx cap sync android` and rebuild.
