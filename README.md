# Flight Records — local-first starter app

This is a prototype of a local-first student progress-sheet app.

## What it does
- Stores student profiles, lesson records, notes, and photos in the browser's IndexedDB on this device.
- Supports camera capture or selecting existing images on compatible phones.
- Searches student names/notes and lesson titles/notes.
- Exports all student records and embedded photos to one JSON backup file.
- Restores a previously exported JSON backup. Restore replaces the records currently in the app, so export first.

## Important limitations
- This is a starter app, not a deployed or certified records system.
- Data stays in this browser/device. It does not sync automatically between your iPhone and Mac.
- Clearing Safari website data, deleting browser data, or device loss can erase records. Export backups regularly and keep at least one copy somewhere else.
- A backup can be large because the original photos are embedded in it. If saving several photos at once fails, try fewer/smaller photos and export regularly.
- Student records may contain private information. Keep backup files in a secure location and do not upload them to a public repository.
- Do not treat this app as a substitute for any official flight-training records or retention requirements.

## How to try it
1. Extract the ZIP.
2. Open `index.html` in a modern browser to test on a computer. Browser security and file-origin rules vary; for dependable iPhone use, serve this static app over HTTPS.
3. For an iPhone home-screen app, host the app code on a free static host (for example, a suitable GitHub Pages setup) and open its HTTPS URL in Safari, then use Share → Add to Home Screen. The app code is hosted, but the records/photos remain in the browser's local storage. Hosting setup is not included in this starter ZIP.
4. Test adding a sample student, attaching a sample photo, exporting a backup, and restoring it before using real student records.

## Backup workflow
- After a training day or weekly, tap **Export all records**.
- Save the downloaded JSON file to the iPhone Files app.
- AirDrop it to your Mac or copy it to an external drive.
- Keep dated backups. To recover, open the app and use **Restore from backup**. Restoring replaces current app records with the backup contents.
