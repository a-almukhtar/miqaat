# Miqaat PWA

Installable web version of Miqaat for iPhone/Android.

## Included
- Local prayer-time calculation
- MWL, Umm al-Qura, Egyptian, Karachi, ISNA
- Standard / Hanafi Asr
- Automatic or manual location
- Qibla compass
- Hijri date
- Monthly prayer table
- 24 language choices (English, Arabic, German, French, Dutch and Russian are translated now; the rest are present and currently fall back to English)
- Imported Adhan audio preview
- Offline PWA shell
- Liquid-glass style UI

## Important iPhone limits
A PWA can be installed from Safari without the Apple Developer Program.
However, iOS does not give a PWA the same reliable exact-time background scheduling and unrestricted background audio as a native iOS app. A full Adhan cannot be guaranteed to autoplay while the PWA is closed.

## Free hosting with GitHub Pages
1. Create a free GitHub repository named `miqaat`.
2. Upload the CONTENTS of the `miqaat_pwa` folder.
3. GitHub repository → Settings → Pages.
4. Choose Deploy from branch → `main` → `/ (root)`.
5. Open the HTTPS Pages address in Safari on the iPhone.
6. Tap Share → Add to Home Screen.

## Free hosting with Cloudflare Pages
Upload this folder as a static website. No build command is needed.

## Local Mac test
From Terminal:
`cd miqaat_pwa`
`python3 -m http.server 8080`

Then open http://localhost:8080 on the Mac.
For iPhone geolocation, compass, service worker and notification testing, use the deployed HTTPS site.
