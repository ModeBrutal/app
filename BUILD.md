# X'Boy Toolkit — Build Guide
## by X'Boy Linux

---

## ✅ Cara Build APK Native (Capacitor)

### 1. Install Node.js
Download: https://nodejs.org (pilih LTS)

### 2. Install Android Studio
Download: https://developer.android.com/studio
- Install Android SDK
- Install Android SDK Build-Tools
- Set ANDROID_HOME environment variable

### 3. Extract ZIP ini, buka terminal di folder ini

### 4. Install dependencies
```bash
npm install
```

### 5. Add Android platform
```bash
npx cap add android
```

### 6. Sync web assets
```bash
npx cap sync android
```

### 7. Build APK
```bash
cd android
./gradlew assembleDebug
```

### 8. APK ada di:
```
android/app/build/outputs/apk/debug/app-debug.apk
```

---

## ✅ Cara Build APK — Android Studio GUI

1. Buka Android Studio
2. File → Open → pilih folder `android/` dari project ini
3. Tunggu Gradle sync selesai
4. Build → Build Bundle(s)/APK(s) → Build APK(s)
5. APK selesai → klik "locate" untuk nemuin file-nya

---

## ✅ Cara Build APK Release (untuk distribusi)

```bash
cd android
./gradlew assembleRelease
```
Lalu sign APK dengan keystore kamu.

---

## Info App
- App ID: com.xboy.toolkit
- Nama: X'Boy Toolkit
- Versi: 2.0.0
- Developer: X'Boy Linux
- Web dir: www/
