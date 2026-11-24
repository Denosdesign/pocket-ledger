# Pocket Ledger

A small personal expense log that runs in your browser.

## Use

Open `index.html` on GitHub Pages. Tap the centre **+** button to enter an expense, then tap **Save**. Today shows cumulative spending for the current financial month by default, with a small switch beside the heading to show today’s spending instead. Today’s receipt remains below the total. Use **Receipt** for past entries, date range searches, 50 entry pages and CSV exports. Use **Review** to confirm categories, and **Overview** for monthly spending. Settings offers colour palettes, Light, Dark and System themes, a configurable financial month start date and custom category management. The financial month applies to budget tracking and monthly totals. Dates 29 to 31 use the last day of shorter months.

On iPhone, open the site in Safari, tap **Share**, choose **Add to Home Screen**, then tap **Add**.

Entries are stored individually in IndexedDB on your device, with date indexes for period queries. Settings are stored in the same database. On first launch after this update, an existing `pocket-ledger-v1` localStorage ledger is copied into IndexedDB and verified. The old browser data is left untouched as an emergency fallback. Download a full JSON backup after upgrading. Clearing browser data or uninstalling the app may delete local records. Safari and an installed iPhone Home Screen app have separate storage, so transfer data between them using a JSON backup.

## Hosting

Static files only. Host the contents of this repository at its root. GitHub Pages works without a build step.

## Notes

Category suggestions through OpenRouter are optional. Known labels are matched locally first and results can be reused without another request. Suggestions of new categories require confirmation; similar names are checked locally before creation. Custom categories can be merged into another category. When enabled, transaction names are sent to the selected provider. Your API key is saved locally in the browser.

The app focuses on logging expenses, reviewing categories and monitoring spending against your financial month budget. Previous card balances and reconciliation records remain in older locally saved data and backups, but the card tracking interface has been removed.

## Backup and history

**Settings → Data → Download JSON** exports all records in backup format v2, excluding your OpenRouter API key. Older v1 backups can also be imported. **Merge** skips records with IDs already present. **Replace** discards the current ledger after confirmation. Receipt CSV exports only the chosen date range and is not a restore backup. The app does not automatically sync between devices.

## Smart tools

Smart Capture is available from the new expense sheet. Parse simple lists locally or explicitly ask the configured AI provider to interpret more complex text. Review and edit every proposed entry before saving. Receipt includes Ask your ledger: the model interprets a question into a restricted query, and the local database calculates the answer. Overview shows a local spending forecast and comparable period statistics, with optional AI insights cached on the device. Review includes a local check of the past 90 days for duplicates, unusually large purchases, inconsistent categories and potential recurring payments. These checks never automatically change records.

Smart Capture sends the entered text and category context only when Ask AI is selected. Ledger queries send the question and date/category context, not transaction history. Generated insights send aggregated figures only. Ordinary manual capture, forecasts and review checks continue to work without AI. Reports are estimates based on recorded spending, not a guarantee of future spending. No new database schema or data migration is required.
