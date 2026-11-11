# JL Inventory Report

Frontend-only inventory management and reporting app with JL branding. No backend, no server, no cloud database.

## Features
- JL opening animation (skippable, reduced-motion aware)
- Dashboard with KPIs, value by category, recent movements and upcoming schedule
- Inventory register with CSV / Excel import
- Stock In / Stock Out with weighted average costing and negative-stock prevention
- Calendar (month, week, day, agenda, upcoming), recurring events, reminders, snooze, notification center
- Reports: print to PDF, Excel export, Word export
- ICS / CSV calendar export, ICS import
- JSON backup and restore (inventory, transactions, events, notifications)

## Privacy
All data is stored in the browser's IndexedDB on the user's device. Nothing is sent to any server. Sharing the app never shares inventory records. Clearing browser data deletes local records, so download backups regularly.

## Run locally
Open `index.html` in a browser (needs internet once to load the Excel library from cdnjs), or serve the folder with any static server.

## Deploy
The included GitHub Actions workflow publishes the site to GitHub Pages on every push to `main`. In the repository go to Settings > Pages and set Source to "GitHub Actions".

## Limitations
Alarms fire only while the page is open in a browser tab. Not yet built: transfers, adjustments, physical counts, suppliers, purchase orders, assets, FIFO costing, optional password lock.
