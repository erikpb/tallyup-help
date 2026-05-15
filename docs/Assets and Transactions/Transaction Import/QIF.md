# QIF Import

QIF (Quicken Interchange Format) is a widely supported export format produced by most desktop finance apps and many online banking portals. TallyUp can import QIF files to bring in your transaction history quickly.

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
- Account balance — if the QIF file includes a current balance, TallyUp sets the asset's balance to match

---

## Pre-import review

Before any data is written, TallyUp shows a review screen. For plan-level imports, this includes:

- Which accounts in the file map to which assets in your plan
- Any new assets that will be created, including their proposed type, currency, and owners
- Warnings about unsupported QIF sections or malformed rows (informational — these do not block the import)

You can adjust the mapping, currency, and owner assignments before confirming. Accounts you do not want to import can be skipped.

---

## Import summary

After the import completes, TallyUp shows a summary:

- Assets created or skipped
- Transactions inserted or updated
- Categories created or reused
- Any warnings (split mismatches, skipped rows)

Importing the same file twice is safe — TallyUp detects duplicates and updates existing transactions rather than creating new ones.

---

## Categories from QIF

Categories in the QIF file are created automatically in TallyUp. If a category already exists with the same name, it is reused. The category hierarchy from the QIF file is preserved.

Category Rules are **not** applied during QIF import — the categories in the file are used directly.

---

## Tips

- Export the longest history available from your bank or finance app before importing. TallyUp handles large files well.
- For plan-level imports, review the account-to-asset mapping carefully before confirming — especially if account names in the file differ from your asset names in TallyUp.
- If you have already categorised some transactions manually, QIF import will not overwrite those categories with its own unless you re-import the same transactions.
