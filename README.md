# Pocket Ledger

Per-C's personal expense tracker. Sections like Room, budgets, PDF reports, backups. Works offline once opened.

## Put it on GitHub Pages

1. On github.com, create a new repository, for example `pocket-ledger` (Public).
2. Click **Add file → Upload files** and drag in everything from this folder:
   `index.html`, `manifest.json`, `sw.js`, `README.md` and the whole `icons` folder.
   Click **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**,
   branch **main**, folder **/ (root)**, then **Save**.
4. After a minute your app is live at `https://YOUR-USERNAME.github.io/pocket-ledger/`.

## Add it to your home screen

- **iPhone (Safari):** open the link, tap **Share → Add to Home Screen → Add**.
- **Android (Chrome):** open the link, tap **⋮ → Add to Home screen** (or **Install app**).

It opens full screen with the Pocket Ledger icon, like a normal app.

## Move your data from the Claude version

1. In the Claude version: **Settings → Download backup**.
2. In the new app: **Settings → Restore from backup → Add to my data**.

## Good to know

- Your expenses are saved **on that phone only**. Download a backup every now and then
  (Settings → Download backup → Save to Files) so nothing is lost if the phone is reset.
- **Changing the icon:** replace the PNGs in `icons/` with yours, same names and sizes
  (`apple-touch-icon.png` 180×180, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` 512×512 with the logo in the middle 80%, `favicon-32.png`).
- **Uploading a new version:** upload the new `index.html`, then open `sw.js`, change
  `pocket-ledger-v1` to `pocket-ledger-v2` (and so on) and commit. Close and reopen the app twice to get the update.
