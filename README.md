# Allergy Trigger Logger — mobile-first version

This is a lightweight web app for logging possible allergy episodes and exporting them for later analysis.

## Main features

- Mobile-first responsive design.
- Larger touch targets suitable for phone use.
- Local browser storage using `localStorage`.
- Add, edit, and delete episodes.
- Export timestamped `.xlsx`, `.csv`, and `.json` files.
- Import `.json` backup on another device.
- Basic Progressive Web App files:
  - `manifest.webmanifest`
  - `service-worker.js`
  - `icon.svg`

## Running locally

Open `index.html` in a browser.

Excel export needs internet access because it loads SheetJS from:

`https://cdn.sheetjs.com/xlsx-0.20.3/package/dist/xlsx.full.min.js`

CSV and JSON export do not need SheetJS.

## Phone access options

### Simple method
Send the folder or `index.html` to the phone and open it in a browser. Local storage will be tied to that browser/device.

### Better method
Host the folder on a simple static host such as GitHub Pages, Netlify, Vercel, or Cloudflare Pages. Then open the link on the phone.

Once hosted, you can usually add it to the home screen:

- iPhone Safari: Share button → Add to Home Screen.
- Android Chrome: Menu → Add to Home screen / Install app.

## Important limitation

Data is local to the device/browser. It does not automatically sync between phone and computer. Use JSON backup/export/import to move data between devices.

## Medical note

This is a tracking tool, not a diagnostic tool. Seek urgent medical care for airway symptoms, wheeze, facial/tongue swelling, collapse, hypotension, or rapidly progressive reactions.
