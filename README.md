Band Merch Organizer v0.3 — Android offline PWA
Upgrade safely from v0.1 or v0.2
Open the existing installed app and Stats > Export backup. Verify the JSON exists in Android Downloads; keep a second copy if possible.
Download this ZIP on Android and extract it using Files.
Open your EXISTING GitHub repository in Chrome (Desktop site if necessary). Replace the seven root files: index.html, app.js, sw.js, manifest.webmanifest, icon.svg, icon-192.png, icon-512.png. Do not upload the enclosing folder. README.md is optional. Commit to main.
In GitHub Actions or Settings > Pages, wait for the deployment to finish. Keep the existing Pages URL and main / (root) configuration.
Open the same Pages URL online. Reload, or close/reopen the installed PWA. Check that the Concert Mode product tiles, payment options and reports appear. Allow a minute for the new service worker to activate. Do NOT clear site data, uninstall, or change domain.
Confirm your existing band, product photos, stock, events and sales are still present. Test airplane mode after loading v0.3 online.
Features
Concert Mode: large one-tap product tiles, category filters, multi-item cart and checkout.
Stock: editable per-product low-stock threshold, initial stock and manual stock movement history, plus sale/void movement history for new transactions. Historical v0.1/v0.2 transactions remain in sales history, but cannot be retroactively reconstructed as stock movements.
Reports: event selection, revenue and unit totals, payment breakdown, CSV export (UTF-8 with BOM).
Payments: Cash/Card/Other on new sales; previous sales are shown as Unspecified rather than guessed.
Backup: JSON export and format-validated import. Same original localStorage key band-merch-v1, data version:1.
Offline: versioned cache for static assets; all inventory and photos stay in browser localStorage.
Important limits
No cloud sync, no server backups, no guaranteed preservation if Android/browser site data is cleared. Photos are compressed but localStorage has size limits. Export a JSON backup regularly, particularly before each update. Voiding a sale restores all items; partial refunds are not supported. This version has not been tested on your specific Android phone.
