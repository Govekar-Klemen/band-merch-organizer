# Band Merch Organizer PWA v0.5.1

Interface cleanup release. Uses existing `band-merch-v1` localStorage key and retains product IDs, sales, photos, Flik QR, events, and stock adjustments.

Changes: four category filters (T-shirts, CDs, Hoodies, Other), existing categories normalized on startup, single photo-first Quick Sell grid with two larger cards per row, grouped collapsible sales history by local date with event filter, and validated backup import with a pre-restore local snapshot under `band-merch-v051-pre-restore`.

Import validation rejects malformed references, invalid quantities/prices and duplicate identifiers. It does not guarantee authenticity of user-provided backups. The snapshot is local to the browser and is not a substitute for an exported JSON backup.

To update on Android: export a JSON backup, extract ZIP, upload app files to the existing GitHub Pages repository root replacing same filenames, commit to main, wait for deployment, open the app online and reload, then verify data and offline functionality. Never clear site storage while updating.
