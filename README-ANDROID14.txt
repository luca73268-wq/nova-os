# NOVA OS for Android 14

This is an installable, offline-capable **web app (PWA)** version of NOVA OS.
It is not a replacement for Android and is not yet a native APK. It opens in its own app-like window once installed.

## Easiest install path on your Android 14 phone

A PWA must be served from HTTPS (or localhost) to install and cache offline. Opening `index.html` directly from Downloads will let you preview it, but won't enable installation/offline caching.

1. Keep the files in this folder together.
2. Upload the folder contents to a static HTTPS host such as GitHub Pages.
3. Open the hosted `index.html` in Chrome on Android.
4. Use Chrome's menu (⋮) and choose **Install app** or **Add to Home screen**.
5. Launch **NOVA OS** from your home screen. After its first successful load, the app shell can work offline.

## Included features

- Desktop-style NOVA OS interface
- Notes saved in browser storage
- Terminal demo and calculator
- Theme settings
- NOVA AI local demo (built-in responses, not a real connected AI model)
- PWA manifest, icons, and offline service worker

## Important limitations

- This is a desktop simulation running inside an app-like browser container, not a new operating system.
- The file manager and system monitor are simulated; web apps cannot freely access Android's entire filesystem or real system metrics.
- NOVA AI is a local demo. A real AI connection needs a backend/API integration and must not expose secret API keys in client-side HTML.
- Browser storage may be cleared by Android or browser settings; export important notes separately.

## Files

- `index.html`: app interface
- `manifest.webmanifest`: install metadata
- `sw.js`: offline cache
- `icons/`: app icons
