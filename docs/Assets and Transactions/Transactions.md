# Transactions

Transactions are the individual entries of activity within an asset — every deposit, withdrawal, trade, and transfer. They are the raw data from which TallyUp builds your reports, categories, and budgets.

---

## Viewing transactions

Open any asset to see its transaction list. Transactions are shown in date order with the date, description, amount, category, and running balance.

You can filter by date range, search by description, or show only uncategorised transactions.

---

## Transaction types

### Cash transactions
| Type | Description |
|---|---|
| **Deposit** | Money coming into the asset |
| **Withdrawal** | Money leaving the asset |
| **Transfer** | Movement of money between two assets in your plan |
| **Interest Income** | Interest earned on the account |
| **Dividend** | Dividend received from a security |

### Investment transactions
| Type | Description |
|---|---|
| **Buy** | Purchase of a security |
| **Sell** | Sale of a security |
| **Move Shares In** | Securities transferred in from another account (no cash effect) |
| **Move Shares Out** | Securities transferred out to another account (no cash effect) |
| **Stock Split** | Corporate action adjusting share quantity |

### Options transactions
| Type | Description |
|---|---|
| **Buy to Open** | Opening a long options position |
| **Buy to Close** | Closing a short options position |
| **Sell to Open** | Opening a short options position |
| **Sell to Close** | Closing a long options position |

---

## Adding a transaction manually

Tap **Add** on the Transactions screen to record a transaction manually. Fill in the date, amount, type, and optionally a payee and description. For investment transactions, you can also specify the security, quantity, price, and commission.

---

## Editing and deleting

Tap any transaction to open it. From there you can edit its details, adjust its category, or delete it.

---

## Categorising transactions

Most cash transaction types can be assigned a category. Categories are stored on **splits** — portions of the transaction amount assigned to a specific category. A simple transaction has one split covering the full amount. See [Categories](Categories.md) for how to set up your category structure.

TallyUp assigns categories automatically using your [Category Rules](Category%20Rules.md). You can review and override these at any time.

---

## Split transactions

A transaction can be divided across multiple categories. For example, a supermarket trip might be split between Groceries and Household. Each split covers a portion of the total amount and can have its own category.

To split a transaction, open it and edit the splits section. Add as many splits as needed — the amounts must sum to the total transaction amount.

---

## Transfer linking

When money moves between two assets in your plan — for example, £500 from a current account to a savings account — TallyUp records a transaction on both sides. These two transactions can be **linked** so the app recognises them as two sides of the same movement, preventing double-counting in reports.

Transfer links are created automatically during import where possible. You can also link or unlink them manually by editing the transfer split on either transaction.

---

## Importing transactions

Rather than adding transactions manually, you can import them in bulk:

- [QIF Import](Transaction%20Import/QIF.md) — from most desktop finance apps and many banks
- [CSV Import](Transaction%20Import/CSV.md) — from bank statement downloads
- [Bank Connections](Transaction%20Import/Bank%20Connections.md) — automatic sync from supported providers

Re-importing the same file is safe — TallyUp detects duplicates and updates rather than creating new entries.
