# Expense Tracker (PWA)

Files: index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png, icon-maskable-512.png, apple-touch-icon.png

## Turn it into an APK
1. Put ALL these files together in a folder on any HTTPS host (GitHub Pages works).
   Keep them in the same folder; paths are relative, so a sub-folder is fine.
2. Open the hosted link in Chrome on your phone. You should get an "Install app" option.
3. Go to https://www.pwabuilder.com, paste the link, press Start.
4. Choose Package for stores > Android > Generate. Download the zip.
5. Inside: an .apk (install directly) and an .aab (Play Store). Keep the signing key file and its passwords safe.
   You need the same key for every future update.

## Notes
- Data is stored on the phone (localStorage). Use "Export backup" at the bottom of the Track page now and then.
- To release an update: change the files, then bump `V` in sw.js (expense-tracker-v5 -> v6).
- Works offline after the first load.
