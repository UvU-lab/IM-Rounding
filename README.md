# Pre-Rounds — home-screen app setup

This folder is the whole app. Hosting it only puts the app's code online — patient
data never leaves your phone.

## 1. Put it online (free, once — GitHub Pages)

Works from a computer or from Safari on your iPhone.

1. Make a free account at github.com.
2. Tap **+ → New repository**. Name it e.g. `prerounds`, set it to **Public**
   (only the code is public — no patient data is ever stored there), tick
   **Add a README file**, then **Create repository**.
3. In the repository: **Add file → Upload files**. Upload these files from this folder:
   `index.html`, `manifest.webmanifest`, `sw.js`, `icon-180.png`, `icon-192.png`, `icon-512.png`.
   Tap **Commit changes**.
4. **Settings → Pages**. Under "Build and deployment", Source = **Deploy from a branch**,
   Branch = **main**, folder **/ (root)** → **Save**.
5. Wait 1–2 minutes, refresh that page — it shows your address, e.g.
   `https://YOUR-USERNAME.github.io/prerounds/`.

## 2. Install it on your iPhone

1. Open that address in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. From now on, always open Pre-Rounds **from the home-screen icon**. The installed app
   keeps its own storage, separate from Safari — anything typed in Safari won't appear there.

It works offline once it has been opened.

## 3. Back up, and move between devices with iCloud Drive

- At the end of each shift: **Save backup file** → **Save to Files** → **iCloud Drive** →
  a folder such as `Pre-Rounds backups`. Files are named with the date and time, so the newest
  one is easy to find.
- On another device (iPhone, iPad, Mac, or a PC with iCloud), open the app, tap
  **Load backup file** and pick the newest file from that folder.
- Loading **merges**. Each patient keeps whichever copy was edited last, new patients are added,
  and patients you deleted on one device stay deleted after you load a later backup.
  Edit on one device at a time and save a backup before switching. If you edit the same
  patient on two devices before syncing, the copy edited last wins.
- The app can't open iCloud files by itself, so you always pick the file in the Files picker.
- The app shows an amber reminder when your last backup file is more than ~20 hours old.
- Turn on **Advanced Data Protection** (Settings → your name → iCloud) to end-to-end encrypt
  iCloud Drive, and delete old backup files you no longer need.

## Updating the app later

Upload the new `index.html` (and `sw.js` if changed) to the same repository. The app picks
up the update next time it opens with a connection and shows a **Reload** banner. Your data
is not affected.

## Privacy

Keep a passcode on your phone, use initials + bed where your site allows, delete old
backup files you no longer need, and clear the list at the end of the rotation.
Check your program's rules on patient lists on personal devices (PHIA in Manitoba).
