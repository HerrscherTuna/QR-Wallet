# QR Pitaka — installable app

Your GCash, Maya and bank QR codes in one place. It works offline after the first visit, opens full-screen from its own home-screen icon, and keeps your codes on your phone only.

## Files

Upload all of these together, in the same folder (no subfolders):

- `index.html` — the app
- `manifest.webmanifest` — app name, colors and icons
- `sw.js` — lets the app open offline
- `qrcode.js`, `jsQR.js` — make and read QR codes
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` — app icons

## Put it online for free (GitHub Pages)

1. Sign in at github.com (create a free account if needed).
2. Click **+** → **New repository**. Name it `qr-pitaka`, set it to **Public**, and click **Create repository**.
3. Click **uploading an existing file**, drag in all the files above, then click **Commit changes**.
4. Go to **Settings** → **Pages**. Under *Branch*, choose **main** and **/(root)**, then **Save**.
5. Wait 1–2 minutes. Your app's address appears at the top of that page, like `https://YOUR-USERNAME.github.io/qr-pitaka/`.

The page is public, but your QR codes are never uploaded. They are stored only in the phone that adds them.

## Install it on your phone

- **Android (Chrome):** open the address. Tap **Install** on the banner, or **⋮** → **Install app** / **Add to Home screen**.
- **iPhone (Safari):** open the address, tap **Share**, then **Add to Home Screen**.

Then open QR Pitaka from your home screen.

## Keep your codes safe

Codes live in the app's storage on that phone. Clearing your browser data or uninstalling can erase them.
Tap **Back up codes** now and then and keep the file (Google Drive or email to yourself). On a new phone, use **Restore backup**.

## Updating the app later

Upload the changed files to the same repository, and change `pitaka-v1` in `sw.js` to `pitaka-v2` (then `v3`, and so on). That tells phones to fetch the new version. Close and reopen the app twice to see it.

## Before relying on amounts

Some wallets ignore the amount on personal (person-to-person) QR codes. For each wallet, make an amount QR, scan it from another phone, and check that the right amount and your name appear. Send ₱1 to confirm.
