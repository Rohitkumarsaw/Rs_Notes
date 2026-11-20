# RS Notes

**Privacy-first, fully offline note-taking for Android.**
No account. No ads. No analytics. No `INTERNET` permission. Your notes never leave your device.

![Version](https://img.shields.io/badge/version-1.2.1-cyan) ![Android](https://img.shields.io/badge/Android-7.0%2B-green) ![Offline](https://img.shields.io/badge/100%25-offline-blue) ![License](https://img.shields.io/badge/license-freeware-lightgrey)

---

## ✨ Features

- **100% offline** — works in airplane mode; nothing is uploaded or synced
- **4-digit PIN lock** — keep private notes behind a quick local PIN gate
- **Full-screen editor** — distraction-free writing (new in `1.2.1`)
- **`.txt` export** — save any note straight to Downloads, no permissions required (new in `1.2.1`)
- **Instant search** — filter notes by title or body as you type
- **Light & dark themes** — easy on the eyes, day or night
- **Pin & colour notes** — keep the important ones on top
- **Zero ads, zero tracking** — no third-party SDKs, no cloud, no telemetry

---

## 📸 Screenshots

| Home (dark) | Editor | PIN lock |
|---|---|---|
| ![Home](screenshots/home_dark.jpg) | ![Editor](screenshots/editor.jpg) | ![PIN](screenshots/pin_lock.jpg) |

| Search | Light mode |
|---|---|
| ![Search](screenshots/search.jpg) | ![Light](screenshots/light_mode.jpg) |

---

## 📥 Download

> **Repo owner:** replace the placeholder links below before publishing.

| Source | Link |
|---|---|
| Direct APK (universal) | `YOUR_APK_URL` |
| Uptodown | `YOUR_UPTODOWN_URL` |
| Google Play | `YOUR_PLAY_URL` |

**Version:** `1.2.1` · **Size:** `51.43 MB` · **Android:** `7.0+` · **Architectures:** `arm64-v8a`, `armeabi-v7a`, `x86_64`

The APK is **universal** — it runs on virtually every modern Android device, including x86 emulators.

---

## 🛠️ Install (from APK)

1. Download `RS_Notes_v1.2.1_universal.apk`
2. Open the file; allow **Install unknown apps** for your browser when prompted
3. Install, then set your optional 4-digit PIN
4. Start writing — no sign-in, no setup wizard

> Updating from an older version? Keep a copy of your notes first, then install over the existing app. If the installer reports a signature conflict, uninstall the old version first (this deletes local notes).

---

## 🔐 Privacy & permissions

RS Notes contains **no `INTERNET` permission**. It cannot send data anywhere.

| What stays on device | What is never collected |
|---|---|
| Notes and titles | Personal data |
| PIN preference | Analytics / crash reports |
| Theme and app settings | Ad identifiers |
| Exported `.txt` files | Location, contacts, files |

Only the standard platform permission required for a local notification receiver (`DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION`) is declared. No storage, contacts, location or network permission is requested.

[Privacy policy](YOUR_PRIVACY_URL)

---

## 📋 Technical details

| Field | Value |
|---|---|
| Package | `com.rohit.rsnotes` |
| Version name / code | `1.2.1` / `2003` |
| Min SDK / Target SDK | `24` (Android 7.0) / `36` |
| APK SHA-256 | `6FEAB4E92C21F9FFB53A44A10723F8DDD5466577E3478D31BE9BC490F70D6C2A` |
| Signing certificate SHA-256 | `AE:CE:55:6B:E6:DD:67:2D:F4:DC:8B:55:65:F2:08:A9:53:76:2F:F2:1D:2E:16:9D:0E:51:19:69:AB:57:75:73` |
| Developer | Rohit Kumar |

You can verify a downloaded APK with:

```powershell
Get-FileHash .\RS_Notes_v1.2.1_universal.apk -Algorithm SHA256
```

---

## 🧱 Build from source

```bash
cd RS_Notes
flutter pub get
flutter build apk --release          # universal APK
flutter build appbundle --release    # signed AAB for Play Console
```

Requirements: Flutter SDK, Android SDK, JDK, and your own signing configuration.

> Do **not** run `flutter clean` on this project. The Gradle memory settings are intentionally tuned for a low-RAM machine (`-Xmx1536m`, `org.gradle.workers.max=1`, `kotlin.daemon.jvmargs=-Xmx768m`).

**Signing material (`key.properties`, keystore) is never committed to this repository.** Keep it offline only.

---

## 📁 Repository structure

```text
.
├── index.html              # 3D landing page (rename the downloaded HTML to this)
├── README.md               # this file
├── screenshots/            # app screenshots used above
├── app-release.apk         # universal release APK (or host it and link above)
└── privacy-policy.html     # optional local copy of the privacy policy
```

---

## 📫 Contact

Bug reports, feedback or privacy questions:
**dellofficial795@gmail.com**

---

## 📄 License

RS Notes is **free to use**. Source code and branding are proprietary; redistribution of modified builds under the same name is not permitted.

---

<p align="center">Made with care for people who want their notes to stay theirs.</p>
