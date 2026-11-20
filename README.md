# NODA POS — Official App Releases 📱📦

Official public release repository for **NODA POS (Point of Sale)** (`com.nodapos.pos`).

This repository hosts official signed release APKs, SHA-256 checksums, changelogs, and installation instructions for Android cash registers, tablets, and mobile devices.

---

## 📥 Download Latest Version

You can always download the latest production APK directly from the [Releases](https://github.com/CarlArvie/pos-releases/releases) tab.

* **Latest Release:** [View Latest Release (v1.1.4)](https://github.com/CarlArvie/pos-releases/releases/latest)
* **Direct APK Download:** Look for `app-release.apk` (universal) under the Assets section of the latest release, or pick `app-arm64-v8a-release.apk` / `app-armeabi-v7a-release.apk` for smaller architecture-specific downloads.

> **Upgrading from `v1.1.3` or earlier:** `v1.1.4` officially rebrands the app to **NODA POS**, changes the Android package ID from `com.example.pos` to `com.nodapos.pos`, and introduces the production release signing key. Android will install `v1.1.4` as a new app alongside `v1.1.3`. Sign in once on **NODA POS v1.1.4** to sync your cloud data, then uninstall the older `pos` app. Starting from `v1.1.4` onward, in-place OTA updates work seamlessly with automatic signing-certificate and SHA-256 verification.

---

## ⚡ How the In-App Updater Works

Installed NODA POS applications automatically check this repository on app startup and cashier login.
* When a newer version tag (e.g. `v1.1.4`) is published here with an attached APK, every older app instance (`v1.1.3`, `v1.1.2`, `v1.1.1`, `v1.1.0`, or `v1.0.0`) will automatically pop up an **Update Available** notification.
* Cashiers and store managers can tap **"Update Now"** to download, verify (HTTPS allowlist + SHA-256 checksum + APK signing certificate match), and install the new APK without needing access to the private source code repository.
* If preferred, managers can also check manually inside the app:
  * **Settings ➔ Check for App Updates**
  * **Device Information ➔ Software Updates**

---

## 📲 Installation Guide for Android Devices

1. **Download APK:** Download `app-release.apk` (or `app-arm64-v8a-release.apk` / `app-armeabi-v7a-release.apk` for low-end 32-bit devices) on your Android device (via Chrome browser).
2. **Allow Installation:** If prompted *"For your security, your phone is not allowed to install unknown apps from this source"*, tap **Settings** and enable **"Allow from this source"**.
3. **Install:** Tap **Install** (or **Update** if updating an existing `v1.1.4+` installation).
4. **Launch:** Open **NODA POS** and log in with your account or store PIN.

---

## 📋 Release History & Changelogs

| Version | Release Date | Summary |
|---|---|---|
| `v1.1.4` | 2026-11-20 | **NODA POS Rebrand & Comprehensive Security Hardening:** Official **NODA POS** branding (`com.nodapos.pos`), new adaptive launcher icon, compact Material 3 Admin Drawer header with live store/register context, signed & R8-obfuscated release builds, hardened OTA updater (HTTPS allowlist + SHA-256 + signing-cert check + universal APK preference), PBKDF2-HMAC-SHA256 PIN hashing with exponential lockout, hardened Supabase RLS/RPCs, CSV formula injection protection, strong password policy + HIBP breach check, fail-closed AuthGuard, and sanitized UI error messages. |
| `v1.1.3` | 2026-11-15 | New **By Product** sales report tab (searchable/filterable full-catalog sales, variant grouping, 0-sales dead-stock filter, lazy per-product trend/receipt drill-down sheet, RBAC-gated P&L columns, and enriched Excel export) + **Allow Negative Stock** now disabled by default (configurable in Settings). |
| `v1.1.2` | 2026-11-15 | Allow negative stock sales (default ON, Admin toggle in Settings), product/variant archive & staff soft-delete fixes with UTC sync resurrection protection, Staff & Cashiers enable/disable toggle (disabled by default, hidden from drawer when off). |
| `v1.1.1` | 2026-11-08 | Comprehensive RBAC Security & Manager Overrides, Employee Payroll Management & Payslip Export, Inter-Store Stock Transfers, Waste & Damage Ledger, Cash Denomination Shift Close, Line-Item Cart Discounts & Notes, ESC/POS Hardware. |
| `v1.1.0` | 2026-11-02 | Multi-store inventory isolation, product barcodes, customer credit & loyalty points, split bills, refund approvals. |
| `v1.0.0` | Initial Release | Core POS, offline SQLite, shift attendance, multi-store inventory isolation, Supabase sync. |

---

## 🔒 Security & Privacy Notice
This repository is exclusively dedicated to distributing signed, verified production binaries and release notes. The application source code is maintained privately by the development team.
