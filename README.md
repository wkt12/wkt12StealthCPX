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
