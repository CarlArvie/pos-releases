# POS Android — Official App Releases 📱📦

Official public release repository for the **POS Android (Point of Sale)** system.

This repository hosts official release APKs, changelogs, and installation instructions for Android cash registers, tablets, and mobile devices. 

---

## 📥 Download Latest Version

You can always download the latest production APK directly from the [Releases](https://github.com/CarlArvie/pos-releases/releases) tab.

* **Latest Release:** [View Latest Release](https://github.com/CarlArvie/pos-releases/releases/latest)
* **Direct APK Download:** Look for `app-release.apk` under the Assets section of the latest release.

---

## ⚡ How the In-App Updater Works

Installed POS applications automatically check this repository on app startup and cashier login.
* When a newer version tag (e.g. `v1.0.1`) is published here with an attached APK, every older app instance (`v1.0.0`) will automatically pop up an **Update Available** notification.
* Cashiers and store managers can tap **"Update Now"** to instantly download and install the new APK without needing access to the private source code repository.
* If preferred, managers can also check manually inside the app:
  * **Settings ➔ Check for App Updates**
  * **Device Information ➔ Software Updates**

---

## 📲 Installation Guide for Android Devices

1. **Download APK:** Download `app-release.apk` on your Android device (via Chrome browser).
2. **Allow Installation:** If prompted *"For your security, your phone is not allowed to install unknown apps from this source"*, tap **Settings** and enable **"Allow from this source"**.
3. **Install:** Tap **Install** (or **Update** if updating an existing version).
4. **Launch:** Open the app and log in with your store PIN.

---

## 📋 Release History & Changelogs

| Version | Release Date | Summary |
|---|---|---|
| `v1.0.1` | *(Upcoming)* | Daily sales isolation fix in reports, daily sales breakdown cards, automatic GitHub in-app updater. |
| `v1.0.0` | Initial Release | Core POS, offline SQLite, shift attendance, multi-store inventory isolation, Supabase sync. |

---

## 🔒 Security & Privacy Notice
This repository is exclusively dedicated to distributing compiled production binaries and release notes. The application source code is maintained privately by the development team.
