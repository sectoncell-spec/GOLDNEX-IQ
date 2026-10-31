# GOLDNEX IQ Android floating shortcut

## Build APK in the cloud (no Android Studio needed on your phone)

1. Download this ZIP and extract it.
2. Create a GitHub repository at https://github.com/new.
3. Upload the extracted project files and folders to the repository (keep the `.github/workflows/android.yml` folder).
4. Open the repository's **Actions** tab.
5. Select **Build GOLDNEX IQ APK** and tap **Run workflow** (or wait for the first push build).
6. When the workflow finishes, open its run and download the **GOLDNEX-IQ-debug-apk** artifact.
7. Extract the downloaded artifact ZIP; inside is `app-debug.apk`.
8. Transfer `app-debug.apk` to your Android phone, open it, and allow installation from that source if Android asks.

## App behavior
- Creates a draggable floating GOLDNEX shortcut after the user grants Android's overlay permission.
- The floating button opens the GOLDNEX app.
- Includes an IQ Option launcher attempt using common Android package IDs; app package names may vary, so IQ Option may need to be opened manually.
- It does not inspect IQ Option, automate screen taps, or execute trades.

## Important
This is a debug APK built from source, not a Play Store release. Only install APKs you built yourself or trust. The floating button requires the user to explicitly grant “Display over other apps.” The cloud build requires a GitHub account and the user to upload the source repository and start the workflow.
