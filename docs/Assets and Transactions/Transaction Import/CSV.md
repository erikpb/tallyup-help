# CSV Import

CSV (comma-separated values) is the most common export format for bank statements and brokerage accounts. Almost every financial institution offers CSV downloads. Tally Up can import these files directly into an asset.

---

## Entry point

CSV import is asset-level: open an asset's Transactions screen and use the import option in the toolbar.

---

## Import flow

### 1. Select a file

Choose a `.csv` file from your device. Tally Up reads the headers and a preview of the rows.

### 2. Choose a format

Tally Up offers two modes:

- **Predefined formats** — for known providers (such as Interactive Investor), Tally Up already knows the column layout and applies it automatically.
- **Custom** — for any other bank or broker, you map the columns yourself.

If you have imported from the same source before, Tally Up recognises the file's column structure and reloads your previous mapping automatically.

### 3. Review and adjust mappings

For custom imports, you assign each CSV column a role:

| Role | What it means |
|---|---|
| Date | The transaction date |
| Description | The transaction narrative |
| Amount | A single signed amount column |
| Debit / Credit | Separate debit and credit columns |
| Running Balance | End-of-row balance (used for reconciliation) |
| Symbol / Quantity / Price | For investment transaction files |
| Fee / Commission | Costs recorded separately from the main amount |

You can also set parse hints for date formats and decimal separators if your file uses a non-standard convention.

### 4. Preview and import

Tally Up shows a preview of how the first few rows will be imported. Any rows with missing required fields or unparseable values are flagged as warnings.

Confirm to run the import.

---

## Saved mappings

For custom imports, Tally Up saves your column mapping and reuses it the next time you import a file with the same column layout. This means you only need to set up the mapping once per bank or broker.

Saved mappings are matched by the file's column structure, not by filename.

---

## Import summary

After import, Tally Up shows:

- Transactions inserted or updated
- Rows skipped (and why)
- Categories auto-assigned (if enabled)

Reimporting the same file is safe — duplicates are detected and updated rather than inserted again.

---

## Tips

- If your bank offers both CSV and QIF export, prefer QIF — it carries more structure (categories, splits, payee names) than most CSV files.
- For investment accounts, look for an export that includes separate columns for quantity, price, and fees rather than a single net amount.
- If dates are not parsing correctly, check the date format hint in the mapping screen (e.g. `dd/MM/yyyy` vs `MM/dd/yyyy`).
