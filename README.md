# 🕶️ WKT12StealthCPX – Covert TCP Intelligence Rewriter  
**"Encrypt the handshake. Mask the metadata."**

## 🔐 Overview
WKT12StealthCPX injects encrypted content into TCP SYN packets and cloaks handshake metadata for stealth-grade network operations. Featuring a toggleable GUI, encrypted audit logging, and integration with your `AdminHash` module, this tool transforms how packets whisper.

---

## 🎛️ GUI Features (Android APK)

| Button                        | Function                                           |
|------------------------------|----------------------------------------------------|
| 🚀 Launch Stealth Injection  | Activates SYN packet injector + handshake encoder  |
| 🧾 View Log                  | Displays latest encrypted TCP logs                 |
| 🔒 Enable Admin Gate         | Requires AdminHash verification before launching   |
| ⚙️ Settings                  | Configure retries, delays, and log behavior        |

---

## 📂 Folder Structure

```plaintext
android/wkt12StealthCPX/
├── gui-wrapper/
│   ├── src/
│   │   ├── main/java/com/wkt12/stealthcpx/
│   │   │   └── MainActivity.java
│   │   ├── res/layout/
│   │   │   └── activity_main.xml
│   │   └── assets/scripts/
│   │       ├── tcp_encryptor.c
│   │       └── launcher.sh
│   └── AndroidManifest.xml
├── launcher.sh
├── splash.txt
└── README.md
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.wkt12.stealthcpx">

    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
    <!-- Optional for rooted ops -->
    <uses-permission android:name="android.permission.ACCESS_SUPERUSER" />

    <application
        android:allowBackup="false"
        android:label="WKT12StealthCPX"
        android:icon="@drawable/logo_tb3"
        android:theme="@style/Theme.AppCompat.Light.DarkActionBar">

        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>

    </application>
</manifest>
