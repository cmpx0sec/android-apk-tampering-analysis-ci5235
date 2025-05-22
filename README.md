# 🔐 Android APK Reverse Engineering & Static Analysis (CI5235)

This project simulates the actions of a suspect employee tampering with an Android APK. I reverse-engineered, modified, and recompiled a calculator app, then analysed its security posture using MobSF. The project aligns with real-world practices in mobile app security and demonstrates reverse engineering, app tampering, permission exploitation, and OWASP risk mapping.

---

## 🧰 Tools Used

- 🛠️ [APK Easy Tool](https://forum.xda-developers.com/t/tool-windows-apk-easy-tool-v1-60-2022-06-23.3333960/) – decompiling & recompiling APKs  
- ✏️ Notepad – editing manifest and XML files  
- 📱 Android Studio Emulator – testing app modifications  
- 🔍 [MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF) – static security analysis  

---

## 📁 What Was Done

- Reverse-engineered the APK of a calculator app using APK Easy Tool.
- Modified the app in the following ways:
  - Added unnecessary location permission in `AndroidManifest.xml`
  - Changed app title to **CipherCalc**
  - Modified button colours and header layout in `colors.xml`
  - Added a "Tampered" label in the layout
  - Embedded a hidden `.txt` file in the APK's internal directory
- Recompiled, signed, and installed the tampered app on a virtual Android device.
- Conducted a full static analysis of both the original and tampered APKs using MobSF.
- Mapped identified risks to the **OWASP Mobile Top 10 (2024)** and proposed mitigations.

---

## 📝 Skills Demonstrated

- APK reverse engineering
- Android app tampering
- Mobile app permission abuse
- Secure app testing
- Static analysis with MobSF
- Risk reporting aligned with OWASP 2024

---

## 📦 Included Files (in `docs/` or download section)

- Original and tampered APKs
- MobSF PDF reports
- Static analysis write-up
- Screenshots of app behavior and tampering
- 5-minute video demo (optional link)



