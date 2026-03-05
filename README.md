# 🚀 PushToApp

> **Wrap any website or HTML project into a real Android APK — no coding required.**

**PushToApp** is a fully browser-based tool that generates a complete Android project from your website URL or local project files. Fill out a 4-step form, download the ZIP, push it to GitHub, and GitHub Actions builds your APK automatically in minutes.

**No server. No installation. No account. Completely free.**

---

## ✨ Features

| Feature | Description |
|---|---|
| 🌐 Website URL or Project Files | Wrap a live URL or upload multiple local files (HTML, CSS, JS, images, fonts, and more) |
| ✨ Splash Screen | Animated launch screen with your icon and app name |
| 🔄 Pull-to-Refresh | Swipe down to reload — native Android feel |
| ◀ Back Button Support | Hardware back navigates your web page history |
| ✈ Offline Fallback | Friendly no-internet page instead of a broken screen |
| 🔒 PIN / Biometric Lock | Require fingerprint or PIN to open the app |
| 📎 File Upload Support | Enables `<input type="file">` inside the WebView |
| 🛡 Block Screenshots | Prevents screenshots and screen recording |
| 🔄 App Update Check | Prompts users when a new version is available |
| ⚙ Custom JS Injection | Run your own JavaScript after every page load |
| 🔐 Force HTTPS Only | Blocks insecure HTTP requests in the WebView |
| ⛶ Fullscreen Mode | Immersive experience — hides status & nav bars |

---

## 🚀 How It Works

```
Step 1 → Enter your website URL (or upload project files) + set app identity
Step 2 → Upload your icon and choose your brand colors
Step 3 → Toggle features on/off (PIN lock, offline mode, pull-to-refresh, etc.)
Step 4 → Download the Android project ZIP → push to GitHub → get your APK
```

### GitHub Actions Build (Free)

1. Download the ZIP from PushToApp
2. Create a new GitHub repository
3. Push the ZIP contents to the repo
4. GitHub Actions automatically builds the APK
5. Download your `.apk` from the Actions tab in **3–5 minutes**

---

## 📁 Generated Project Structure

```
your-app/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/<package>/MainActivity.java
│   │       ├── assets/                  # Your uploaded HTML/CSS/JS files
│   │       ├── res/
│   │       │   ├── drawable/            # Splash screen assets
│   │       │   ├── mipmap-*/            # Auto-scaled app icons (all densities)
│   │       │   ├── layout/              # XML layouts
│   │       │   └── values/              # Colors, strings, themes
│   │       └── AndroidManifest.xml
│   └── build.gradle
├── .github/
│   └── workflows/
│       └── build.yml                    # GitHub Actions APK builder
├── build.gradle
├── gradle.properties
└── settings.gradle
```

---

## ⚙️ Configuration Options

### Step 1 — App Information
- **Source Type** — Live website URL or upload project files (HTML, CSS, JS, images, fonts, JSON, and more)
- **Entry Point** — Choose which HTML file is the main entry point when multiple files are uploaded
- **App Name** — Displayed on the home screen
- **Version** — Semantic version (e.g. `1.0.0`)
- **Short Description** — Optional, shown in internal docs / store listings
- **Developer / Company Name**
- **Contact Email**
- **Package ID** — Auto-generated from your app name (e.g. `com.yourname.appname`)

### Step 2 — Branding
- **App Icon** — PNG, 512×512 recommended (auto-scaled to all densities)
- **Primary Color** — Main theme color
- **Accent Color** — Splash screen & UI accent
- **Splash Screen Style** — Icon only or icon + app name

### Step 3 — Feature Toggles
All features are pre-coded and injected automatically — just flip the switch:

```
✅ Pull-to-Refresh
✅ Back Button Navigation
✅ Offline Fallback Page
✅ PIN / Biometric Lock
✅ File Upload Support
✅ Block Screenshots
✅ App Update Check
✅ Custom JavaScript Injection
✅ Force HTTPS Only
✅ Fullscreen / Immersive Mode
```

---

## 📦 Supported Upload File Types

When using **Upload Project Files** mode, PushToApp accepts:

```
Web     → .html .htm .css .js .mjs .ts .jsx .tsx .json .xml .svg
Images  → .png .jpg .jpeg .gif .webp .ico
Fonts   → .woff .woff2 .ttf .otf .eot
Docs    → .txt .md .csv .pdf
```

> `index.html` is used as the entry point by default. If you have multiple HTML files, you can select the entry point manually.

---

## 💾 My Apps

PushToApp automatically saves your previous builds locally in the browser. Access them anytime from the **My Apps** button — no account or cloud sync needed. You can re-download or delete saved projects at any time.

---

## 🛠 Tech Stack

- **Frontend** — Vanilla HTML, CSS, JavaScript
- **Fonts** — Syne · DM Sans · JetBrains Mono
- **ZIP Generation** — [JSZip](https://stuk.github.io/jszip/) (client-side, no server)
- **Build System** — Gradle + GitHub Actions
- **Target** — Android 5.0+ (API 21+)
- **WebView Engine** — Android System WebView (Chromium)

---

## 📋 Requirements

To build the APK you need:

- A free [GitHub](https://github.com) account
- A public or private GitHub repository
- That's it — builds run entirely on GitHub's free CI servers

---

## 🔒 Privacy

> All processing happens **entirely in your browser.**
> No data is sent to any server. Your files, URL, and configuration never leave your device.

---

## 📦 Version

**PushToApp v2.0** — Browser-based · No install · No account required

---

*by [@shikwonh](https://github.com/shikwonh)*
