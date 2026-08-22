# Prayer Companion

A daily prayer journal and prayer-list web app, installable on iPhone/Android as a home-screen app (PWA) via GitHub Pages.

## Files in this folder

- `index.html` — the app itself
- `manifest.json` — tells the phone the app name/icon/colors for home screen install
- `sw.js` — service worker, lets the app open even with no internet
- `icons/icon-192.png`, `icons/icon-512.png` — placeholder app icons (swap these for your own design anytime — just keep the same filenames and sizes)

## How to publish with GitHub Pages

1. **Push these files to your repo**, at the root (or in a `/docs` folder — just be consistent with step 2):
   ```bash
   git add .
   git commit -m "Add Prayer Companion PWA"
   git push
   ```

2. **Enable GitHub Pages:**
   - Go to your repo on GitHub → **Settings** → **Pages**
   - Under "Source," choose the branch (usually `main`) and folder (`/root` or `/docs`)
   - Click **Save**

3. **Get your live URL.** GitHub will show something like:
   ```
   https://yourusername.github.io/your-repo-name/
   ```
   It can take a minute or two to go live the first time.

4. **Install on iPhone:**
   - Open the URL in **Safari** (must be Safari, not Chrome, for iOS install to work)
   - Tap the **Share** icon (square with an arrow)
   - Tap **Add to Home Screen**
   - The app icon appears on the home screen and opens full-screen, no browser bar

## Notes

- Right now, none of the form fields (journal entries, prayer profiles, etc.) save data — it resets on reload. That's the next thing to add if you want it to function as a real journal (can be done with browser local storage, no backend needed).
- To change the icon, replace the two PNG files in `/icons` with your own square images at the same sizes and filenames.
- If you rename the repo or move it into a subfolder on GitHub Pages, double check the paths in `manifest.json` and `index.html` still resolve correctly.
