🧪 Viber-UI Fake Overlay App (Red Team PoC)

This Android app demonstrates how to overlay a fake Viber chat UI on top of the real Viber app using SYSTEM_ALERT_WINDOW. Intended for Red Team Lab testing only.

⚙️ Features

Draws full-screen fake PNG over Viber app

Uses TYPE_APPLICATION_OVERLAY

Service triggered manually or via AccessibilityService


🚨 Legal Warning

This code is for ethical red team simulation inside closed lab environments only. Never use against real users without written consent.

🔧 Build Instructions

./gradlew assembleDebug
adb install app/build/outputs/apk/debug/app-debug.apk

📁 Folder Structure

Viber-UI/
├── app/
│   ├── src/main/
│   │   ├── java/com/redteam/overlaydemo/
│   │   │   └── OverlayService.kt
│   │   ├── res/layout/
│   │   │   └── overlay_layout.xml
│   │   └── res/drawable/
│   │       └── fake_viber_ui.png
│   └── AndroidManifest.xml
├── build.gradle
├── README.md
├── LICENSE
└── .gitignore

📸 Fake UI Example

You can customize the fake_viber_ui.png with:

Fake login prompt

KBZPay / WavePay confirmation

Social engineering screens


✅ Tested On

Android 10, 11 (Emulators + Physical Devices)

Rooted devices with Frida/Logcat overlay debugging


🛑 Deployment

Not for Google Play

Internal sideload only (adb install)


🧠 Author Notes

Built by Ethan for Red Team overlay phishing simulation. Testing is strictly limited to authorized security research.
