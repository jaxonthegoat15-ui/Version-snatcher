# Version Snatcher (Quest 3 / 3S)

Opens a game APK, shows its Unity editor version, and extracts `.so`, `.dll` and `global-metadata.dat`
into `Downloads/VersionSnatcher` on the headset.

## Build the APK with GitHub
1. Create a new GitHub repo and upload everything in this folder (keep the `.github` folder).
2. Open the **Actions** tab. The "Build APK" workflow runs on every push (or press "Run workflow").
3. When it finishes, open the run and download the **VersionSnatcher-apk** artifact (a zip containing `app-debug.apk`).

## Install on Quest
Enable developer mode, then: `adb install app-debug.apk`
(or use SideQuest). Find it under Unknown Sources in the app library.

## Editing the UI
All of the UI lives in `app/src/main/assets/index.html`.
