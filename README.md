# Pocket Ledger

A small personal expense log that runs in your browser.

## Use

Open `index.html` on GitHub Pages. Tap the centre **+** button to enter an expense, then tap **Save**. Today shows cumulative spending for the current financial month by default, with a small switch beside the heading to show today’s spending instead. Today’s receipt remains below the total. Use **Receipt** for past entries, **Review** to confirm categories, and **Overview** for monthly spending. Settings offers colour palettes, Light, Dark and System themes, a configurable financial month start date and custom category management. The financial month applies to budget tracking and monthly totals. Dates 29 to 31 use the last day of shorter months.

On iPhone, open the site in Safari, tap **Share**, choose **Add to Home Screen**, then tap **Add**.

Entries and settings are stored locally on your device. Safari and an installed iPhone Home Screen app have separate storage, so export a backup in Safari and import it into the installed app if you already have entries. Clearing browser data may delete your entries.

## Hosting

Static files only. Host the contents of this repository at its root. GitHub Pages works without a build step.

## Notes

Category suggestions through OpenRouter are optional. Known labels are matched locally first and results can be reused without another request. Suggestions of new categories require confirmation; similar names are checked locally before creation. Custom categories can be merged into another category. When enabled, transaction names are sent to the selected provider. Your API key is saved locally in the browser.

The app focuses on logging expenses, reviewing categories and monitoring spending against your financial month budget. Previous card balances and reconciliation records remain in older locally saved data and backups, but the card tracking interface has been removed.
