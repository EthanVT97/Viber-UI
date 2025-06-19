# 🧪 Viber-UI Fake Overlay App (Red Team PoC)

This Android app demonstrates how to overlay a fake Viber chat UI 
on top of the real Viber app using `SYSTEM_ALERT_WINDOW`. Intended 
for Red Team Lab testing only.

## ⚙️ Features
- Draws full-screen fake PNG over Viber app
- Uses `TYPE_APPLICATION_OVERLAY`
- Service triggered manually or via AccessibilityService

## 🚨 Legal Warning
**This code is for ethical red team simulation inside closed lab environments only. Never use against real users without written consent.**

## 🔧 Build Instructions

```bash
./gradlew assembleDebug
adb install app-debug.apk
