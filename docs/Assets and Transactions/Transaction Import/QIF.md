# QIF Import

QIF (Quicken Interchange Format) is a widely supported export format produced by most desktop finance apps and many online banking portals. Tally Up can import QIF files to bring in your transaction history quickly.

---

## Entry points

You can import a QIF file at two levels:

- **Plan level** — imports all accounts in the file, optionally creating new assets for accounts that don't yet exist in your plan. Access this from the toolbar on the Assets screen.
- **Asset level** — imports transactions from the file into a single selected asset. Access this from the toolbar on the Transactions screen for that asset. The file must contain only one account.

---

## What gets imported

- Transactions with date, amount, payee, and memo
- Split transactions (a single transaction divided across multiple categories)
- Categories — created automatically if not already present
- Account balance — if the QIF file includes a current balance, Tally Up sets the asset's balance to match

---

## Pre-import review

Before any data is written, Tally Up shows a review screen. For plan-level imports, this includes:

- Which accounts in the file map to which assets in your plan
- Any new assets that will be created, including their proposed type, currency, and owners
- Warnings about unsupported QIF sections or malformed rows (informational — these do not block the import)

You can adjust the mapping, currency, and owner assignments before confirming. Accounts you do not want to import can be skipped.

---

## Import summary

After the import completes, Tally Up shows a summary:

- Assets created or skipped
- Transactions inserted or updated
- Categories created or reused
- Any warnings (split mismatches, skipped rows)

Importing the same file twice is safe — Tally Up detects duplicates and updates existing transactions rather than creating new ones.

---

## Currency detection

For plan-level imports, Tally Up tries to determine the correct currency for each account automatically before showing the review screen. It checks in this order:

1. **Account name** — if the account name contains a three-letter ISO currency code (e.g. `Savings USD` or `GBP Current Account`), that currency is used.
2. **Filename** — if the QIF filename contains an isolated three-letter currency code (e.g. `transactions-GBP-2024.qif`), that currency is used.
3. **Existing asset** — if the account maps to an asset already in your plan, that asset's currency is used.
4. **Base currency** — if none of the above apply, your app base currency is used as the default.

If the account name and filename both contain currency codes and they conflict, Tally Up leaves the currency blank and requires you to choose one in the review screen before proceeding.

You can always override the detected currency in the review screen before confirming the import.

---

## Categories from QIF

Categories in the QIF file are created automatically in Tally Up. If a category already exists with the same name, it is reused. The category hierarchy from the QIF file is preserved.

Category Rules are **not** applied during QIF import — the categories in the file are used directly.

---

## Tips

- Export the longest history available from your bank or finance app before importing. Tally Up handles large files well.
- For plan-level imports, review the account-to-asset mapping carefully before confirming — especially if account names in the file differ from your asset names in Tally Up.
- If you have already categorised some transactions manually, QIF import will not overwrite those categories with its own unless you re-import the same transactions.
