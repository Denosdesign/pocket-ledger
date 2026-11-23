# Pocket Ledger

A small, local spending tracker.

## Features

* Add purchases with a name, amount and date.
* See spending against a monthly budget.
* Review transactions and reconcile them with card statements.
* Track repayments separately from expenses.
* Export and import a JSON backup.
* Optionally get category suggestions through OpenRouter.

## Run locally

No build step or dependencies are required.

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## GitHub Pages

In **Settings → Pages**, select **Deploy from a branch**, then choose `main` and `/ (root)`.

## Data and privacy

Records and settings stay in the browser's local storage. They do not automatically sync between devices. Use the export feature to keep a backup.

OpenRouter is optional. When enabled, it receives the purchase name and available categories, not the transaction amount. The API key is stored in the browser and is not encrypted. Keep a spending limit on the key and do not commit one to the repository.

## Licence

No licence has been selected.
