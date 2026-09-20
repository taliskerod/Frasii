# Frasi (Android)

Offline Italian sentence trainer: type English, get Italian automatically (on-device Google ML Kit),
organize sentences into groups, and play them hands-free or as flashcards with active-recall sets.

## Build the APK (no Android Studio needed)

1. Create a **private** repository on github.com (for example `frasi`).
2. Upload everything in this folder, including the hidden `.github` folder and `keystore/`.
   Easiest way: on the new repo page choose "uploading an existing file" and drag the whole folder in,
   or use GitHub Desktop.
3. Open the repo's **Actions** tab. The "Build APK" workflow runs on every push to `main`
   (you can also start it with "Run workflow"). It takes about 5 to 8 minutes.
4. When it's green, open **Releases** on the repo page and download `Frasi.apk` on your phone.
5. Install it. Android will ask you to allow installs from your browser or file manager once.

To update the app later, change a file, push, and install the new APK over the old one.
Your sentences are kept because every build is signed with the same key in `keystore/`.
Keep the repo private so that key stays yours.

## First run on the phone

- Connect to Wi-Fi once so the Italian translation model (about 30 MB) can download.
  After that, translation works fully offline.
- In Settings, pick your Italian and English female and male voices. Tap "Install voice data"
  if Italian voices are missing, and prefer voices not marked "network" for offline use.
- Use Settings, Backup, "Copy backup" now and then. Uninstalling the app deletes your data.
