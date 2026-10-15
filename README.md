# Vendo

A personal virtual snack vending machine. Scan your snacks in, get 2 tokens a day, vend responsibly (or break the glass).

Static web app: no build step, no backend. All data stays in the browser (localStorage).

## Deploy on GitHub Pages
1. Push this folder to a repo (e.g. `vendo`).
2. Settings > Pages > Deploy from a branch > `main` / root.
3. Open `https://<username>.github.io/vendo/` on your iPhone in Safari > Share > Add to Home Screen.

## Notes
- Barcode lookup uses the Open Food Facts public API (name, brand, front image). Unknown barcodes: type a name and take a photo.
- Camera scanning uses the browser BarcodeDetector API. If unsupported (e.g. some iOS Safari versions), type the barcode number.
- Needs HTTPS for the camera (GitHub Pages provides it).
- Files: `index.html` (app), `manifest.webmanifest` + `sw.js` + `icons/` (installable, offline).
