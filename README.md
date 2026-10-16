# Misa (Android)

## Build the APK in the cloud (no Android Studio needed)
1. Create a new GitHub repo and upload everything in this folder (including the hidden .github folder).
2. Open the repo's Actions tab, pick "Build Misa APK", tap Run workflow.
3. When it finishes (about 5 minutes), download the "misa-apk" artifact, unzip it, and install app-debug.apk on your phone (allow "install unknown apps").

## Build locally instead
npm install && npx cap add android
Add RECORD_AUDIO and MODIFY_AUDIO_SETTINGS permissions to android/app/src/main/AndroidManifest.xml
npx cap sync android && npx cap open android

## First run
Open Misa, expand Settings, paste your Anthropic API key (console.anthropic.com), tap Save, allow the microphone, then turn on Always listening and say "Hey Misa".
