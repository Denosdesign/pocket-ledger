# Pocket Ledger

A small personal expense log that runs in your browser.

## Use

Open `index.html` on GitHub Pages. Tap the centre **+** button to enter an expense, then tap **Save**. Today displays spending and today’s receipt. Use **Receipt** for past entries, **Review** to confirm categories and reconcile records, and **Overview** for monthly spending. Settings offers colour palettes, Light, Dark and System themes, and custom category management.

On iPhone, open the site in Safari, tap **Share**, choose **Add to Home Screen**, then tap **Add**.

Entries and settings are stored locally on your device. Safari and an installed iPhone Home Screen app have separate storage, so export a backup in Safari and import it into the installed app if you already have entries. Clearing browser data may delete your entries.

## Hosting

Static files only. Host the contents of this repository at its root. GitHub Pages works without a build step.

## Notes

Category suggestions through OpenRouter are optional. Known labels are matched locally first and results can be reused without another request. Suggestions of new categories require confirmation; similar names are checked locally before creation. Custom categories can be merged into another category. When enabled, transaction names are sent to the selected provider. Your API key is saved locally in the browser.

Card estimates assume all logged spending was paid with the same card. Reconciliation checks against the statement total you enter.
