# NOVA — YouTube Companion PWA

A minimal home-screen companion for searching YouTube, launching YouTube or attempting to hand a search to Brave, and saving recent searches locally.

## Deploy
This must be hosted on HTTPS to be installable as a proper iPhone Home Screen web app.
1. Create a GitHub repository (e.g. `nova-youtube`).
2. Upload all files in this folder to the repository root.
3. In repository Settings → Pages, choose Deploy from a branch, `main`, `/ (root)`, then Save.
4. Wait for the Pages URL (https://USERNAME.github.io/nova-youtube/).
5. Open that URL in Safari on iPhone → Share → Add to Home Screen → enable Open as Web App if shown → Add.

## Limitations
- This is not a full browser engine and does not embed or proxy YouTube.
- YouTube searches open the YouTube website. The Brave shortcut attempts the iOS Brave URL scheme; if that does not open, it copies the YouTube URL for manual opening in Brave.
- Ad blocking is provided by Brave only when the destination opens in Brave. The PWA itself cannot block YouTube ads.
- Background playback is controlled by YouTube/Brave and iOS. The PWA cannot grant itself native background-audio privileges.
- Saved searches use localStorage on this device/browser.
